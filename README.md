 <div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=200&color=0:0F172A,50:172554,100:2563EB&text=Nitish%20Konamarthi&fontSize=42&fontColor=FFFFFF&fontAlignY=38&desc=Backend%20Engineering%20%7C%20AI%20Infrastructure%20%7C%20Cloud&descAlignY=59&descSize=16" width="100%" alt="Nitish Konamarthi — Backend Engineering, AI Infrastructure and Cloud" />

# Konamarthi Nitish Veera Venkatesh

### Software Developer · Backend Engineering · AI Infrastructure · Cloud Computing

Building backend systems, intelligent applications and developer-focused infrastructure.

<p>
  <a href="https://www.linkedin.com/in/konamarthi-nitish-veera-venkatesh-4380282b6/">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="https://github.com/Nitish-Konamarthi">
    <img src="https://img.shields.io/badge/GitHub-Profile-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
  </a>
  <a href="https://www.npmjs.com/~konamarthi-nitish-veera-venkatesh">
    <img src="https://img.shields.io/badge/npm-Publisher-CB3837?style=for-the-badge&logo=npm&logoColor=white" alt="npm"/>
  </a>
  <a href="https://pypi.org/project/chest-xray-diagnosis/">
    <img src="https://img.shields.io/badge/PyPI-Published%20Package-3775A9?style=for-the-badge&logo=pypi&logoColor=white" alt="PyPI"/>
  </a>
</p>

</div>

---

## 👋 About Me

I am **Konamarthi Nitish Veera Venkatesh**, a Computer Science and Engineering graduate with a strong interest in backend engineering, AI infrastructure, cloud computing and distributed systems.

I enjoy building software beyond the application layer — understanding how systems communicate, how data flows through services, how APIs are secured, how infrastructure behaves under failure, and how engineering decisions affect reliability, performance and maintainability.

My work combines backend development, AI/ML applications, cloud deployment and practical system design.

I have independently built and maintained several technical projects, published software packages to both npm and PyPI, developed an AI-powered medical imaging application, and co-authored a research paper published in the International Journal of Innovative Research in Technology (IJIRT).

**What I am particularly interested in:**

- Backend engineering and scalable API architectures.
- AI infrastructure, LLM gateways and model-provider orchestration.
- Distributed systems, reliability and cloud-native engineering.
- Database design, caching, queues and data consistency.
- Developer tools, automation and engineering productivity.
- Practical applications of machine learning and explainable AI.

I believe good engineering is not just about making software work. It is about making systems understandable, testable, secure, maintainable and useful to other developers.

---

## 🚀 Featured Projects

### 01. TokenSentry — AI Infrastructure & LLM Gateway

**A self-hosted AI gateway for governing, routing and managing LLM requests.**

<a href="https://github.com/Nitish-Konamarthi/tokensentry-proto">
  <img src="https://img.shields.io/badge/Source%20Code-GitHub-181717?style=flat-square&logo=github" alt="Source code"/>
</a>
<a href="https://tokensentry-ai.vercel.app">
  <img src="https://img.shields.io/badge/Project%20Site-Live-2563EB?style=flat-square&logo=vercel&logoColor=white" alt="Project site"/>
</a>

TokenSentry is an infrastructure layer positioned between AI clients or coding tools and configured LLM providers. It aims to make model access more governable through centralized authentication, policy enforcement, routing, budgets and usage accounting.

**Core engineering work:**

- Built a Fastify and TypeScript API gateway.
- Implemented API-key authentication and request rate limiting.
- Developed organization-level budget controls and model policies.
- Implemented deterministic model routing and provider adapters.
- Built Agent Guard checks for gateway-visible agent/session signals.
- Integrated PostgreSQL for durable application data and Valkey for shared transient state and atomic controls.
- Implemented usage accounting, analytics and audit logging.
- Developed a Next.js administration dashboard and project website.

**Provider integrations:** OpenAI, Anthropic, Google Gemini, Groq and OpenRouter.

**Technology:** TypeScript, Node.js, Fastify, PostgreSQL, Drizzle ORM, Valkey, ioredis, Next.js, Docker and NGINX.

