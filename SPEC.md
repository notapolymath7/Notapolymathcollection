# Notapolymath Collection - Digital Book Library

## Project Overview
- **Project name**: Notapolymath Collection
- **Type**: Single-page web application (single HTML file)
- **Core functionality**: A digital library showcase for physics, chemistry, and mathematics books with filtering, search, and PDF reader modal
- **Target users**: Students, researchers, and enthusiasts of STEM subjects

## UI/UX Specification

### Layout Structure

**Page Sections**:
1. Fixed left sidebar (260px width)
2. Main content area (remaining width)
   - Sticky topbar
   - Page heading + tab pills
   - Book grid sections

**Responsive Breakpoints**:
- Desktop: Full layout (≥1024px)
- Tablet: Sidebar collapses to icons (768px-1023px)
- Mobile: Sidebar hidden, hamburger menu (< 768px)

### Visual Design

**Color Palette**:
- Background: `#0d0d0f`
- Surface primary: `#141418`
- Surface secondary: `#1c1c22`
- Border: `#2a2a35`
- Physics accent: `#3b82f6` (blue)
- Chemistry accent: `#10b981` (green)
- Mathematics accent: `#f59e0b` (amber)
- All subjects: `#a78bfa` (purple)

**Typography**:
- Logo/Headings: Playfair Display (serif), weights 400, 600, 700
- Body text: DM Sans (sans-serif), weights 400, 500, 600
- Labels/badges: DM Mono (monospace), weight 500

**Spacing System**:
- Base unit: 4px
- Sidebar padding: 24px
- Card gap: 20px
- Section margin: 32px

**Visual Effects**:
- SVG noise texture overlay (subtle, 0.03 opacity)
- Box shadows on cards with colored glow on hover
- Smooth transitions (0.3s ease)
- Glowing dots on nav items

### Components

**Sidebar**:
- Logo section: 📚 emoji + "Notapolymath Collection" title + "DIGITAL LIBRARY" subtitle
- Navigation items: All, Physics, Chemistry, Mathematics
  - Colored glowing dot (subject color)
  - Label text
  - Book count badge
- Footer: Copyright text

**Topbar**:
- Search input (filters cards live)
- "+ Upload Book" button

**Tab Pills**:
- Horizontal row: All, ⚛ Physics, 🧪 Chemistry, ∑ Mathematics
- Active state with background color

**Book Cards**:
- Colored cover area with large emoji
- Subject tag badge (colored)
- Book title (bold)
- Author name
- Page count + file size metadata
- Two buttons: "📖 Read" (opens modal), "⬇ PDF" (download)
- Hover: colored glow effect

**Modal**:
- Book emoji + title
- Placeholder PDF viewer (iframe with code snippet)
- Download PDF button
- Close button (×)
- Click overlay to close

## Functionality Specification

### Core Features

1. **Navigation Filtering**
   - Click sidebar nav items to filter books by subject
   - Click tab pills to filter books by subject
   - Sidebar and tabs stay in sync

2. **Search**
   - Live filtering by title/author
   - Updates total book count
   - Case-insensitive matching

3. **Book Display**
   - Grouped by subject (Physics, Chemistry, Mathematics)
   - Each subject has a section header
   - Cards within section in responsive grid

4. **PDF Reader Modal**
   - Opens on "Read" button click
   - Shows book info + placeholder iframe
   - "Download PDF" button
   - Closes on × or overlay click

### Data (21 Books)

**Physics (7)**:
1. Concepts of Physics Vol.1 - H.C. Verma - 470 pages - 12.5 MB
2. University Physics - Young & Freedman - 1536 pages - 45.2 MB
3. The Feynman Lectures Vol. I - Feynman - 1552 pages - 38.7 MB
4. Introduction to Electrodynamics - Griffiths - 554 pages - 18.3 MB
5. Waves & Oscillations - N.K. Bajaj - 612 pages - 15.8 MB
6. Classical Mechanics - Goldstein - 680 pages - 22.1 MB
7. Modern Physics - Arthur Beiser - 528 pages - 14.9 MB

**Chemistry (7)**:
1. Organic Chemistry - Morrison & Boyd - 1250 pages - 32.4 MB
2. Physical Chemistry - Atkins - 1056 pages - 28.6 MB
3. Inorganic Chemistry - J.D. Lee - 824 pages - 21.2 MB
4. Biochemistry - Stryer - 1204 pages - 35.7 MB
5. Pharmaceutical Chemistry - Ashutosh Kar - 456 pages - 11.3 MB
6. Green Chemistry - Paul Anastas - 324 pages - 8.9 MB
7. Thermodynamics in Chemistry - Castellan - 680 pages - 17.4 MB

**Mathematics (7)**:
1. Higher Engineering Mathematics - B.S. Grewal - 1108 pages - 29.8 MB
2. Calculus: Early Transcendentals - Stewart - 1344 pages - 41.2 MB
3. Linear Algebra - Gilbert Strang -  576 pages - 16.5 MB
4. Probability & Statistics - Walpole - 812 pages - 24.1 MB
5. Number Theory - Hardy & Wright -  428 pages - 13.2 MB
6. Differential Equations - Dennis Zill -  518 pages - 15.6 MB
7. Discrete Mathematics - Kenneth Rosen -  972 pages - 26.9 MB

### Book Emojis
- Physics: ⚛️
- Chemistry: 🧪
- Mathematics: ∑

## Acceptance Criteria

1. ✅ Page loads with dark theme and noise texture
2. ✅ Sidebar shows logo, navigation, footer
3. ✅ All 21 books displayed in grouped sections
4. ✅ Clicking nav/tabs filters to correct subject
5. ✅ Search filters cards live by title/author
6. ✅ Book count updates correctly
7. ✅ Modal opens on "Read" click
8. ✅ Modal closes on × or overlay click
9. ✅ Cards have hover glow effect
10. ✅ Responsive layout works on different widths