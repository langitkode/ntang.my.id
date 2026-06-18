# Agent Capabilities & Web Development Best Practices (AGENTS.md)

This document defines the universal standard operating procedures, architectural skills, and quality benchmarks the coding agent must apply when building or modifying this website.

## 1. Clean Code & Architecture
* **Modular Design:** Break the UI down into small, single-responsibility, reusable components.
* **Separation of Concerns:** Keep business logic, data models, and UI presentation layers strictly isolated.
* **Semantic HTML:** Always use meaningful HTML tags (e.g., `<main>`, `<section>`, `<article>`, `<header>`, `<footer>`) instead of generic nested generic divisions to ensure correct document structure.
* **Dry Principle:** Abstract repetitive logic, styling configurations, or utility functions into shared helpers.

## 2. Responsive & Modern Layouts
* **Mobile-First Approach:** Design and write layout styles for mobile devices first, then scale up using media queries for larger viewports.
* **Fluid Layouts:** Utilize flexible grid systems and flexible box models to prevent layout breakage on custom screen dimensions.
* **Content Preservation:** Ensure interactive elements (e.g., navigation menus, contact forms, tables) collapse gracefully and remain fully functional on touch devices.

## 3. Web Accessibility (a11y)
* **Screen Reader Support:** Add descriptive alternative text (`alt`) to all functional images and proper ARIA labels (`aria-*`) to interactive components lacking text.
* **Keyboard Navigation:** Ensure every interactive element (links, buttons, inputs) is focusable and can be fully operated via keyboard alone.
* **Contrast Compliance:** Maintain sufficient color contrast ratios between text elements and backgrounds to meet international accessibility guidelines.

## 4. Performance & Core Web Vitals
* **Asset Optimization:** Enforce standard modern compression formats for images and vector graphics. Implement lazy loading for off-screen mediaassets.
* **Layout Shifts:** Always declare explicit width and height dimensions or aspect-ratio boundaries on media containers to mitigate Unexpected Layout Shifts.
* **Execution Efficiency:** Avoid heavy computations inside rendering cycles. Optimize asynchronous operations to prevent blocking the user interface thread.

## 5. Security & Form Handling
* **Input Sanitization:** Validate, clean, and constrain all user-supplied data on both the interface layer and data-handling layer before processing.
* **State Management:** Securely handle state and transient data without leaking sensitive user credentials or system metadata into client logs.
