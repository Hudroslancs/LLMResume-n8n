# AGENTS.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Project Overview

AI-powered resume tailoring system that automatically rewrites a master resume to match job descriptions. Triggered via Telegram, processed by Llama3, and delivered as a PDF.

## Tech Stack

- **Automation**: n8n (self-hosted)
- **AI Model**: Llama3 via Ollama
- **PDF Generation**: Gotenberg (Chromium-based)
- **Delivery**: Telegram Bot
- **Infrastructure**: Proxmox LXC, Cloudflare Zero Trust
- **Storage**: Nextcloud

## Architecture

### n8n Workflow Pipeline (`My workflow.json`)

```
Telegram Trigger (receive JD)
    ↓
HTTP Request (fetch master_resume.md from GitHub)
    ↓
AI Agent (Llama3 rewrites resume for JD)
    ↓
Markdown → HTML conversion
    ↓
JavaScript (convert to binary)
    ↓
Gotenberg API (HTML → PDF)
    ↓
Telegram (send PDF)
```

### Key Files

- `master_resume.md` - Source resume with embedded CSS for print-ready PDF output. CSS controls precise margins, fonts, and page breaks.
- `My workflow.json` - n8n workflow definition (import into n8n to use)

## Important Constraints

### Resume Styling
The `master_resume.md` uses inline `<style>` with millimeter-based margins and specific fonts. When modifying:
- Preserve the `@page` margin settings for PDF consistency
- Keep `page-break-inside: avoid` rules for clean section breaks
- Font sizes are calibrated for professional A4 output (11px body, 26px name)

### AI Agent Prompts
The workflow uses specific system prompts to ensure:
- ATS-optimized output
- No invented facts
- Original Markdown/CSS preserved
- Action-oriented language

### External Dependencies
The workflow fetches `master_resume.md` directly from GitHub raw URL. Changes to the resume require pushing to the `main` branch.
