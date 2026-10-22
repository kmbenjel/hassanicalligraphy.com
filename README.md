# Ibrahim Calligraphy (إبراهيم حسني إدريسي — الخط العربي المغربي)

<div align="center">

**Interactive Digital Showcase, Virtual Academy & Distance Cohorts for Moroccan Arabic Calligraphy**

[![Live Website](https://img.shields.io/badge/Live%20Platform-hassanicalligraphy.com-10b981?style=for-the-badge&logo=google-chrome&logoColor=white)](https://hassanicalligraphy.com/)
[![React / Vite](https://img.shields.io/badge/Frontend-React%20%7C%20Vite%20%7C%20Tailwind-61dafb?style=for-the-badge&logo=react&logoColor=black)](https://vitejs.dev)
[![Typography](https://img.shields.io/badge/Typography-Traditional%20Maghrebi%20RTL-orange?style=for-the-badge)](https://hassanicalligraphy.com/)
[![Performance](https://img.shields.io/badge/UX-Sub--second%20Fast%20Load-blue?style=for-the-badge)](https://hassanicalligraphy.com/)

[**🌐 Live Production Platform (hassanicalligraphy.com / ibrahimcalligraphy.com)**](https://hassanicalligraphy.com/)

</div>

---

## 📌 Executive Summary

**Ibrahim Calligraphy** (`hassanicalligraphy.com` / `ibrahimcalligraphy.com`) is a digital cultural platform and distance-learning portal built for master calligrapher and teacher **Ibrahim Hassani Idrissi** (Fes, Morocco).

The platform serves two primary goals:
1. **Interactive Cultural Showcase**: High-resolution gallery and curated historical context celebrating authentic Moroccan calligraphy styles (المبسوط، المجوهر، الثلث المغربي، والكوفي المربع).
2. **Virtual Masterclass & Cohort Enrollment**: An optimized enrollment and onboarding funnel for small, intensive distance learning cohorts (10 to 15 students per group), featuring weekly live streaming sessions, structured homework critique schedules, and direct master feedback.

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

## 📸 Visual Snapshots & Video Demos

> [!NOTE]
> Below are placeholder cards for desktop/mobile UI screen captures, high-resolution calligraphic artwork plates, and student workshop videos.

<div align="center">

| 📱 Mobile-First RTL Landing Experience | ✒️ Interactive Artwork & Script Gallery |
|:---:|:---:|
| ![Mobile Experience Placeholder](https://placehold.co/400x700/0f172a/d97706?text=Mobile+Cohort+Landing) <br> *Seamless RTL enrollment flow with rich typography* | ![Artwork Gallery Placeholder](https://placehold.co/400x700/0f172a/10b981?text=Maghrebi+Script+Gallery) <br> *High-resolution inspection of classical Maghrebi scripts* |

</div>

<br>

<div align="center">

| 🎥 Live Online Masterclass Demo Video | 📜 Master Calligrapher Profile & Biography |
|:---:|:---:|
| ![Live Class Video Placeholder](https://placehold.co/600x400/0f172a/e11d48?text=Live+Class+Video+Demo) <br> *Video demonstration of live critique and pen technique* | ![Calligrapher Bio Placeholder](https://placehold.co/600x400/0f172a/3b82f6?text=Master+Calligrapher+Profile) <br> *Master Ibrahim Hassani Idrissi in his Fes workshop* |

</div>

---

## 👥 Credits

- **Master Calligrapher & Instructor:** [إبراهيم حسني إدريسي](https://hassanicalligraphy.com) (Ibrahim Hassani Idrissi), Fes, Morocco.
- **System Architecture & Development:** Built by [خالد بنجلون](https://benjelloun.dev) (Khalid Benjelloun) with [Google Antigravity](https://github.com/google).
