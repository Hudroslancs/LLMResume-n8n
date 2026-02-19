<style>
@page {
    margin-top: 10mm;
    margin-bottom: 10mm;
}
@import url('https://fonts.googleapis.com/css2?family=Helvetica:wght@400;700&display=swap');

body {
    font-family: 'Helvetica', Arial, sans-serif;
    line-height: 1.4;
    color: #1a1a1a;
    max-width: 900px;
    margin: auto;
    padding: 5px 50px 20px 50px;
}

h1 {
    text-align: left;
    color: #004a99;
    font-size: 26px;
    margin-bottom: 5px;
    text-transform: uppercase;
    letter-spacing: 1px;
}

p {
    margin: 2px 0;
    font-size: 11px;
    color: #333;
}

a {
    color: #004a99;
    text-decoration: none;
}

h2 {
    color: #004a99;
    font-size: 15px;
    margin-top: 20px;
    text-transform: uppercase;
}

h3 {
    color: #1a1a1a;
    font-size: 12.5px;
    margin-bottom: 2px;
    margin-top: 10px;
}

ul {
    margin-top: 5px;
    padding-left: 18px;
}

li {
    font-size: 11px;
    margin-bottom: 4px;
    text-align: justify;
}

.sub-info {
    font-size: 10.5px;
    font-style: italic;
    color: #555;
}

@media print {
    h2, h3 {
        page-break-after: avoid;
    }
    section {
        page-break-inside: avoid;
    }
}
</style>

# HUD ROSLAN
**Infrastructure & Automation Engineer | AWS & CEH Certified**
Kuala Lumpur, Malaysia | +601121917499 | hudroslan@gmail.com
[GitHub](https://github.com/Hudroslancs) | [LinkedIn](https://www.linkedin.com/in/hudroslan/) | [Portfolio](https://hudroslan.com)

## PROFESSIONAL SUMMARY
Infrastructure professional with 5 years of experience managing mission-critical systems in healthcare and engineering environments. Specialized in automation, security implementation, and self-hosted infrastructure. Proven track record deploying production applications and maintaining 99%+ uptime for critical services. AWS Certified Cloud Practitioner and Certified Ethical Hacker.

## TECHNICAL SKILLS
- **Infrastructure & Virtualization:** Proxmox VE, AWS (EC2, S3, IAM, Lambda), Linux (Ubuntu, Debian), Docker, Dualboot: Fedora Atomic Silverblue, Windows 11 Pro
- **Automation & Development:** Python (Flask, APIs), n8n Workflows, Bash Scripting, Git/GitHub, CI/CD Pipelines
- **Security & Networking:** Cloudflare Zero Trust, Tailscale, Authentik SSO, DICOM/PACS, VLANs, Firewall Configuration
- **Specialized Expertise:** Medical Imaging Infrastructure (PACS/DICOM), AI Integration (Ollama/LLM), Document Processing

## KEY PROJECTS

### AI-Powered Resume Automation System | [GitHub](https://github.com/hudroslan/resume-automation)
<p class="sub-info">Self-Hosted Production System | 2024-Present</p>

- Architected end-to-end automation pipeline processing job descriptions and generating tailored resumes using AI
- **Technology Stack:** n8n (orchestration), Ollama/Llama3 (AI), Gotenberg (PDF generation), Telegram Bot API, Cloudflare Zero Trust
- **Infrastructure:** Self-hosted on Proxmox with custom domain (hudroslan.com), SSL certificates, and Zero Trust security
- **Code Quality:** Modular n8n workflows with error handling, logging, and rollback capabilities
- **Impact:** Reduced resume customization from 2 hours to 2 minutes; processed 20+ applications successfully
- **Open Source:** Workflow templates and documentation available on GitHub

### Production Homelab Infrastructure | [Documentation](https://github.com/hudroslan/homelab)
<p class="sub-info">5-Node Production Environment | 2023-Present</p>

- Designed and maintain production-grade homelab serving 10+ users across multiple devices
- **Architecture:** Proxmox hypervisor, 5 VM nodes with custom IP scheme (192.168.100.x), Tailscale mesh network
- **Services Deployed:** Nextcloud (1TB+ storage, 3 users), n8n (automation), Ollama (AI inference), Authentik (SSO), Bitwarden (password vault)
- **Security Implementation:** Enterprise SSO (Authentik) with LDAP integration, Zero Trust networking (Tailscale + Cloudflare), automated backups
- **Monitoring:** Uptime tracking, resource monitoring, automated alerting for service failures
- **Uptime:** 99.2% average uptime over 6 months with documented incident response procedures

### Digital Jobsheet Automation | [Demo](https://github.com/hudroslan/jobsheet-app)
<p class="sub-info">Python Flask Production Application | 2023-Present</p>

- Developed and deployed full-stack web application replacing paper-based engineering workflows
- **Backend:** Python Flask with RESTful API, SQLite database, automated data validation
- **Frontend:** Precision HTML/CSS with millimeter-based rendering for consistent A4/PDF output
- **Security:** Tailscale Zero Trust networking for secure remote access without public exposure
- **Deployment:** Production environment on Linux VM with systemd service management
- **Impact:** 100% digital workflow adoption, eliminated data entry errors, enabled real-time remote access for field technicians
- **Code:** Clean, documented Python with unit tests and error handling

<div style="page-break-before: always;"></div>

## PROFESSIONAL EXPERIENCE

### Healthcare IT Infrastructure Specialist | Amedix Sdn Bhd
<p class="sub-info">Kuala Lumpur, Malaysia | March 2020 - Present</p>

- Manage production PACS/DICOM medical imaging infrastructure serving multiple hospitals and clinics
- Deploy and maintain imaging systems (X-ray machines, workstations, PACS servers) across 10+ sites
- Configure Linux-based medical imaging systems including network settings, service dependencies, and data transfer protocols
- Implement and maintain backup strategies ensuring 99%+ uptime and zero data loss for critical medical imaging data
- Provide on-call support for production incidents with documented resolution times and root cause analysis
- Collaborate with clinical staff and IT teams on system requirements, regulatory compliance, and workflow optimization
- **Technologies:** Linux (Ubuntu/Debian), DICOM Protocol, Java, Network Administration, VMware

### Product Designer | Luxbee Sdn Bhd
<p class="sub-info">Kuala Lumpur, Malaysia | 2019 - 2020</p>

- Prepared technical CAD drawings (3D models, shop drawings, as-built documentation) for manufacturing projects
- Designed factory storage solutions optimizing space utilization and operational efficiency
- Collaborated with engineering and production teams on design specifications and manufacturing feasibility

### Structural Design Engineer | Galaxy Aerospace Malaysia
<p class="sub-info">Subang, Malaysia | 2017</p>

- Supported CAMO activities including technical records management and airworthiness compliance (AD/SB)
- Contributed to design and fabrication of specialized maintenance tools for Airbus and Agusta Westland helicopters
- Participated in modification engineering for Bambi Bucket system on AW139 aircraft

## CERTIFICATIONS
- **AWS Certified Cloud Practitioner** | Amazon Web Services | Valid through 2026
- **Certified Ethical Hacker (CEH)** | EC-Council | Credential ID: ECC8247441923

## EDUCATION
- **Bachelor of Engineering Technology (Industrial Design)** | Universiti Kuala Lumpur (UniKL) | 2013-2017
- **Foundation in Law** | UiTM Kuantan Faculty of Law | 2011
- **SPM** | SMT Muadzam Shah Civil Engineering | 2009