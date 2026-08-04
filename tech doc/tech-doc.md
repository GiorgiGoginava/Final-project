# Technical and Content Specification

# Caucasus BioSphere Expeditions

### Eco-Tourism & Citizen Science Platform for Georgia

**Project Type:** Static Website
**Technology Stack:** HTML5, CSS3, Vanilla JavaScript
**Version:** 1.0
**Document Type:** Technical & Content Specification

---

# 1. Project Overview

## 1.1 Project Description

**Caucasus BioSphere Expeditions** is a static educational and tourism website promoting eco-tourism, biodiversity conservation, and citizen-science expeditions across Georgia's diverse ecosystems. The platform introduces visitors to scientifically guided field experiences where participants contribute to biological research while exploring some of the country's most unique protected landscapes.

Unlike commercial travel websites, the emphasis is on conservation, environmental education, sustainable tourism, and real scientific participation. The website serves both as an informational portal and a recruitment platform for prospective expedition participants.

The project is designed as a responsive front-end website using only standard web technologies without any server-side processing.

---

## 1.2 Project Goals

The website aims to:

- Promote Georgia as a destination for ecological tourism.
- Educate visitors about Georgia's diverse microclimates and protected ecosystems.
- Encourage participation in citizen-science initiatives.
- Showcase ongoing biological research and wildlife conservation.
- Provide a simple, accessible method for users to express interest in joining expeditions.
- Demonstrate modern front-end web development practices using semantic HTML5, CSS3, and Vanilla JavaScript.

---

## 1.3 Target Audience

The platform is designed for:

- Nature enthusiasts
- Biology and environmental science students
- Eco-tourists
- Wildlife photographers
- Conservation volunteers
- Academic researchers
- Universities and educational groups
- International travelers interested in sustainable tourism

---

## 1.4 Featured Georgian Microclimates

The website highlights four ecologically distinct research destinations:

### Lagodekhi Protected Areas

- Ancient beech forests
- Endemic wildlife
- Bird monitoring
- Large mammal tracking
- Forest biodiversity surveys

### Vashlovani National Park

- Semi-desert ecosystem
- Steppe landscapes
- Gazelle monitoring
- Reptile research
- Dry climate ecology

### Mtirala National Park

- Colchic subtropical rainforest
- Endemic plant species
- Amphibian biodiversity
- High rainfall ecosystems
- Moss and fern habitats

### Kazbegi Alpine Zone

- Alpine meadows
- Glacier monitoring
- High-altitude flora
- Caucasian Tur conservation
- Climate change research

---

## 1.5 Technology Stack

The website will be developed exclusively using:

### HTML5

Used for:

- Semantic page structure
- Accessibility
- SEO-friendly markup
- Forms
- Navigation

---

### CSS3

Used for:

- Responsive layouts
- Grid systems
- Flexbox alignment
- Typography
- Animations
- Color themes
- Component styling

---

### Vanilla JavaScript

Used for:

- Mobile navigation toggle
- Form validation
- Interactive filters
- Dynamic UI behavior
- Success message display
- Basic DOM manipulation

---

### No External Dependencies

The project intentionally excludes:

- Backend technologies
- Databases
- Frameworks (React, Vue, Angular)
- Bootstrap
- jQuery
- Node.js
- APIs
- Authentication systems

The website functions entirely as a static front-end project.

---

# 2. Site Architecture / Sitemap

The project follows a flat four-page architecture.

```
index.html
│
├── expeditions.html
├── about.html
└── contact.html
```

---

## 2.1 Home (index.html)

The homepage serves as the primary landing page introducing visitors to the mission of Caucasus BioSphere Expeditions. It provides a visual overview of featured destinations, highlights the organization's values, and directs users toward expedition opportunities.

---

## 2.2 Expeditions (expeditions.html)

This page showcases available field expeditions throughout Georgia. Users can browse research locations, compare expedition characteristics, and filter expeditions by ecosystem type before proceeding to the application page.

---

## 2.3 Research & Mission (about.html)

This page communicates the scientific mission of the organization, explains its conservation philosophy, and introduces the field researchers and expedition leaders responsible for ongoing ecological projects.

---

## 2.4 Join Expedition / Contact (contact.html)

The contact page provides organizational contact information, displays the headquarters location, and contains the expedition inquiry form used by interested participants.

---

# 3. Content & UI Layout per Page

---

# Home (index.html)

## Sticky Navigation

