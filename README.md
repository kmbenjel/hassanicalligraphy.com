# Hassani Calligraphy

<div align="center">

**Interactive Digital Showcase, Virtual Academy & Distance Cohorts for Moroccan Calligraphy (`hassanicalligraphy.com`)**

[![Live Website](https://img.shields.io/badge/Live%20Platform-hassanicalligraphy.com-10b981?style=for-the-badge&logo=google-chrome&logoColor=white)](https://hassanicalligraphy.com/)
[![React / Vite](https://img.shields.io/badge/Frontend-React%20%7C%20Vite%20%7C%20Tailwind-61dafb?style=for-the-badge&logo=react&logoColor=black)](https://vitejs.dev)
[![Replit](https://img.shields.io/badge/Platform-Replit%20%2B%20VS%20Code%20SSH%20(Claude%20%26%20Antigravity)-F26207?style=for-the-badge&logo=replit&logoColor=white)](https://hassanicalligraphy.com/)
[![Typography](https://img.shields.io/badge/Typography-Traditional%20Maghrebi%20RTL-orange?style=for-the-badge)](https://hassanicalligraphy.com/)

[**🌐 Live Production Platform (hassanicalligraphy.com)**](https://hassanicalligraphy.com/)

</div>

---

## 📌 Executive Summary

**Hassani Calligraphy** ([`hassanicalligraphy.com`](https://hassanicalligraphy.com/)) is a production digital cultural platform and distance-learning academy built for master calligrapher, manuscript researcher, and teacher **Ibrahim Hassani Idrissi** (Fes, Morocco — recipient of the Mohammed VI Incentive Award for Moroccan Calligraphic Art, 2025, and graduate of the Al-Qarawiyyin Mosque calligraphy program).

The platform serves two primary goals:
1. **Interactive Cultural Showcase**: High-resolution gallery, atelier tour, and curated codicological context celebrating authentic Moroccan and Andalusi calligraphy styles (*Al-Mabsut*, *Al-Mujawhar*, *Maghrebi Thuluth*, and *Andalusi* script), alongside a cross-link to the companion manuscript encyclopedia [`masahif-al-maghrib.com`](https://masahif-al-maghrib.com).
2. **Virtual Masterclass & Cohort Enrollment**: A trilingual (`AR` / `EN` / `FR`) enrollment and onboarding funnel for small, intensive distance-learning cohorts (10 to 15 students per track, 3-month levels), featuring weekly live instructional sessions, structured homework critique schedules, and direct master feedback via WhatsApp.

---

## 🛠️ Engineering Workflow (Replit UI + Claude Code & Antigravity via VS Code Remote-SSH)

This client project was developed using a combined **Replit + VS Code Remote-SSH** workflow:

- **Replit Platform & UI**: Built and hosted on Replit using the standard Replit workspace UI and deployment pipeline.
- **Claude Code & Google Antigravity over VS Code SSH**: Connected **VS Code (and Antigravity IDE) via Remote-SSH** directly to the Replit project environment (`*.replit.dev:22`) to run **Claude Code** and **Google Antigravity** directly against the live Replit workspace.
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
        RTLDesignSystem["RTL Design System\n- Classical Web Typography\n- CSS Logical Properties\n- Warm Parchment & Gold Aesthetics"]
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
    S->>C: Clicks 'Register for Upcoming Cohort'
    C->>C: Validates remaining seat capacity (Limited 10-15 students)
    C->>WA: Pre-populates structured registration message
    WA->>M: Direct transmission of student inquiry & background
    M-->>S: Confirms enrollment, delivers course materials & private class link
```

---

## ✒️ Calligraphic Styles Preserved

The digital gallery highlights the nuanced distinctions between classical Maghrebi calligraphic schools:

| Style | Codicological Role | Visual Characteristics |
|---|---|---|
| **Al-Mabsut** | Principal script for Qur'anic manuscripts and sacred texts | Rounded curves, deep open bowls (*nun*, *sad*), balanced proportions, and clear legibility. |
| **Al-Mujawhar** | Royal correspondence, legal edicts, and scholarly treatises | Fluid, ligature-rich, rapid cursive flow with tight vertical rhythm. |
| **Maghrebi Thuluth** | Monumental architectural inscriptions, illuminated headings | Towering ascenders, sharp architectural angles, and decorative majesty. |
| **Square Kufic** | Geometric architectural medallions and tilework (*Zellij*) | Strict orthogonal grid, binary ink/negative balance, mathematical precision. |

---

## 📸 Live Production UI Showcase (`hassanicalligraphy.com`)

<div align="center">

| 🏛️ Trilingual (`AR` / `EN` / `FR`) Hero & Cohort Registration | ✒️ Interactive Artwork & Illuminated Manuscript Gallery |
|:---:|:---:|
| ![Desktop Hero and Cohort CTA](./public/images/showcase/desktop-hero-bio.png) <br> *Warm parchment-inspired RTL landing interface with language switcher (`AR` / `EN` / `FR`), upcoming cohort countdown, and direct WhatsApp enrollment.* | ![Interactive Artwork Gallery](./public/images/showcase/artwork-gallery.png) <br> *Lazy-loaded high-resolution gallery showcasing traditional Maghrebi calligraphy plates executed with reed pen (*qalam*), natural ink, and gold leaf illumination (*tadhhib*).* |

</div>

<br>

<div align="center">

| 📚 Distance Cohort Curriculum & Track Structure | 📜 Master Calligrapher Biography & Fes Atelier |
|:---:|:---:|
| ![Cohort Curriculum and Pricing](./public/images/showcase/cohort-curriculum.png) <br> *Structured 3-month cohort levels across Mabsut, Mujawhar, Maghrebi Thuluth, and Andalusi scripts — combining weekly live classes with line-by-line group critique sessions.* | ![Master Biography and Workshop](./public/images/showcase/about-master.png) <br> *Academic and artistic profile of Master Ibrahim Hassani Idrissi (Al-Qarawiyyin graduate & 2025 Mohammed VI Calligraphy Award laureate) teaching in Fes.* |

</div>

<br>

<div align="center">

| 📱 Mobile-First Responsive RTL Experience |
|:---:|
| <img src="./public/images/showcase/mobile-rtl-landing.png" alt="Mobile RTL Landing Experience" width="380"> <br> *Mobile-first responsive layout engineered with CSS Logical Properties, classical web fonts, and one-tap WhatsApp cohort registration.* |

</div>

---

## 👥 Credits

- **Master Calligrapher & Instructor:** [Ibrahim Hassani Idrissi](https://hassanicalligraphy.com), Fes, Morocco.
- **System Architecture & Full-Stack Development:** Built by [Khalid Benjelloun](https://benjelloun.dev) using Replit, alongside Claude Code and [Google Antigravity](https://github.com/google) via a VS Code Remote-SSH connection to the Replit workspace.
