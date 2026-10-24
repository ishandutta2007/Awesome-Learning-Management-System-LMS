# Awesome-Learning-Management-System-LMS

## Top Learning Management System (LMS) Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Self-Hosted Course Delivery, SCORM/LTI Compliance & Scalable Learner Analytics*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Learning Management Systems (LMS)**. These tools help educational institutions, training departments, and organizations deliver courses, track learner progress, assess competencies, and manage compliance training — with a spectrum running from polished commercial suites to self-hosted platforms that handle everything from small classrooms to massive open online courses.

**Examples** include Moodle, Open edX, Chamilo, ILIAS, Canvas LMS, and Kolibri (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, SCORM/LTI interoperability, and scalable learner analytics — especially relevant as **Moodle powers 300+ million users across 240+ countries** [citation:3][citation:14], and **Open edX runs edX.org itself** with proven MOOC-scale infrastructure [citation:3][citation:8].

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **Adobe Captivate Prime** — Enterprise LMS with AI-powered recommendations, mobile learning, and deep integration with Adobe's eLearning authoring tools. **Subscription-based** per-learner pricing. **Best for enterprises** already using Adobe Captivate for content creation, accepting per-user costs and cloud dependency.

- **Docebo** — AI-driven enterprise LMS with social learning, gamification, and extended enterprise (multi-tenant) capabilities. **Subscription-based** with custom enterprise pricing. **Best for large organizations** needing a polished, feature-rich platform with strong multi-tenant support.

- **Cornerstone OnDemand** — Comprehensive talent and learning suite with compliance tracking, performance management, and recruiting integration. **Enterprise subscription pricing**. **Best for large enterprises** wanting learning tightly coupled with HR and talent management.

- **TalentLMS** — Accessible cloud LMS with a clean interface, mobile app, and built-in course authoring. **Subscription-based** with a free tier for up to 5 users. **Best for small to mid-size organizations** wanting a simple, well-designed cloud LMS without self-hosting overhead.

- **Canvas LMS Cloud** — Instructure's commercial cloud offering. **The open-source version (canvas-lms) provides the same core features** — assignments, SpeedGrader, discussions, and quizzes — but the cloud version adds Data Access Platform (DAP) analytics, premium support, and enterprise SLAs [citation:4][citation:9]. **Best for institutions** wanting Canvas's polished UX and analytics without operating the Ruby on Rails stack themselves [citation:14].

## Open-Source GitHub Projects

- **Moodle** — **The world's most widely deployed open-source LMS.** GPL-3.0 licensed, **300+ million users across 240+ countries** [citation:3][citation:14]. **The most feature-complete open-source LMS**: courses, 40+ quiz question types, assignments with rubrics, forums, wikis, SCORM 1.2/2004 packages, competency frameworks, badges, and granular role/permission systems [citation:3]. **Plugin ecosystem**: **2,000+ extensions** covering plagiarism detection, virtual labs, e-commerce, and more [citation:3][citation:8]. **LTI 1.1/1.3/Advantage compliant** for integration with commercial content and tools [citation:8]. **Deployment**: Bitnami Docker image makes it straightforward — **one application container plus MariaDB**, ready in ~3 minutes, running on **2 GB RAM minimum (4 GB recommended)** [citation:8][citation:14]. **The honest caveats**: **admin interface is complex** with hundreds of settings, **default theme looks dated** (modern themes exist), and **resource usage grows with concurrent users** [citation:3]. **Best for educational institutions, corporate training departments, and anyone needing a feature-complete LMS** on modest hardware with the largest plugin ecosystem available.

- **Open edX** — **The MOOC platform built by MIT and Harvard.** AGPL-3.0 licensed, **powers edX.org** with proven massive-scale infrastructure [citation:3][citation:8]. **Excels at massive open online courses**: video-based learning paths, discussion forums, auto-graded programming exercises via XBlocks, built-in certificate generation, and learning analytics [citation:3][citation:8]. **Deployment via Tutor**: `pip install "tutor[full]"` then `tutor local launch` — deploys **7+ containers** (LMS, CMS, MySQL, MongoDB, Redis, Meilisearch, Caddy) [citation:8]. **The honest caveats**: **resource-heavy (8 GB RAM minimum, 16 GB recommended)**, **steeper learning curve for course creators**, and **overkill for small teams** [citation:3][citation:8]. **Best for organizations delivering MOOCs**, universities with large enrollments, or companies creating self-paced training at scale — the only open-source LMS proven at edX.org's level [citation:3][citation:10].

- **Chamilo** — **The lightweight LMS for small teams and international projects.** GPLv3 licensed, **officially recognized as a Digital Public Good** by the Digital Public Goods Alliance (UN-supported initiative) [citation:11]. **Chamilo 2.0** (May 2026) is a major release with **completely redesigned interface** built on Vue 3 and PrimeVue, **AI-powered tools** for generating exercises and learning paths, **REST API with JWT authentication**, **LTI 1.3**, **cloud storage support** (Azure Blob, AWS S3, Google Cloud Storage), and **OnlyOffice integration** for collaborative document editing [citation:6]. **Distinctive features**: **80+ language interface**, **"jargon" system** to rename platform terms to your organization's vocabulary, **training session management** (same course delivered to multiple groups on different schedules), **competency management with Open Badges**, and **lower resource requirements (2 GB RAM workable)** [citation:3][citation:11]. **The honest caveats**: **smaller plugin ecosystem than Moodle**, **SCORM support less robust**, and **fewer integrations with commercial tools** [citation:3]. **Best for small schools, training companies, and international projects** wanting a modern, lightweight LMS with strong multilingual and data-sovereignty features [citation:11].

- **ILIAS** — **The German-engineered LMS for compliance training.** Open-source, with **particularly strong assessment and competency tracking features** [citation:3]. **Widely used in corporate compliance training and government education in Europe** [citation:3]. **Best for regulated industries and government agencies** needing rigorous assessment engines, SCORM 2004 support, and detailed competency tracking — especially in European contexts where ILIAS has strong adoption.

- **Canvas LMS (Open Source)** — **The open-source version of Instructure's Canvas.** AGPL-3.0 licensed, providing **the same core features as the cloud version** — assignments, SpeedGrader, discussions, and quizzes [citation:14]. **Modern, polished UI that students actually like**, with **SpeedGrader and rubrics widely considered superior to Moodle's grading tools** [citation:3][citation:14]. **The honest caveats**: **resource-heavy (8 GB RAM minimum, ~2 GB RAM active with 50 users)**, **requires PostgreSQL, Redis, and a background job processor**, and **the free version lacks premium features** like new quizzes, Canvas Commons, and Data Access Platform analytics [citation:4][citation:14]. **Best for institutions** wanting Canvas's modern UX and are willing to operate the Ruby on Rails stack themselves — or those evaluating whether the cloud version's premium features justify the cost [citation:4][citation:9].

- **Kolibri** — **The offline-first LMS for low-connectivity environments.** Open-source, designed for **offline/low-bandwidth education** with minimal server requirements [citation:3]. **Best for schools and NGOs** operating in areas with unreliable internet — it is the only major open-source LMS built specifically for offline-first deployment [citation:3].

### Additional Strong Open-Source Options

- **Sakai** — Long-standing open-source LMS used in higher education, with a focus on collaboration and research. Mentioned in academic comparisons alongside Moodle, Open edX, and Canvas [citation:1]. Best for universities with existing Sakai deployments.
- **Dokeos** — Lightweight LMS suitable for smaller institutions due to simplicity and lightweight structure, mentioned alongside Chamilo in academic comparisons [citation:1]. Best for small organizations wanting minimal overhead.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- LMS platforms differ significantly in target scale (small teams vs MOOCs), resource requirements (2 GB vs 16 GB RAM), and feature emphasis (traditional course management vs video-first MOOCs vs compliance training). **Moodle is the best overall choice for most self-hosters** with 2,000+ plugins and 300+ million users, running on 2 GB RAM [citation:3][citation:14]. **Open edX is the MOOC specialist** with proven edX.org scale, but requires 8 GB+ RAM and a steeper learning curve [citation:8][citation:10]. **Chamilo is the lightweight international option** with 2.0's modern Vue 3 interface, 80+ languages, and Digital Public Good recognition, but has a smaller plugin ecosystem [citation:3][citation:11]. **Canvas LMS has the best UI but demands 8 GB+ RAM** and lacks premium features in the open-source version [citation:4][citation:14]. **ILIAS is for compliance-heavy European contexts** [citation:3]. **The choice often comes down to scale and resources**: Moodle for most, Open edX for MOOCs, Chamilo for small/international teams, Canvas for UX-focused institutions with hardware budget, and Kolibri for offline environments.
- Self-hosted open-source solutions require proper server provisioning (2 GB for Moodle, 8 GB+ for Open edX and Canvas), database configuration (MySQL/MariaDB for Moodle, MySQL+MongoDB for Open edX, PostgreSQL for Canvas), and awareness that "free" open-source still has infrastructure and maintenance costs.

---

**Made for educators, training administrators, and organizations choosing learning management systems that match their scale, budget, and self-hosting requirements.**
Let's make learning management systems more open, scalable, and learner-friendly.
