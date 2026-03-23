![Lexicon Logo](https://lexicongruppen.se/media/wi5hphtd/lexicon-logo.svg)

# Tailwind CSS Practice Exercises

This document contains 20 exercises to help you master Tailwind CSS, ranging from basic utility usage to advanced layout and interactivity.

---

### 1. Typography & Spacing
**Task:** Create a text section with a main heading (H1), a subtitle (H2), and two paragraphs of dummy text.
- **Goals:**
  - Use `text-4xl` for the heading and `text-xl` for the subtitle.
  - Apply `font-bold` and `font-semibold`.
  - Use `leading-relaxed` for the paragraphs.
  - Add vertical spacing between elements using `space-y-4` or `mb-4`.

### 2. Colorful Alert Boxes
**Task:** Create three different alert boxes: **Success** (Green), **Warning** (Yellow), and **Danger** (Red).
- **Goals:**
  - Use `bg-*`, `border-*`, and `text-*` colors.
  - Add `p-4` padding and `rounded-lg` corners.
  - Add a small `font-bold` label at the beginning of each alert.

### 3. Simple Card with Shadow
**Task:** Build a centered card that contains a title, a short description, and a "Read More" button.
- **Goals:**
  - Use `max-w-sm` and `mx-auto` to center it.
  - Apply `shadow-md` and `bg-white`.
  - Style the button with `bg-blue-600`, `text-white`, and `px-4 py-2`.

### 4. Circular Profile Badge
**Task:** Create a small profile component with a circular image on the left, and a name/title on the right.
- **Goals:**
  - Use `flex` and `items-center`.
  - Make the image circular using `rounded-full` and `w-12 h-12`.
  - Use `gap-4` to separate the image from the text.

### 5. Interactive Buttons
**Task:** Create a set of three buttons: **Primary**, **Secondary**, and **Outline**.
- **Goals:**
  - Add `hover:bg-*` effects.
  - Use `transition-colors` and `duration-300` for smooth changes.
  - Add `focus:ring-2` to show a ring when the button is clicked.

---

### 6. Responsive Two-Column Layout
**Task:** Create a section with text on one side and an image on the other.
- **Goals:**
  - Start as a single column on mobile.
  - Switch to two columns on medium screens (`md:grid-cols-2`).
  - Use `items-center` to vertically align the text with the image.

### 7. Product Grid (3-Columns)
**Task:** Build a responsive grid of 6 product cards (Image, Name, Price).
- **Goals:**
  - Mobile: 1 column.
  - Tablet (`sm`): 2 columns.
  - Desktop (`lg`): 3 columns.
  - Use `gap-6` for consistent spacing.

### 8. Hero Section with Overlay
**Task:** Create a hero section with a background image, a dark semi-transparent overlay, and centered white text.
- **Goals:**
  - Use `relative` for the container and `absolute inset-0` for the overlay.
  - Use `bg-black/50` (arbitrary opacity) for the overlay.
  - Center the content using `flex items-center justify-center`.

### 9. Pricing Table Comparison
**Task:** Create 3 pricing cards side-by-side. The middle card (Pro plan) should be visually distinct.
- **Goals:**
  - Use `scale-105` or a thicker `border-blue-500` to highlight the middle card.
  - Use `shadow-xl` for the highlighted card and `shadow-md` for the others.

### 10. Simple Navigation Bar
**Task:** Create a navbar with a logo on the left and 4 links on the right.
- **Goals:**
  - Use `flex justify-between`.
  - Add `hover:text-blue-500` to the links.
  - Make the navbar `sticky top-0` with a `backdrop-blur-md` effect.

---

### 11. Custom Flexbox Alignment
**Task:** Create a container with 4 small boxes and demonstrate 3 different layouts by changing only the parent classes.
- **Goals:**
  - Layout 1: Centered both ways (`justify-center items-center`).
  - Layout 2: Space between items (`justify-between`).
  - Layout 3: Items aligned to the bottom-right (`justify-end items-end`).

### 12. Feature List with Icons
**Task:** Build a grid of "Features" where each item has a colored icon background.
- **Goals:**
  - Use a small `div` with `rounded-lg` and a background color for the icon container.
  - Add a `group` class to the feature card and `group-hover:scale-110` to the icon container.

### 13. Sticky Sidebar Layout
**Task:** Create a two-column layout where the main content is long and scrollable, but the sidebar stays fixed while scrolling.
- **Goals:**
  - Use `grid-cols-4` (1 for sidebar, 3 for content).
  - Apply `sticky top-6` to the sidebar content.

### 14. Gallery with Aspect Ratios
**Task:** Create a 4-image gallery where images have different fixed aspect ratios.
- **Goals:**
  - Use `aspect-video` for the first image.
  - Use `aspect-square` for the others.
  - Use `object-cover` to prevent image distortion.

### 15. Responsive Order Change
**Task:** Create a layout with two blocks: **[Text Block]** and **[Image Block]**.
- **Goals:**
  - On mobile: Image should be on TOP.
  - On desktop: Image should be on the RIGHT.
  - **Trick:** Place Text Block first in HTML, use `order-last` or `flex-row-reverse` to flip them.

---
## Optional Exercises

### 16. Group-Hover Reveal
**Task:** Create a card with an image. When the user hovers over the card, an "Add to Cart" button should slide up from the bottom.
- **Goals:**
  - Use `group` on the card.
  - Use `translate-y-full group-hover:translate-y-0` on the button.
  - Use `overflow-hidden` on the card to hide the button initially.

### 17. Peer-State Toggle (Pure CSS)
**Task:** Create a "Terms and Conditions" checkbox that, when checked, changes the color and state of a "Submit" button below it.
- **Goals:**
  - Use the `peer` class on the checkbox.
  - Use `peer-checked:bg-green-600` and `peer-checked:cursor-pointer` on the button.
  - Use `pointer-events-none opacity-50` on the button by default.

### 18. Dark Mode Toggle Simulation
**Task:** Create a card that has two sets of styles: one for light mode and one for dark mode.
- **Goals:**
  - Use `dark:bg-slate-900` and `dark:text-white`.
  - Add a parent class `dark` to a wrapper div to test the styles.

### 19. Form Validation UI
**Task:** Build an input field for "Email" that shows a red border and a small error message only when it's focused and invalid.
- **Goals:**
  - Use `invalid:border-red-500` and `focus:invalid:ring-red-500`.
  - Use the `peer` utility to show/hide the error message.

### 20. Full Dashboard Shell
**Task:** Create the skeleton of a dashboard with a full-height sidebar and a top header.
- **Goals:**
  - Sidebar: `h-screen w-64 fixed left-0 top-0`.
  - Main Content: `ml-64 p-8`.
  - On mobile: Hide the sidebar (`hidden md:block`) and show a bottom navigation bar instead.

---

## Starter Template

You can use this template to start your exercises:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tailwind CSS Exercises</title>
  <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-50 text-gray-900">
  <div class="max-w-5xl mx-auto p-10 space-y-20">
    <h1 class="text-center text-5xl font-extrabold text-blue-600">Tailwind Practice</h1>
    
    <!-- Exercise 1 -->
    <section id="ex-1">
      <h2 class="text-2xl font-bold mb-4">1. Typography & Spacing</h2>
      <div class="p-6 bg-white rounded-xl shadow-sm border border-gray-200">
        <!-- Your Code Here -->
      </div>
    </section>

    <!-- ... Add more sections here ... -->

  </div>
</body>
</html>
```
