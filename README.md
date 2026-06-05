🛩️ NTX Aerial — Launching Soon
Overview
NTX Aerial is a North Texas–based aerial imaging and roof inspection service preparing for FAA Part 107–certified operations.
This project hosts the NTX Aerial landing page, built with HTML + CSS and deployed via Azure Static Web Apps CI/CD.
The site introduces the brand, mission, and upcoming service offerings while showcasing a clean, modern design optimized for clarity and reliability.

🌐 Live Site
Production URL: https://ntxaerial.com  
Hosting: Azure Static Web Apps (Central US region)
CI/CD: GitHub Actions workflow (azure-static-web-apps-victorious-ocean-0b31c1010.yml)

📁 Repository Structure
plaintext
NTX_Aerial_Site/
├── index.html
├── styles.css
├── background.jpg
├── ntx_aerial_logo.png
├── README.md
└── .github/
    └── workflows/
        └── azure-static-web-apps-victorious-ocean-0b31c1010.yml
✨ Features
Responsive HTML + CSS landing page

Custom NTX Aerial branding and logo

Azure Static Web Apps CI/CD pipeline for automated deployment

“Launching Soon” hero section with FAA Part 107 notice

Informational sections for upcoming services and contact details

Dynamic year rendering via JavaScript

⚙️ Deployment Workflow
The GitHub Actions workflow automates build and deployment to Azure:

yaml
on:
  push:
    branches: [main]
  pull_request:
    types: [opened, synchronize, reopened, closed]
    branches: [main]

jobs:
  build_and_deploy_job:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - name: Build And Deploy
        uses: Azure/static-web-apps-deploy@v1
        with:
          azure_static_web_apps_api_token: ${{ secrets.AZURE_STATIC_WEB_APPS_API_TOKEN_VICTORIOUS_OCEAN_0B31C1010 }}
          repo_token: ${{ secrets.GITHUB_TOKEN }}
          action: "upload"
          app_location: "/"
          output_location: "."
This ensures every push to main automatically updates the live site.

🧩 Local Development
To edit or preview locally:

bash
git clone https://github.com/mmlcj5-dev/NTX_Aerial_Site.git
cd NTX_Aerial_Site
code .
Open index.html in your browser or use VS Code’s Live Server extension.

🚀 Roadmap
Add booking/contact form integration

Include drone footage gallery and service portfolio

Expand to real estate and construction documentation

Implement analytics and SEO optimization

Add automated email notifications for inquiries

📬 Contact
Questions or collaboration inquiries:
📧 mark@ntxaerial.com

🏁 Credits
Developer: Mark (mmlcj5‑dev)
Hosting: Azure Static Web Apps
Domain: ntxaerial.com

🎓 Technical Learning Goals
This project is part of my ongoing effort to deepen my engineering skillset while building real, production‑ready solutions for my own business. NTX Aerial serves as a practical sandbox for learning, applying, and demonstrating modern cloud‑native development patterns.

Cloud & DevOps
Deploying static sites using Azure Static Web Apps

Implementing CI/CD pipelines with GitHub Actions

Managing secrets securely using GitHub Encrypted Secrets

Understanding Azure resource provisioning and lifecycle management

Web Development
Building responsive landing pages with HTML + CSS

Structuring clean, accessible front‑end code

Optimizing static assets for performance and branding

Preparing for future integrations (forms, galleries, booking systems)

Version Control & Collaboration
Using Git and GitHub for project organization

Maintaining clean commit history and branching discipline

Automating deployments through GitHub → Azure workflows

Business‑Driven Engineering
Creating a real-world web presence for a new service business

Designing customer‑facing content with clarity and professionalism

Planning for future expansion into drone imaging, inspections, and real estate media

Applying technical skills directly to entrepreneurial goals

🧠 Skills Demonstrated
This project highlights a blend of cloud engineering, DevOps automation, front‑end development, and real‑world business application. It serves as both a professional portfolio piece and a foundation for NTX Aerial’s online presence.

Cloud & DevOps Engineering
Deploying production workloads using Azure Static Web Apps

Implementing continuous deployment pipelines with GitHub Actions

Managing secure deployment tokens via GitHub Secrets

Understanding cloud hosting models for static vs. dynamic workloads

Automating build + deploy cycles triggered on main branch updates

Front‑End Development
Building responsive, mobile‑friendly layouts using HTML5 + CSS3

Designing clean, modern UI components (hero sections, pill badges, CTAs)

Structuring semantic markup for accessibility and SEO

Using lightweight JavaScript for dynamic content (e.g., auto‑year footer)

Version Control & GitHub Proficiency
Managing repositories, branches, and commit history

Integrating GitHub Actions workflows into real projects

Maintaining clean repo structure and deployment‑ready code

Using Git effectively for iterative development and updates

Branding & Business Integration
Creating a professional landing page for a real service business

Translating business goals into technical implementation

Establishing a digital presence with a custom domain (ntxaerial.com)

Preparing infrastructure for future booking, media, and customer workflows

Entrepreneurial Engineering
Applying cloud and automation skills to launch a real venture

Building a scalable foundation for drone imaging and inspection services

Combining technical learning with business execution and branding

© 2026 NTX Aerial — North Texas Aerial - Imaging & Inspection