# Technical and Content Specification — BioCaucasus

## 1. Project Overview

The goal of this project is to build a highly informative, static promotional website for **Caucasus BioSphere Expeditions**, an eco-tourism and citizen science platform focused on Georgia's unique biodiversity. The primary objective is to encourage visitors to explore Georgia while participating in real scientific fieldwork and contributing to ecological data collection across four distinct ecosystems.

The architecture prioritizes a clear, intuitive user experience (UX), responsive design, and fast loading times, utilizing a pure **HTML5/CSS3/Vanilla JavaScript** stack with no frameworks, backend services, or databases.

---

## 2. Site Architecture / Sitemap

The website will feature a flat and easy-to-navigate structure consisting of four primary pages:

* **Home (`index.html`):** The entry point, introducing the BioSphere mission, featured ecosystems, and the primary expedition CTA.
* **Expeditions (`expeditions.html`):** An interactive catalog of citizen science expeditions with category filtering and application CTAs.
* **About Us (`about.html`):** The project's story, conservation mission, core principles, and research team.
* **Contact (`contact.html`):** Office contact information, expedition registration form, and embedded location map.

---

## 3. Content & UI Layout per Page

### Home

* **Navigation Bar:** Sticky header containing the Caucasus BioSphere Expeditions logo/name and links to all primary pages, with a mobile navigation toggle.
* **Hero Section:** High-quality Georgia nature imagery with a strong headline such as **“Explore Georgia. Protect Nature. Join Real Scientific Expeditions.”**, supporting text, and a prominent **“Join an Expedition”** CTA linking to the Expeditions or Contact page.
* **Featured Ecosystems:** A responsive 4-column/grid section presenting the four featured microclimates and expedition areas:

  * **Lagodekhi Protected Areas:** Ancient Forest Ecosystem — bird and large mammal tracking.
  * **Vashlovani National Park:** Semi-Desert & Steppe Ecosystem — gazelle monitoring and dry-climate research.
  * **Mtirala National Park:** Colchic Subtropical Rainforest — amphibian research and high-rainfall ecosystem monitoring.
  * **Kazbegi Alpine Zone:** Alpine Meadows — Caucasian tur conservation, glacier, and climate-change research.
* **Why Join Us:** A 4-column feature section with simple icons and short explanatory text:

  * Real Fieldwork
  * Expert Biologists
  * Zero-Impact Travel
  * Citizen Science
* **Footer:** Copyright information, social media links, and quick navigation links.

### Expeditions

* **Hero Section:** A simple page header with a natural landscape background or subtle pattern and the page title **“Expeditions.”**
* **Filters/Sorting (UI Only):** A horizontal row of Vanilla JavaScript-driven category buttons:

  * All
  * Alpine
  * Rainforest
  * Semi-Desert
  * Forest
* **Tour Grid:** The main content area displaying expedition cards. Each card will include:

  * High-quality thumbnail image
  * Location/ecosystem tag
  * Expedition title
  * Short description
  * Duration and difficulty level
  * **“Join / Apply”** CTA linking to `contact.html`
* **Dynamic Filtering:** JavaScript will show and hide expedition cards according to the selected ecosystem category without reloading the page.

### About Us

* **Our Story:** A two-column layout featuring text describing the project's purpose, citizen science approach, and conservation mission alongside a high-quality field or Georgia landscape photograph.
* **Core Conservation Pillars:** A responsive grid presenting the project's major principles, including biodiversity research, responsible tourism, habitat protection, and citizen participation.
* **Research Team Spotlight:** A responsive card grid featuring field scientists and researchers. Each card will include:

  * Scientist name
  * Specialization
  * Ecosystem focus
  * Short professional biography
  * Optional profile/field photograph

### Contact / Join Expedition

* **Contact Information:** Clearly structured office details including:

  * Tbilisi, Georgia
  * Project email
  * Phone number
  * Office hours
* **Inquiry Registration Form:** A clearly grouped form for visitors who want to participate in an expedition.
* **Embedded Map:** Responsive `<iframe>` map showing the project's office/location area.
* **Submission Success State:** After valid submission, JavaScript will replace or supplement the form with a dynamic **“Thank You for Joining the Mission”** success panel without reloading the page.

---

## 4. Form Specification

The inquiry form will be built purely with semantic HTML5 form elements and validated using Vanilla JavaScript.

### Required Input Fields & UI Structure

* **Full Name:** Text input (`<input type="text">`).
* **Email Address:** Email input (`<input type="email">`).
* **Phone Number:** Optional telephone input (`<input type="tel">`).
* **Preferred Expedition/Region:** Dropdown select (`<select>`) containing the available ecosystems/expeditions.
* **Preferred Travel Date:** Date picker (`<input type="date">`).
* **Participant Count:** Number input (`<input type="number">`).
* **Research Background / Message:** Multi-line textarea (`<textarea>`).
* **Submit Button:** Clearly styled CTA button for joining/applying to an expedition.

### Frontend JavaScript Validation Rules

* **Real-time Feedback:** Use `input` and `blur` events to validate fields before submission and display a small red error message directly below each invalid field.
* **Name:** Must not be empty and must contain at least 2 characters.
* **Email:** Must match a standard email pattern, for example: `/^[^\s@]+@[^\s@]+\.[^\s@]+$/`.
* **Phone:** Optional; if provided, it should contain a reasonable telephone character set such as numbers, spaces, `+`, `-`, and parentheses.
* **Expedition:** The default **“Select an expedition/region”** option must not be accepted as the final selection.
* **Travel Date:** Must contain a valid date selection.
* **Participant Count:** Must be greater than `0`.
* **Message:** Must contain meaningful text and should not be submitted as an empty value.
* **Submission Action:** Use `e.preventDefault()` to prevent the default browser submission. If all fields pass validation, display the **“Thank You for Joining the Mission”** success UI dynamically without reloading the page.

---

## 5. Technical Guidelines

* **HTML5 Semantics:** Strictly use semantic HTML5 tags to structure the document, including `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<form>`, and `<footer>`. This improves accessibility, document structure, and maintainability.

* **CSS Organization:**

  * Define a global `:root` block for CSS variables to manage the project's visual system.
  * Use a nature-inspired palette based on Georgia's landscapes, including **Forest Green `#2e5a44`**, **Steppe Gold `#d4a373`**, Glacier Blue, neutral earth tones, and supporting colors.
  * Use **CSS Grid** for the expedition, ecosystem, feature, and research-team layouts.
  * Use **Flexbox** for navigation, buttons, alignment, card controls, and other one-dimensional layouts.
  * Follow a **mobile-first responsive design** approach with media queries for larger screen sizes.
  * Maintain consistent spacing, typography, colors, buttons, cards, and responsive behavior throughout all pages.

* **JavaScript:** Keep all scripts modular and written in Vanilla JavaScript. Use `document.querySelector`/`querySelectorAll` for DOM selection and standard `addEventListener` handlers for interactions, including:

  * Mobile navigation toggle.
  * Expedition category filtering.
  * Real-time form validation.
  * Dynamic form success state.
  * No external JavaScript frameworks or libraries.

* **Workflow & Deployment:** Use a **Kanban workflow in Trello** to organize project tasks, moving work through stages such as planned, in progress, review, and completed. The final static website should be deployed through **Vercel or Netlify**. No backend, database, server-side processing, or external application framework is required.
