<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header.svg" />
  <source media="(prefers-color-scheme: light)" srcset="assets/header-light.svg" />
  <img src="assets/header.svg" width="100%" alt="Zeeshan Zafar — Full Stack and Mobile Software Engineer" />
</picture>

### I turn complex ideas into dependable software.

Thoughtful interfaces. Maintainable backends. Mobile experiences built with care.

[![Portfolio](https://img.shields.io/badge/Portfolio-6D28D9?style=for-the-badge&logo=vercel&logoColor=white)](https://zeeshan-zafar.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-6D28D9?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/zeeshi-ch/)
[![Email](https://img.shields.io/badge/Email-6D28D9?style=for-the-badge&logo=gmail&logoColor=white)](mailto:Zeeshich019@gmail.com)
[![Book a call](https://img.shields.io/badge/Book_a_call-6D28D9?style=for-the-badge&logo=calendly&logoColor=white)](https://calendly.com/zeeshich019/30min)

![Experience](https://img.shields.io/badge/Experience-4%2B_years-A78BFA?style=flat-square&labelColor=24212B)
![Projects](https://img.shields.io/badge/Projects_contributed_to-50%2B-A78BFA?style=flat-square&labelColor=24212B)
![Location](https://img.shields.io/badge/Based_in-Lahore%2C_Pakistan-A78BFA?style=flat-square&labelColor=24212B)

[Projects](#selected-work) · [Engineering](#how-i-build) · [Stack](#tech-stack) · [Experience](#experience) · [Contact](#lets-connect)

</div>

---

## About me

**Curious by nature. Engineer by craft.**

I’m a **Full Stack & Mobile Software Engineer** based in Lahore, Pakistan, building software professionally since **2022**.

My work connects product thinking with maintainable architecture—from API and database design to web interfaces and mobile releases.

- **Web:** React, Next.js, TypeScript, and reusable interfaces.
- **Backend:** Node.js, NestJS, Hono, API design, and database workflows.
- **Mobile:** React Native, Expo, Kotlin, and Jetpack Compose.
- **Product experience:** Enterprise platforms, healthcare, AI voice applications, fintech, and education.

I’ve contributed to **50+ projects**, ranging from individual features to complete products. Some work remains private under NDAs; the projects below represent work I can share publicly.

---

## Selected work

### Hexa AI
**Real-time voice AI · Full-stack development**

[![Hexa AI overview](assets/hexa-ai.svg)](https://zeeshan-zafar.vercel.app/projects/hexa-ai)

A multi-tenant platform for configuring AI voice agents, conversation flows, and calling workflows.

**My work**
- Built visual conversation-flow interfaces and backend integrations.
- Designed real-time voice orchestration connecting telephony, speech recognition, AI models, and speech synthesis.
- Connected company-scoped calling workflows and administrative access.

**Stack:** Next.js · NestJS · React Flow · PostgreSQL · Twilio · OpenAI · ElevenLabs

[Engineering case study ↗](https://zeeshan-zafar.vercel.app/projects/hexa-ai) · [Live product ↗](https://gethexa.ai/)

---

### Case Management Hub
**Enterprise workflows · Full-stack development**

[![Case Management Hub overview](assets/case-management.svg)](https://zeeshan-zafar.vercel.app/projects/case-management)

A platform connecting client records, configurable forms, scheduling, reporting, and service operations.

**My work**
- Built configurable drag-and-drop forms.
- Connected submissions to client-profile updates using three identification paths.
- Handled permissions across patient, provider, and public form submissions.
- Supported autofill from existing client-profile data.

**Stack:** Next.js · TypeScript · NestJS · PostgreSQL

[Engineering case study ↗](https://zeeshan-zafar.vercel.app/projects/case-management) · [Product website ↗](https://casemanagementhub.org/) · [Portal ↗](https://app.casemanagementhub.org/)

---

### StarKidz
**Published mobile learning app · Formerly Nedjmati**

[![StarKidz overview](assets/nedjmati.svg)](https://zeeshan-zafar.vercel.app/projects/nedjmati)

![Google Play downloads](https://img.shields.io/badge/Google_Play-50K%2B_downloads-A78BFA?style=flat-square&labelColor=24212B)

A learning application with dynamic subjects, units, lessons, questions, and multilingual experiences.

**My work**
- Built mobile interfaces driven by backend learning content.
- Developed and maintained data-seeding scripts for source material supplied in different formats.
- Handled content-version updates and language changes throughout the app.
- Connected learning sessions, audio, and progress tracking.

**Stack:** React Native · Expo · TypeScript · Firebase · PostgreSQL

[Engineering case study ↗](https://zeeshan-zafar.vercel.app/projects/nedjmati) · [Google Play ↗](https://play.google.com/store/apps/details?id=com.nedjmati.nedjmatiapp)

<sub>Download count describes the app’s public reach, rather than a measured result attributable to one engineering change.</sub>

<details>
<summary><strong>More projects</strong></summary>

<br />

| Project | Focus | Core technologies |
|---|---|---|
| **[Homewellness](https://zeeshan-zafar.vercel.app/projects/homewellness)** | Healthcare marketplace with service requests, quotations, appointments, and provider workflows | Next.js, Hono, Bun, Drizzle ORM, PostgreSQL |
| **[Degn](https://degn.app/)** | Native Android fintech application with market charts, payment integrations, and secure authentication | Kotlin, Jetpack Compose, Firebase |
| **[GOAT App](https://apps.apple.com/us/app/goat-app/id1597319742)** | Reservation workflows, synchronized availability, Firebase query improvements, and React Native upgrades | React Native, Firebase, JavaScript |

[Explore all projects ↗](https://zeeshan-zafar.vercel.app/projects)

</details>

---

## How I build

I care about how a product works—and how it feels to use.

One example is **Case Management Hub’s form system**. The challenge extended beyond drag-and-drop editing: submissions needed to identify the correct client, respect permissions, prefill existing information, and update the appropriate profile data.

```mermaid
flowchart TD
    Editor["Drag-and-drop form builder"] --> Definition["Saved form definition"]
    Definition --> Patient["Patient portal"]
    Definition --> Provider["Provider portal"]
    Definition --> Public["Public form — no login"]
    Patient --> Rules["Apply submission permissions"]
    Provider --> Rules
    Public --> Rules
    Rules --> Identify["Resolve client using the relevant identifier"]
    Identify --> Profile["Load permitted profile data"]
    Profile --> Form["Render form with available autofill"]
    Form --> Submit["Validate submitted values"]
    Submit --> Update["Update permitted client fields"]
    classDef accent fill:#6D28D9,color:#FFFFFF,stroke:#A78BFA;
    class Editor,Rules,Identify,Update accent;
```

**My approach**
- Understand the workflow before choosing the implementation.
- Keep interfaces, API contracts, and data models aligned.
- Make permission boundaries explicit.
- Build reusable components where they simplify the product.
- Validate important paths and keep the code understandable as it grows.

---

## Tech stack

| Area | Technologies |
|---|---|
| **Web** | React · Next.js · TypeScript · Tailwind CSS |
| **Mobile** | React Native · Expo · Kotlin · Jetpack Compose · Android · iOS |
| **Backend** | Node.js · NestJS · Express · Hono · Bun · FastAPI |
| **Data** | PostgreSQL · MySQL · MongoDB · Firebase · Supabase · SQL Server |
| **ORMs** | Prisma · Drizzle ORM |
| **Tools** | Git · Docker · Bash · Kafka |
| **Integrations** | OpenAI · ElevenLabs · Twilio · Stripe · Firebase Cloud Messaging · MoonPay · TransFi |

<details>
<summary><strong>Additional languages</strong></summary>

JavaScript · Java · Python · C++ · C · PHP · HTML · CSS

</details>

---

## Experience

| Role | Company | Period |
|---|---|---|
| **Software Engineer / Full-Stack Developer** | Verdant Soft · Lahore | Jan 2026 – Present |
| **Software Engineer** | TheDesignerX · Lahore | Jul 2022 – Dec 2025 |

<details>
<summary><strong>What I worked on</strong></summary>

<br />

**Verdant Soft**
- Full-stack web applications and backend services.
- AI calling platforms, healthcare workflows, and mobile learning products.
- Reusable interfaces, third-party integrations, and connected data workflows.

**TheDesignerX**
- Enterprise workflow applications.
- Native Android applications for industrial operations.
- React Native applications for eCommerce and fundraising.
- Node.js and Firebase serverless integrations.

</details>

**Education:** BS Computer Science · COMSATS University Islamabad, Lahore Campus

---

## GitHub activity

My contributions are spread across **[ZeeshiCh](https://github.com/ZeeshiCh)** and my professional account, **[zeeshanzafarvs](https://github.com/zeeshanzafarvs)**. Public repository activity represents only part of my engineering work.

<details>
<summary><strong>View public GitHub statistics</strong></summary>

<br />

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=ZeeshiCh&amp;show_icons=true&amp;hide_border=true&amp;bg_color=191923&amp;title_color=A78BFA&amp;icon_color=A78BFA&amp;text_color=F5F3FF" />
  <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats.vercel.app/api?username=ZeeshiCh&amp;show_icons=true&amp;hide_border=true&amp;bg_color=F7F5F0&amp;title_color=6D28D9&amp;icon_color=6D28D9&amp;text_color=24212B" />
  <img src="https://github-readme-stats.vercel.app/api?username=ZeeshiCh&amp;show_icons=true&amp;hide_border=true&amp;bg_color=191923&amp;title_color=A78BFA&amp;icon_color=A78BFA&amp;text_color=F5F3FF" alt="ZeeshiCh public GitHub statistics" />
</picture>

</details>

<details>
<summary><strong>Contribution animation</strong></summary>

<br />

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ZeeshiCh/ZeeshiCh/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ZeeshiCh/ZeeshiCh/output/github-snake.svg" />
  <img src="https://raw.githubusercontent.com/ZeeshiCh/ZeeshiCh/output/github-snake.svg" width="100%" alt="Animated contribution snake" />
</picture>

</details>

---

<a id="lets-connect"></a>

## Let’s connect

Have a web, backend, or mobile product to build—or an engineering role to discuss?

**[Explore my portfolio ↗](https://zeeshan-zafar.vercel.app/)** · **[Download résumé ↓](https://zeeshan-zafar.vercel.app/assets/zeeshan-zafar-cv.pdf)** · **[Book a 30-minute call ↗](https://calendly.com/zeeshich019/30min)**

[LinkedIn](https://www.linkedin.com/in/zeeshi-ch/) · [Zeeshich019@gmail.com](mailto:Zeeshich019@gmail.com) · [+92 333 606 0197](tel:+923336060197)

<sub>Built with intention. From Lahore, Pakistan.</sub>
