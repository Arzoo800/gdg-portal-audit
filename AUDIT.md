# GDG Portal Review & Suggestions Report

**Website URL:** https://gdgcaitr.vercel.app/
**Reviewed by:** [Aapka Naam Here]
**Role:** Web Developer Applicant (GDGoC AITR)

---

## 1. Responsiveness & Visual Inspection

### Mobile View (375px - 430px screens)
- **Broken Links:** Checked main navigation and footer links. Found placeholder links (`#`) in social icons/footer that need exact redirection.
- **Text Alignment:** On smaller screens (e.g., iPhone SE/Android standard), some section headers wrap awkwardly or break across lines.
- **Layout Overflow:** Slight horizontal scrolling observed in event cards grid on viewports below 360px width.
- **Navbar/Hamburger Menu:** Mobile menu works, but smooth transition animations can be improved when toggling open/close state.

### Desktop View (1024px+ screens)
- **Visual Glitches:** Padding/margin inconsistency between the Hero section and the Upcoming Events section on high-resolution displays (1080p and above).
- **Asset Loading:** Large banner images on the home page take noticeable time to load (needs optimization like webp format or lazy loading).

---

## 2. Bugs & Technical Findings

1. **Console Errors/Warnings:** Unused asset warning and missing image fallback if an event image URL fails to load.
2. **Form Validation:** Input fields in interactive sections allow empty or unvalidated string submissions.
3. **Accessibility (a11y):**
   - Certain buttons and icon-only components lack proper `aria-label` attributes for screen readers.
   - Low contrast ratio on secondary grey text elements in dark mode/theme.

---

## 3. Constructive Suggestions & Feature Improvements

### Priority 1: Performance & UX
- **Image Optimization:** Convert png/jpg images to `.webp` format and implement Next.js / React lazy loading (`loading="lazy"`).
- **SEO & Meta Tags:** Add Open Graph (OG) tags so that links share rich preview cards on WhatsApp, Twitter, and LinkedIn.
- **Skeleton Loaders:** Add animated skeleton components while fetching events data to improve Perceived Performance.

### Priority 2: New Feature Ideas
- **Interactive Event Calendar:** A filterable month-view calendar showing all past and future GDGoC events.
- **Member / Contributor Leaderboard:** A section displaying active community members, GitHub contributors, or event badges earned.
- **Dark/Light Mode Toggle:** Persistent dark/light theme switch saved in `localStorage`.
- **Search & Filter:** Live search bar on the events page to filter events by category (e.g., Hackathon, Workshop, Tech Talk).

---

## 4. Summary Checklist

- [x] Tested across Mobile, Tablet, and Desktop screen sizes.
- [x] Identified layout responsiveness and padding bugs.
- [x] Documented missing accessibility tags and image performance issues.
- [x] Provided actionable suggestions for new features and performance gains.