Navigation remains fixed to the top of the viewport during scrolling.

Navigation links:

- Home
- Expeditions
- Research & Mission
- Join Expedition

A responsive mobile navigation menu is available for smaller screens.

---

## Hero Section

The hero section serves as the primary visual introduction.

### Components

Headline:

> Explore Georgia. Protect Nature. Join Real Scientific Expeditions.

Subtitle:

> Travel beyond tourism and become part of biodiversity research across Georgia's remarkable ecosystems.

Primary CTA Button:

**Explore Expeditions**

Secondary CTA:

**Learn About Our Mission**

Background imagery emphasizes Georgia's forests, alpine landscapes, wildlife, and protected areas.

---

## Featured Expeditions Grid

A responsive grid featuring four expedition highlights:

1. Lagodekhi Wildlife Tracking
2. Vashlovani Desert Ecology
3. Mtirala Rainforest Biodiversity
4. Kazbegi Alpine Research

Each card contains:

- Featured image
- Expedition title
- Short description
- Duration
- CTA button

---

## Why Join Us

Four informational columns with icon support.

### Real Fieldwork

Participate directly in scientific research projects.

### Expert Biologists

Learn from experienced conservation scientists.

### Zero-Impact Travel

Follow environmentally responsible tourism principles.

### Citizen Science

Contribute valuable ecological observations used by researchers.

---

## Footer

Contains:

- Quick Navigation
- Contact Information
- Social Media Icons
- Copyright
- Sustainability statement

---

# Expeditions (expeditions.html)

## Hero Header

A compact hero section introducing Georgia's scientific expeditions.

---

## Expedition Filters

Interactive buttons:

- All
- Alpine
- Rainforest
- Semi-Desert
- Forest

JavaScript filters displayed cards without reloading the page.

---

## Expedition Cards Grid

Each expedition card includes:

- Expedition photograph
- Expedition title
- Georgian location
- Research focus
- Duration
- Difficulty level
- "Apply Now" button

The Apply Now button redirects users to:

```
contact.html
```

---

# Research & Mission (about.html)

## Two-Column Introduction

### Left Column

Story of the organization.

Topics include:

- Conservation mission
- Citizen science
- Educational outreach
- Sustainable tourism
- Long-term biodiversity monitoring

### Right Column

Large photograph showing researchers conducting fieldwork in Georgia.

---

## Core Conservation Pillars

Responsive grid featuring:

- Wildlife Monitoring
- Habitat Restoration
- Environmental Education
- Climate Research
- Sustainable Tourism
- Community Engagement

---

## Field Scientists Spotlight

Research team cards displaying:

- Portrait
- Name
- Research specialization
- Primary ecosystem
- Biography

---

# Join Expedition / Contact (contact.html)

## Contact Information

Organization Headquarters

Tbilisi, Georgia

Email

[info@caucasusbiosphere.ge](mailto:info@caucasusbiosphere.ge)

Phone

+995 XXX XX XX XX

Office Hours

Monday–Friday

09:00–18:00

---

## Inquiry Form

Centered responsive form encouraging expedition registration.

---

## Google Map

Embedded iframe displaying the organization's office or expedition coordination center in Tbilisi.

---

# 4. Form Specification

## HTML Form Fields

| Field                         | Input Type | Required |
| ----------------------------- | ---------- | -------- |
| Full Name                     | text       | Yes      |
| Email Address                 | email      | Yes      |
| Phone Number                  | tel        | No       |
| Preferred Expedition / Region | select     | Yes      |
| Preferred Travel Date         | date       | Yes      |
| Participant Count             | number     | Yes      |
| Research Background / Message | textarea   | Yes      |
| Submit                        | button     | Yes      |

---

## Dropdown Options

- Select an Expedition
- Lagodekhi Protected Areas
- Vashlovani National Park
- Mtirala National Park
- Kazbegi Alpine Zone

---

# JavaScript Validation Rules

## Validation Events

Validation occurs using:

- input
- blur

Real-time feedback is provided while the user interacts with the form.

---

## Error Display

Validation errors appear:

- Immediately beneath the relevant input
- Styled in red
- Removed automatically once corrected

---

## Validation Criteria

### Full Name

Requirements:

- Minimum 2 characters
- Alphabetic characters and spaces permitted
- Cannot be empty

---

### Email Address

Validated using a regular expression.

Example format:

```
name@example.com
```

---

### Preferred Expedition

The default placeholder option is considered invalid.

