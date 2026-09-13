![ALU Web Development Banner](https://holbertonschool.com)

# Figma to Semantic HTML — Structure & Content Architecture

## 📋 Project Overview
This project focuses on the core foundational layer of web development: translating a professional visual interface from a **Figma designer file** into a pure, clean, and semantically accurate **HTML5 structure**. 

Following best architectural practices, this phase completely separates content from presentation. There is **zero CSS and zero styling**—just a robust text blueprint that guarantees accessibility (A11y), strong Search Engine Optimization (SEO) baselines, and a logical document outline for future styling layouts.

## 🎨 Design Specifications
The structure is modeled character-for-character from the following design resources:
* **Source Files:** Page in Figma / Static Desktop & Mobile Draft Mockups.
* **Typography Requirements:** Linked asset integration placeholders prepared for `Source Sans Pro` and `Spin-Cycle-OT` typefaces.
* **Layout Geometry:** Blueprint designed by rounding pixel float coordinates down to clear structural wrappers.

## 📂 Project Structure
```text
alu-web-development/
└── html_advanced/        # Advanced structural project workspace
    ├── README.md         # Documentation engine (Current File)
    └── index.html        # Pure semantic HTML5 layout from Figma blueprints
```

## 🛠️ Core Engineering & Semantic Landmarks
To avoid the chaotic layout antipattern known as "div soup," the webpage structure is divided into explicit HTML5 landmark zones:

### 1. Document Architecture
* `<!DOCTYPE html>` & `<html lang="en">`: Establishes the modern layout parsing mode and explicitly tracks document language for text translation engines.
* `<head>`: Houses global technical metadata, strict character encoding definitions (`utf-8`), and responsive browser viewport scaling parameters.

### 2. Layout Component Blocks
Instead of using generic structural wrappers, content zones are divided using specialized container semantics:
* `<header>`: Identifies the global entry block housing branding layouts and site navigation systems.
* `<nav>`: Explicitly encapsulates the primary list item collections of site-wide hyperlinks.
* `<main>`: Tells browser accessibility scrapers exactly where the unique, core textual body of the design lives.
* `<section>`: Divides the mock design into individual thematic chapters or modules (e.g., hero blocks, services grids, testimonial arrays).
* `<article>`: Used for self-contained, independent editorial components that could be shared on external text boards.
* `<aside>`: Isolates secondary background context elements sitting distinct from the main page body timeline.
* `<footer>`: Sets the terminal block maps containing copyright details, auxiliary terms links, and signature branding notes.

### 3. Content Hierarchies & Elements
* **Heading Scaffolding (`<h1>` to `<h6>`):** Implements a strict, unbroken hierarchy of heading depths to pass document summary checks perfectly.
* **Media Anchors:** Includes explicit description tags (`alt="..."`) on graphic endpoints to satisfy strict screen-reader navigation frameworks.

## 🚦 Verification & Compliance Quality Assurance
The script logic is verified directly through command-line API requests using the **W3C Nu HTML Checker**. 

```bash
# Execute automated web syntax parsing checks
curl -H "Content-Type: text/html; charset=utf-8" --data-binary @index.html "https://w3.org"
```
*Note: A completely compliant, bug-free HTML structure results in an absolute silent exit return inside your terminal terminal shell.*

---
**Built with precision by Juanne Asabah (AJ)**
