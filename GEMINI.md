# Open Resume - Shawn's Portfolio

This project is a high-performance, bilingual (Traditional Chinese/English) personal resume website for **Shawn**, a Senior Backend and Crawler Architect. The design features a modern terminal-like aesthetic with a focus on core efficiency metrics and technical depth.

## Project Overview

- **Purpose:** Personal portfolio and resume showcase.
- **Main Technologies:**
    - **Frontend:** HTML5, [Tailwind CSS](https://tailwindcss.com/) (via CDN), [Font Awesome](https://fontawesome.com/), Google Fonts (Fira Code).
    - **Interactivity:** Vanilla JavaScript for language switching and scroll animations (Intersection Observer).
    - **Architecture:** Single-page application (SPA) style within a single `index.html` file.
- **Workflow:** Employs **SDD (Spec-Driven Development)** using AI Agents and **OpenSpec** for change management.

## Project Structure

- `index.html`: The main entry point containing all content, styles, and logic.
- `openspec/`: Contains specifications and change logs for the project.
    - `config.yaml`: Configuration for the OpenSpec workflow.
    - `specs/`: Directory for project specifications (currently empty).
    - `changes/`: History of changes applied to the project.
- `.gemini/`: Custom skills and commands for the Gemini CLI agent.

## Building and Running

Since this is a static HTML project using CDNs for all dependencies, there is no build step required.

- **To View:** Open `index.html` directly in any modern web browser.
- **Development:** Edit `index.html` and refresh the browser to see changes.
- **Deployment:** Can be hosted on any static site hosting service (GitHub Pages, Vercel, Netlify, etc.).

## Development Conventions

- **AI-Assisted Development:** The project uses the **OpenSpec** workflow. When proposing changes, use the `openspec-propose` skill.
- **Styling:** Use Tailwind CSS utility classes. Custom styles are embedded in the `<style>` tag within `index.html`.
- **Bilingual Support:** Content is wrapped in `.lang-zh` and `.lang-en` classes. Language switching is handled by the `setLang(lang)` JavaScript function.
- **Responsive Design:** Utilizes Tailwind's responsive prefixes (`md:`, `lg:`) to ensure compatibility across devices.
- **Visual Effects:** Scroll-triggered animations are implemented using the `.reveal` class and an `IntersectionObserver`.

## Key Features

- **Performance Metrics:** Showcases high-throughput (3,000+ RPS) and low-latency optimization achievements.
- **Experience Timeline:** Detailed history of roles at KICKS CREW, KooData, and attittu.
- **Project Showcase:** Highlights specialized work in performance engines, distributed crawlers, and game development (Godot).
