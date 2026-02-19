# From the Other Side: Paranormal Sighting Platform

This project is a full-stack web application that serves as a platform for sharing and documenting paranormal encounters. It allows users to browse existing ghost stories, submit their own sightings, and explore a curated collection of supernatural experiences from around the world.

---

## Live Demo

**[Visit the Live Site Here](https://your-deployment-url.com)**

---

## Key Technologies and Implementation Details

### Core Node.js Backend Architecture

* **HTTP Server Foundation:** Built using **Node.js's native `http` module** to create a lightweight, performant server without external framework dependencies, demonstrating fundamental web server concepts.
* **API Endpoint Management:** Implemented a clean **RESTful API structure** with dedicated GET and POST handlers at `/api` for retrieving and submitting paranormal sighting data.
* **Static File Serving:** Custom **`serveStatic` utility** handles all frontend asset delivery (HTML, CSS, JS, images) with proper MIME type detection and error handling.
* **Modular Route Handling:** Separated request logic into **dedicated handler modules** (`routeHandlers.js`) for maintainable code organization and clear separation of concerns.

### Data Management & Security

* **JSON Data Storage:** Utilizes a **local JSON file (`data.json`)** as the database for all paranormal sightings, implementing file-based persistence with proper error handling.
* **Input Sanitization:** Implements **`sanitize-html` library** to clean and validate all user-submitted content, preventing XSS attacks and ensuring data integrity.
* **UUID Generation:** Each sighting receives a **unique identifier** using UUID v4 format for reliable data referencing and management.
* **Async/Await Patterns:** Leverages **modern JavaScript async/await** throughout the codebase for clean, readable asynchronous operations.

### Frontend Interactivity & UX

* **Dynamic Content Rendering:** The `renderCards` function dynamically generates **sighting cards** from API data using template literals and DOM manipulation.
* **Event Delegation:** Implements efficient **event handling** with a single listener on the cards container for all expand/collapse interactions.
* **Progressive Disclosure:** Features **expandable story cards** with "Read in full" functionality for better content scannability and user experience.
* **Form Validation:** Client-side validation ensures **data quality** before submission, providing immediate feedback to users.

### UI/UX Design & Accessibility

* **Responsive Design:** Built with **mobile-first CSS** using Flexbox and Grid layouts for optimal viewing across all device sizes.
* **Semantic HTML5:** Utilizes **proper semantic elements** (`<header>`, `<main>`, `<article>`) and ARIA attributes for enhanced accessibility.
* **Typography & Branding:** Integrates **Google Fonts (Frijole & Poppins)** to create a distinctive, atmospheric design that matches the paranormal theme.
* **Navigation Structure:** Implements **clear site navigation** with consistent header/footer layout and intuitive user flow between Home, Read, and Upload sections.