Users must select one of the listed Georgian reserves.

---

### Participant Count

Rules:

- Must be numeric
- Greater than zero
- Whole numbers only

---

### Phone Number

Optional.

If provided:

- Accepts digits
- Optional "+" prefix
- Spaces and hyphens permitted

---

### Research Background

Cannot be empty.

Encourages applicants to describe:

- Academic interests
- Conservation experience
- Motivation

---

## Form Submission

JavaScript intercepts form submission using:

```javascript
event.preventDefault();
```

Upon successful validation:

- Form submission is prevented.
- The form is hidden.
- A confirmation panel is displayed.

Success message:

# Thank You for Joining the Mission!

> Your expedition inquiry has been received. Our research coordinators will contact you soon with expedition details and preparation information.

---

# 5. Technical Guidelines

## HTML5 Standards

The project follows semantic HTML5 structure.

Required semantic elements include:

- `<header>`
- `<nav>`
- `<main>`
- `<section>`
- `<article>`
- `<footer>`

Additional semantic considerations:

- Proper heading hierarchy (`h1`–`h6`)
- Meaningful `alt` attributes for images
- Descriptive link text
- Accessible form labels
- Logical document outline

These practices improve accessibility, maintainability, and search engine optimization.

---

## CSS Architecture

### CSS Variables

Global variables are defined within the `:root` selector.

#### Color Palette

Inspired by Georgia's natural environments:

- Forest Green
- Moss Green
- Steppe Gold
- Glacier Blue
- Alpine White
- Charcoal Gray
- Earth Brown

Variables also define:

- Typography
- Font sizes
- Spacing scale
- Border radius
- Shadows
- Transition durations

---

### Layout System

#### CSS Grid

Used for:

- Expedition card grids
- Feature sections
- Two-column layouts
- Conservation pillar grid
- Footer organization

---

#### Flexbox

Used for:

- Navigation
- Hero content alignment
- Buttons
- Card headers
- Form layout
- Footer links

---

### Responsive Design

The project follows a mobile-first development strategy.

Recommended breakpoints:

| Device  |      Width |
| ------- | ---------: |
| Mobile  |    < 768px |
| Tablet  | 768–1023px |
| Desktop |   ≥ 1024px |

Media queries adapt:

- Navigation
- Grid columns
- Typography
- Image scaling
- Button sizing
- Section spacing

---

## JavaScript Guidelines

Implementation uses modern, framework-free JavaScript.

Recommended practices:

- Modular organization by feature
- `document.querySelector()` and `document.querySelectorAll()` for DOM selection
- `addEventListener()` for user interactions
- Event delegation where appropriate
- Clear function naming and separation of concerns

Core interactive features include:

- Mobile navigation toggle
- Expedition filter controls
- Real-time form validation
- Submission interception with `event.preventDefault()`
- Success state rendering after valid submission

---

## Workflow

Development follows a simple Kanban methodology managed in Trello.

### To Do

- Plan content
- Prepare page wireframes
- Collect imagery
- Define styles
- Create HTML structure

### In Progress

- Implement layouts
- Build responsive components
- Develop interactive JavaScript
- Test accessibility and responsiveness

### Done

- Cross-browser testing
- Content review
- Performance optimization
- Final quality assurance
- Deployment

---

## Deployment Strategy

As a static website, deployment is straightforward.

### Hosting Platforms

Recommended options:

- Vercel
- Netlify

Deployment process:

1. Organize project files (`index.html`, `expeditions.html`, `about.html`, `contact.html`, `css/`, `js/`, `img/`).
2. Push the repository to a Git hosting service.
3. Connect the repository to Vercel or Netlify.
4. Configure build settings (none required for static hosting).
5. Deploy automatically on each commit.
6. Attach a custom domain if desired.
7. Enable HTTPS and verify production functionality.

---

# Conclusion

The **Caucasus BioSphere Expeditions** website is designed as a modern, accessible, and responsive static web application that promotes eco-tourism, conservation, and citizen science within Georgia's diverse natural landscapes. By combining semantic HTML5, scalable CSS3 architecture, and focused Vanilla JavaScript interactions, the project demonstrates professional front-end development practices while providing an engaging platform for visitors to discover research expeditions, learn about conservation initiatives, and register their interest in participating. Its streamlined four-page structure, responsive interface, and maintainable codebase make it suitable for academic assessment, portfolio presentation, and real-world deployment on static hosting platforms.
