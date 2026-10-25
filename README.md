# Hassani Calligraphy — إبراهيم حسني إدريسي (الخط العربي المغربي)

<div align="center">

**Interactive Digital Showcase, Virtual Academy & Distance Cohorts for Moroccan Arabic Calligraphy (`hassanicalligraphy.com`)**

[![Live Website](https://img.shields.io/badge/Live%20Platform-hassanicalligraphy.com-10b981?style=for-the-badge&logo=google-chrome&logoColor=white)](https://hassanicalligraphy.com/)
[![React / Vite](https://img.shields.io/badge/Frontend-React%20%7C%20Vite%20%7C%20Tailwind-61dafb?style=for-the-badge&logo=react&logoColor=black)](https://vitejs.dev)
[![Replit SSH](https://img.shields.io/badge/Cloud%20IDE-Replit%20SSH%20%2B%20Claude%20%26%20Antigravity-F26207?style=for-the-badge&logo=replit&logoColor=white)](https://hassanicalligraphy.com/)
[![Typography](https://img.shields.io/badge/Typography-Traditional%20Maghrebi%20RTL-orange?style=for-the-badge)](https://hassanicalligraphy.com/)

[**🌐 Live Production Platform (hassanicalligraphy.com)**](https://hassanicalligraphy.com/)

</div>

---

## 📌 Executive Summary

**Hassani Calligraphy** ([`hassanicalligraphy.com`](https://hassanicalligraphy.com/)) is a production digital cultural platform and distance-learning academy built for master calligrapher, manuscript researcher, and teacher **Ibrahim Hassani Idrissi** (Fes, Morocco — recipient of the Mohammed VI Incentive Award for Moroccan Calligraphic Art, 2025, and graduate of Al-Qarawiyyin Mosque calligraphy program).

The platform serves two primary goals:
1. **Interactive Cultural Showcase**: High-resolution gallery, atelier tour (`المرسم`), and curated codicological context celebrating authentic Moroccan and Andalusi calligraphy styles (المبسوط، المجوهر، الثلث المغربي، والخط الأندلسي), alongside a cross-link to the companion manuscript encyclopedia [`masahif-al-maghrib.com`](https://masahif-al-maghrib.com).
2. **Virtual Masterclass & Cohort Enrollment**: A multilingual (`AR` / `EN` / `FR`) enrollment and onboarding funnel for small, intensive distance-learning cohorts (10 to 15 students per track, 3-month levels), featuring weekly live instructional sessions, structured homework critique schedules, and direct master feedback via WhatsApp.

---

## 🛠️ Cloud-to-Workstation Engineering Workflow (Replit SSH + Claude & Antigravity)

This client project is engineered and maintained using a **hybrid cloud-container + local Linux workstation architecture**:

- **Remote Replit Development Container over SSH**: The full-stack source workspace runs inside a dedicated Replit container connected directly to the local Linux workstation via SSH (`*.replit.dev:22`).
- **Multi-Agent Orchestration (Claude Code & Google Antigravity)**: Rather than relying on browser-based cloud editors, development, multilingual RTL layout refinement (`AR` / `EN` / `FR`), lazy-loaded section splitting, and performance tuning are steered directly from the Linux workstation over SSH using **Claude Code** and **Google Antigravity** (and mobile-steered via [`workstation-discord-bridge`](https://github.com/kmbenjel/workstation-discord-bridge)).
- **Production Bundle & Showcase Repository**: This repository (`kmbenjel/hassanicalligraphy.com`) houses the compiled Vite + React + Tailwind production assets (`public/assets/`, `public/images/`), architecture documentation, and visual showcase of the live platform at [`hassanicalligraphy.com`](https://hassanicalligraphy.com/).

---

## 🏗️ System Architecture & Component Interaction

```mermaid
flowchart TB
    subgraph ClientLayer ["🌐 Client Experience (Mobile / Desktop)"]
        Landing["Modern RTL Landing Page\n(Hero, Bio, Cohort Details, Pricing)"]
        Gallery["Interactive High-Res Artwork Showcase\n(Deep Zoom, Script Classification)"]
        EnrollmentModal["Cohort Enrollment & Onboarding Modal\n(Tier Selection, WhatsApp Integration)"]
        AudioPreview["Scribal & Calligraphic Audio Context\n(Ambient Tradition Experience)"]
    end

    subgraph AppCore ["⚡ Frontend Core (React + Tailwind + Vite)"]
        StateEngine["State Management\n(Cohort Slots, Active Gallery Filter, Bidi Engine)"]
        AnalyticsConsent["Privacy-First Analytics Layer\n(Cookieless GA4 & Privacy Consent)"]
        RTLDesignSystem["RTL Design System\n- Tajawal & Cairo Typography\n- CSS Logical Properties\n- Fluid Dark / Gold Luxury Aesthetics"]
    end

    subgraph Infrastructure ["☁️ Cloud & Edge Delivery"]
        CDN["Google Frontend / CDN Edge\n(Sub-second TTFB, HTTP/3, Brotli)"]
        AssetStorage["Optimized Visual Assets & WebP Plates"]
        DirectBridge["Direct Master Mentorship Channel\n(WhatsApp Business API Gateway)"]
    end

    Landing --> StateEngine
    Gallery --> StateEngine
    EnrollmentModal --> DirectBridge
    AudioPreview --> AssetStorage
    
    StateEngine --> RTLDesignSystem
    StateEngine --> AnalyticsConsent
    
    RTLDesignSystem --> CDN
    AssetStorage --> CDN
```

---

## 🔄 Sequence Diagram: Student Onboarding & Cohort Journey

```mermaid
sequenceDiagram
    autonumber
    actor S as 👨‍🎓 Prospective Student
    participant W as 🌐 Platform (hassanicalligraphy.com)
    participant C as 📝 Cohort State Engine
    participant WA as 💬 WhatsApp Master Channel
    participant M as ✒️ Master Ibrahim Hassani

    S->>W: Lands on site (Discovers curriculum & calligraphy samples)
    S->>W: Explores gallery (Mabsut, Mujawhar, Thuluth Maghrebi plates)
    S->>W: Reviews live cohort schedule (Monday live class + Sunday critique)
    S->>C: Clicks 'سجّل في الفوج القادم' (Register for upcoming cohort)
    C->>C: Validates remaining seat capacity (Limited 10-15 students)
    C->>WA: Pre-populates structured registration message
    WA->>M: Direct transmission of student inquiry & background
    M-->>S: Confirms enrollment, delivers course materials & private class link
```

---

## ✒️ Typographic Styles Preserved

The digital gallery highlights the nuanced distinctions between classical Maghrebi calligraphic schools:

| Style (الأسلوب) | Codicological Role | Visual Characteristics |
|---|---|---|
| **الخط المبسوط (Al-Mabsut)** | Principal script for Qur'anic manuscripts and sacred texts | Rounded curves, deep open bowls (*nun*, *sad*), balanced proportions, and clear legibility. |
| **الخط المجوهر (Al-Mujawhar)** | Royal correspondence, legal edicts, and scholarly treaties | Fluid, ligature-rich, rapid cursive flow with tight vertical rhythm. |
| **الثلث المغربي (Maghrebi Thuluth)** | Monumental architectural inscriptions, illuminated headings | Towering ascenders, sharp architectural angles, and decorative majesty. |
| **الكوفي المربع (Square Kufic)** | Geometric architectural medallions and tilework (Zellij) | Strict orthogonal grid, binary ink/negative balance, mathematical precision. |

---

## 📸 Live Production UI Showcase (`hassanicalligraphy.com`)

<div align="center">

| 🏛️ Trilingual (`AR` / `EN` / `FR`) Hero & Cohort Registration | ✒️ Interactive Artwork & Illuminated Manuscript Gallery (`معرض الأعمال`) |
|:---:|:---:|
| ![Desktop Hero and Cohort CTA](./public/images/showcase/desktop-hero-bio.png) <br> *Warm parchment-inspired RTL landing interface with language switcher (`ع` / `EN` / `FR`), upcoming cohort countdown, and direct WhatsApp enrollment.* | ![Interactive Artwork Gallery](./public/images/showcase/artwork-gallery.png) <br> *Lazy-loaded high-resolution gallery showcasing traditional Maghrebi calligraphy plates executed with reed pen (*qalam*), natural ink, and gold leaf illumination (*tadhhib*).* |

</div>

<br>

<div align="center">

| 📚 Distance Cohort Curriculum & Track Structure (`البرنامج الدراسي`) | 📜 Master Calligrapher Biography & Fes Atelier (`عن الأستاذ`) |
|:---:|:---:|
| ![Cohort Curriculum and Pricing](./public/images/showcase/cohort-curriculum.png) <br> *Structured 3-month cohort levels across Mabsut, Mujawhar, Maghrebi Thuluth, and Andalusi scripts — combining weekly live classes with line-by-line group critique sessions.* | ![Master Biography and Workshop](./public/images/showcase/about-master.png) <br> *Academic and artistic profile of Master Ibrahim Hassani Idrissi (Al-Qarawiyyin graduate & 2025 Mohammed VI Calligraphy Award laureate) teaching in Fes.* |

</div>

<br>

<div align="center">

| 📱 Mobile-First Responsive RTL Experience |
|:---:|
| <img src="./public/images/showcase/mobile-rtl-landing.png" alt="Mobile RTL Landing Experience" width="380"> <br> *Mobile-first responsive layout engineered with CSS Logical Properties, Amiri/Noto Naskh Arabic web fonts, and one-tap WhatsApp cohort registration.* |

</div>

---

## 👥 Credits

- **Master Calligrapher & Instructor:** [إبراهيم حسني إدريسي](https://hassanicalligraphy.com) (Ibrahim Hassani Idrissi), Fes, Morocco.
- **System Architecture & Full-Stack Development:** Built by [خالد بنجلون](https://benjelloun.dev) (Khalid Benjelloun) using Replit SSH, Claude Code, and [Google Antigravity](https://github.com/google).
