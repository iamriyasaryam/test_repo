
# 🧩 Companion Frontend Architecture (MVP)

The frontend of **Companion** is built using **React + Tailwind CSS**, designed to provide a premium developer-centric experience inspired by platforms like GitHub, Micro1, and Careerflow.

---

## 🏗️ Tech Stack

| Layer        | Technology         |
|--------------|--------------------|
| UI Library   | React 18+          |
| Styling      | Tailwind CSS       |
| Fonts        | Sora (primary), JetBrains Mono (code), One bold accent font |
| Animations   | Framer Motion / Tailwind transitions |
| Routing      | React Router       |
| State Mgmt   | React Context / Zustand (for scalable state) |
| Forms        | React Hook Form / Formik |
| HTTP         | Axios              |
| Icons        | Lucide / HeroIcons / Custom SVGs |

---

## 🧱 Folder Structure

```
src/
├── assets/                # Logo, Images, SVGs
├── components/            # Global reusable components
│   ├── buttons/
│   ├── cards/
│   ├── navbar/
│   ├── footer/
│   ├── layout/
├── constants/             # Global constants
├── context/               # App-wide context providers
├── hooks/                 # Custom React Hooks
├── pages/                 # Main routed pages
│   ├── Landing/
│   ├── Home/
│   ├── Discover/
│   ├── Profile/
│   ├── ProjectDetail/
│   ├── Blog/
│   ├── Auth/
│   ├── DashboardRecruiter/
│   ├── NotFound.jsx
├── routes/                # Route definitions
├── services/              # API services
├── styles/                # Tailwind/theme overrides
├── utils/                 # Helper functions
└── App.jsx
```

---

## 🧭 Routing Architecture

| Route Path           | Page Component              | Purpose |
|----------------------|-----------------------------|---------|
| `/`                  | `LandingPage.jsx`           | Public landing for devs + recruiters |
| `/home`              | `HomePage.jsx`              | Dev’s personalized feed |
| `/discover`          | `DiscoverPage.jsx`          | Explore users, posts, articles |
| `/profile/:username` | `ProfilePage.jsx`           | Developer's public portfolio/profile |
| `/project/:id`       | `ProjectDetail.jsx`         | Full detail of any project |
| `/blog`              | `BlogHome.jsx`              | Public blog index |
| `/blog/:slug`        | `BlogPost.jsx`              | Single blog post |
| `/auth/login`        | `LoginPage.jsx`             | Login for devs or recruiters |
| `/auth/register`     | `RegisterPage.jsx`          | Register new user |
| `/dashboard`         | `RecruiterDashboard.jsx`    | Private recruiter dashboard |
| `*`                  | `NotFound.jsx`              | 404 fallback |

---

## 📄 Pages Required for MVP

1. **Landing Page**  
2. **Auth Pages (Login/Register)**  
3. **User Home Feed**  
4. **Discover Page (Search, trending)**  
5. **Profile Page (Dev profile = portfolio)**  
6. **Project Detail Page**  
7. **Blog Section (List + Single)**  
8. **Recruiter Dashboard**  
9. **404 Page**

---

## 🧩 Component Categories

### Global Components:
- Navbar (glass floating)
- Footer (multi-column GitHub style)
- Buttons (primary, outline, icon)
- CTA Section
- Toast/Alert
- Modal (Login, Add Project, Report, etc.)
- Loader

### Landing Page Sections:
- Hero Section
- Company Strip Slider
- How It Works (Verification)
- Features for Devs & Recruiters
- Points System + Portfolio Unlock
- Call to Action (Join Now)
- Blog/Resources Previews
- Footer

### Profile Page Components:
- ProfileHeader
- BioCard
- ProjectListCard
- SkillsCard
- Timeline (Education + Exp)
- Verification Badges
- EndorsementsList
- Report/Feedback Buttons

### Discover Page:
- Filter Bar (Trending/Recent)
- Post Cards (Text, Image, Project)
- Article/Project/User Highlights
- Tags/Hashtags Filter

### Recruiter Dashboard:
- Search/Filter Panel
- Profile Previews (Cards)
- Trust Score & Badge View
- Shortlist (wishlist/cart-style)
- Detailed View Modal

---

## 🧠 Theme + UI Strategy

- **Color Palette:** Jet black base, deep red accent `#D11F4E`, white/gray for text.
- **Background Texture:** Grid dots, soft gradients, or subtle patterns.
- **Glassmorphism:** Used on Navbar, Cards, and Modals.
- **Micro Interactions:** Animations for hover, transitions, buttons.

---

## 🧪 Future-Proofing

- Use component-based design with full reusability.
- Build with responsiveness (mobile-first).
- Maintain centralized theme for colors, spacing, and typography.
- Integrate lazy loading and code splitting.

---

## 🎯 Final Goal

Create a frontend experience that:
- Highlights credibility over fluff.
- Encourages interaction and trust.
- Feels modern, polished, and developer-centric.
