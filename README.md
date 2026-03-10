Name: Christopher Banda Student ID: 2022048971

## Design Theme

The portfolio follows a **warm dark editorial** aesthetic — a deliberate contrast between a deep navy-black hero section and warm off-white content sections. The goal was to feel professional and modern without being cold or generic.

**Color Palette:** The primary background is a warm off-white (`#fafaf8`) with a complementary warm beige (`#f0ede8`) used to alternate section backgrounds and create visual rhythm. The hero section uses a near-black deep navy (`#0f0f1a`) to create a strong first impression. The accent color is a bold terracotta-red (`#e8533a`), used consistently for buttons, hover states, section underlines, and the profile image border — tying the whole design together.

**Typography:** Two Google Fonts are paired intentionally. *Syne* (an angular, geometric display font) is used for all headings, the logo, navigation, and buttons — giving the portfolio a distinctive, modern edge. *DM Sans* (a clean, humanist sans-serif) is used for body text, ensuring comfortable readability across all sections.

**Layout:** The hero section uses Flexbox to center content both vertically and horizontally, filling the full viewport height for a strong landing. The About section uses CSS Grid to place the profile image beside the biography text on larger screens, stacking vertically on mobile. The Projects section uses a CSS Grid that scales from 1 column (mobile) to 2 columns (tablet) to 3 columns (desktop).

**Details & Interactions:** Section headings each have a short terracotta underline accent created with a CSS `::after` pseudo-element. Project cards lift slightly on hover with a box-shadow transition. Skill badges highlight in the primary color on hover. The navigation becomes a hamburger menu on mobile, animating into an × icon when open. A subtle animated scroll indicator on the hero section guides users downward.

---

## Challenges & Solutions

**Challenge 1: Mobile Navigation Overflow**
On small screens (375px), the horizontal navigation links overflowed the header. The solution was to implement a hamburger menu that hides the nav links by default on mobile and toggles them open as a full-width dropdown using JavaScript and a `.nav__menu--open` class. The button animates between ☰ and × using CSS transforms.

**Challenge 2: Responsive CSS Grid for About Section**
Making the about section switch from a stacked single-column layout on mobile to a side-by-side image-and-text layout on tablet required careful use of CSS Grid with `grid-template-columns: 1fr` on mobile and `grid-template-columns: 240px 1fr` at the 768px breakpoint.

**Challenge 3: Maintaining Visual Consistency Across Breakpoints**
Ensuring typography, spacing, and section headings scaled well across all four breakpoints required defining all sizes as CSS custom properties in `:root` and overriding only what needed to change inside each media query, rather than rewriting styles from scratch.

---

## Credits

- **Fonts:** [Syne](https://fonts.google.com/specimen/Syne) and [DM Sans](https://fonts.google.com/specimen/DM+Sans) via Google Fonts (open source, SIL Open Font License)
- **Project images:** `aa.jpg`, `bb.jpeg`, `cc.jpg` — provided by student
- **Profile image:** `chris.jpg`
- **Color inspiration:** Custom palette designed for this project
- **No CSS frameworks used** — all styles written from scratch