**Engineering documentation:**

- [Architecture and system design](https://github.com/Nitish-Konamarthi/tokensentry-proto/blob/main/docs/architecture.md)
- [API documentation](https://github.com/Nitish-Konamarthi/tokensentry-proto/blob/main/docs/API.md)
- [Deployment guide](https://github.com/Nitish-Konamarthi/tokensentry-proto/blob/main/docs/DEPLOYMENT.md)
- [Architecture decisions](https://github.com/Nitish-Konamarthi/tokensentry-proto/blob/main/docs/DECISIONS.md)
- [API OpenAPI specification](https://github.com/Nitish-Konamarthi/tokensentry-proto/blob/main/api/openapi.yaml)

The repository includes GitHub Actions workflows for package builds, type checking, automated tests and infrastructure configuration validation.

**Deployment:** A public project site is available on Vercel. The repository also documents a Vercel API prototype configuration and a Docker Compose deployment template. The documented free-tier configuration is intended for prototyping, not production workloads.

---

### 02. Chest X-Ray Diagnostic Assistant — Explainable Medical AI

**A multi-stage deep learning application for chest X-ray pathology analysis and visual explainability.**

<a href="https://github.com/Nitish-Konamarthi/Chest-X-Ray-Diagnostic-Assistant">
  <img src="https://img.shields.io/badge/Source%20Code-GitHub-181717?style=flat-square&logo=github" alt="Source code"/>
</a>
<a href="https://chest-x-ray-diagnostic-assistant.vercel.app">
  <img src="https://img.shields.io/badge/Application-Demo-2563EB?style=flat-square&logo=vercel&logoColor=white" alt="Application demo"/>
</a>
<a href="https://ijirt.org/publishedpaper/IJIRT198365_PAPER.pdf">
  <img src="https://img.shields.io/badge/Research-IJIRT%20Paper-8B5CF6?style=flat-square" alt="Research paper"/>
</a>

An AI-powered medical imaging application developed around a multi-stage inference pipeline, explainable predictions and an interactive web interface.

**Technical implementation:**

- Developed a three-stage image validation pipeline using MobileNetV2 and ResNet18 models.
- Implemented DenseNet-121 for multi-label classification of 14 thoracic pathologies using the NIH ChestX-ray14 dataset.
- Integrated Grad-CAM++ to generate visual explanations of model predictions.
- Integrated Google Gemini for generating natural-language explanations from structured model outputs.
- Developed a FastAPI backend and React frontend.
- Integrated Geoapify for location-based specialist discovery.
- Designed failure-handling paths for invalid images and unavailable inference resources.

**Reported research result:** The published paper reports an average AUROC of **0.8779** for the 14-pathology classification experiment.

**Technology:** Python, PyTorch, DenseNet-121, MobileNetV2, ResNet18, Grad-CAM++, FastAPI, React, Google Gemini and Geoapify.

The application is intended for research and educational purposes. Its predictions are not a substitute for professional medical diagnosis or clinical validation.

#### Published software packages

The project was also packaged and distributed through two software ecosystems.

**Python package — PyPI**

[![PyPI Version](https://img.shields.io/pypi/v/chest-xray-diagnosis?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/chest-xray-diagnosis/)
[![PyPI License](https://img.shields.io/pypi/l/chest-xray-diagnosis?style=flat-square)](https://pypi.org/project/chest-xray-diagnosis/)

- Package: `chest-xray-diagnosis`
- Distribution: PyPI
- Author: Nitish Konamarthi
- Licence: MIT
- [View PyPI package](https://pypi.org/project/chest-xray-diagnosis/)

```bash
pip install chest-xray-diagnosis
```

**Node.js package — npm**

[![npm Version](https://img.shields.io/npm/v/chest-xray-diagnosis?style=flat-square&logo=npm)](https://www.npmjs.com/package/chest-xray-diagnosis)
[![npm License](https://img.shields.io/npm/l/chest-xray-diagnosis?style=flat-square)](https://www.npmjs.com/package/chest-xray-diagnosis)

- Package: `chest-xray-diagnosis`
- Distribution: npm
- Published version: 1.0.1
- Licence: MIT
- Publisher: Konamarthi Nitish Veera Venkatesh
- [View npm package](https://www.npmjs.com/package/chest-xray-diagnosis)

```bash
npm install chest-xray-diagnosis
```

The npm package provides a Node.js launcher workflow designed to bootstrap the Python backend and launch its API server.

---

## 📄 Research & Publication

### Multi-Stage Deep Learning with Explainability for Chest X-Ray Pathology Detection using DenseNet-121

**Published in the International Journal of Innovative Research in Technology (IJIRT).**

<p>
  <a href="https://ijirt.org/publishedpaper/IJIRT198365_PAPER.pdf">
    <img src="https://img.shields.io/badge/Published%20Research-Read%20Full%20Paper-8B5CF6?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="Read paper"/>
  </a>
</p>

| Publication detail | Information |
|---|---|
| Journal | International Journal of Innovative Research in Technology |
| Publication | April 2026 |
| Volume | 12 |
| Issue | 11 |
| Paper ID | IJIRT 198365 |
| ISSN | 2349-6002 |
| Research area | Deep Learning, Medical Imaging, Explainable AI |

**Authors as listed in the publication:**

1. Mrs. T. Kranthi
2. K. Nitish V Venkatesh
3. Marrapu Tarun
4. Karanam Swapna Preethi
5. Gorli Praveena
6. Shaik Mohammed Marshuk

**Research contributions and technical areas:**

- Multi-stage validation for rejecting invalid and non-thoracic images.
- Transfer learning with MobileNetV2 and ResNet18.
- Multi-label thoracic pathology classification using DenseNet-121.
- Model explainability using Grad-CAM++.
- Integration of large language models for natural-language reporting.
- Full-stack implementation with FastAPI and React.

The paper uses the NIH ChestX-ray14 dataset and discusses the methodology, architecture, training process, evaluation and limitations.

[Read the published research paper (PDF)](https://ijirt.org/publishedpaper/IJIRT198365_PAPER.pdf)

---

### 03. Manager-ERP — Business & Supply Chain Management

**A full-stack ERP system designed around vegetable retail, wholesale and hotel supply-chain operations.**

[![Repository](https://img.shields.io/badge/Source%20Code-GitHub-181717?style=flat-square&logo=github)](https://github.com/Nitish-Konamarthi/Manager-ERP)

A practical ERP project focused on business workflows, transactional consistency and modular backend architecture.

**Implemented system areas:**

- Modular monolith architecture.
- Multi-tenant organizations, shops, warehouses and branches.
- Inventory management, stock batches and reservations.
- Sales, billing and procurement workflows.
- Supplier and customer management.
- Accounting, ledger and financial reporting.
- Role-based access control and granular permissions.
- Audit logging and concurrency management.
- Background job processing.

**Technology:** Node.js, NestJS, TypeScript, PostgreSQL, Prisma, Redis, BullMQ, React, Vite, Docker Compose and JWT.

The project also contains architectural documentation covering domain modelling, business workflows, concurrency, security and project structure.

[Explore the repository and technical documentation](https://github.com/Nitish-Konamarthi/Manager-ERP)

---

### 04. English Speaking Tutor — Local-First AI Application

**A privacy-focused, locally running AI-powered English practice application.**

[![Repository](https://img.shields.io/badge/Source%20Code-GitHub-181717?style=flat-square&logo=github)](https://github.com/Nitish-Konamarthi/EnglishSpeakingTutor)

Developed a Windows-based application combining local language-model inference, voice interaction and persistent conversational memory.

**Key implementation areas:**

- Local Qwen model inference through llama.cpp.
- Speech recognition using Whisper.
- Text-to-speech using Kokoro.
- Persistent conversations and session management.
- SQLite-backed conversation storage.
- Semantic retrieval using MiniLM embeddings and SQLite FTS5.
- Local-first processing with no cloud transmission of audio or transcripts by the application.

**Technology:** Python, llama.cpp, Qwen, Whisper, Kokoro, SQLite, sentence-transformers and JavaScript.

[Explore the repository](https://github.com/Nitish-Konamarthi/EnglishSpeakingTutor)

---

## 🛠️ Technical Skills

My technical interests and practical development experience span the following areas.

| Area | Technologies |
|---|---|
| Programming languages | TypeScript, JavaScript, Python, Java, SQL |
| Backend development | Node.js, Fastify, NestJS, FastAPI |
| Frontend development | React, Next.js, Vite |
| Databases | PostgreSQL, SQLite |
| Caching & messaging | Redis, Valkey, BullMQ |
| ORM & data access | Prisma, Drizzle ORM |
| AI & Machine Learning | PyTorch, DenseNet-121, Grad-CAM++, LLM integrations |
| Local AI inference | llama.cpp, Qwen, Whisper, Kokoro |
| Cloud platforms | AWS, Oracle Cloud Infrastructure |
| DevOps & infrastructure | Docker, Docker Compose, NGINX, GitHub Actions |
| Deployment | Vercel and cloud-hosted application prototypes |
| Engineering practices | REST APIs, RBAC, CI/CD, integration testing, API documentation, system design |

---

## ☁️ Cloud & Infrastructure Learning

I am particularly interested in understanding the infrastructure behind reliable software systems.

My learning and implementation interests include:

- Cloud architecture and infrastructure provisioning.
- Networking, VPCs, subnets and security boundaries.
- Containerization and deployment automation.
- CI/CD workflows and infrastructure validation.
- Database reliability, caching and state management.
- Distributed systems and fault handling.
- Observability, security and operational practices.

I have completed the following Oracle Cloud Infrastructure learning certifications:

- OCI Foundations Associate.
- OCI AI Foundations.

I continue to develop practical experience with AWS and cloud-native engineering concepts.

---

## 🧠 How I Approach Engineering

A few principles guide how I build software:

**Architecture before complexity**

I try to establish clear service boundaries, data ownership, API contracts and system responsibilities before adding more components.

**Testing and reproducibility**

A project should include a documented setup process, repeatable checks and tests that help other developers understand its behaviour.

**Security and reliability**

Authentication, secrets handling, validation, failure handling and data consistency should be part of the design rather than afterthoughts.

**Honest technical documentation**

I believe documentation should distinguish implemented functionality, prototypes, measured results and planned features.

**Building for other developers**

Developer tooling should have understandable interfaces, clear documentation, sensible defaults and a manageable contribution process.

---

## 🤝 Collaboration & Opportunities

I am interested in opportunities and collaborations involving:

- Backend Software Engineering.
- Cloud and Platform Engineering.
- AI Infrastructure and Developer Tooling.
- API platforms and distributed systems.
- Applied AI and intelligent software systems.

I enjoy working on technically challenging problems, learning from experienced engineers and contributing to products where reliability, architecture and engineering quality matter.

I also welcome constructive feedback, bug reports, technical discussions and contributions to my public projects.

---

## 📬 Connect With Me

<p align="center">
  <a href="https://github.com/Nitish-Konamarthi">
    <img src="https://img.shields.io/badge/GitHub-Nitish--Konamarthi-181717?style=for-the-badge&logo=github" alt="GitHub"/>
  </a>
  <a href="https://www.linkedin.com/in/konamarthi-nitish-veera-venkatesh-4380282b6/">
    <img src="https://img.shields.io/badge/LinkedIn-Nitish%20Konamarthi-0A66C2?style=for-the-badge&logo=linkedin" alt="LinkedIn"/>
  </a>
  <a href="https://www.npmjs.com/~konamarthi-nitish-veera-venkatesh">
    <img src="https://img.shields.io/badge/npm-Publisher-CB3837?style=for-the-badge&logo=npm" alt="npm"/>
  </a>
  <a href="https://pypi.org/project/chest-xray-diagnosis/">
    <img src="https://img.shields.io/badge/PyPI-Publisher-3775A9?style=for-the-badge&logo=pypi" alt="PyPI"/>
  </a>
</p>

<p align="center">
  <i>Building thoughtfully. Learning continuously. Engineering with purpose.</i>
</p>

<p align="center">
  <sub>Thank you for visiting my profile.</sub>
</p>
