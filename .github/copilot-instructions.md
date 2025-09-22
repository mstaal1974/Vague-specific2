# Copilot Instructions for AI Agents

## Project Overview
This is a single-page interactive web app for categorizing instructions as "Vague" or "Specific." The app is implemented in a single `Index.html` file using vanilla JavaScript, Tailwind CSS (via CDN), and custom CSS. No build tools or external dependencies are required beyond the CDN links.

## Architecture & Key Patterns
- **Single-file structure:** All HTML, CSS, and JavaScript are contained in `Index.html`. There are no separate JS or CSS files.
- **UI Components:** The app uses Tailwind CSS utility classes for layout and styling. Custom styles are defined in a `<style>` block in the `<head>`.
- **Interactivity:** Drag-and-drop functionality is implemented with native JS event listeners. Instructions are dynamically generated and categorized by user interaction.
- **Instruction Data:** The set of instructions is hardcoded in a JS array (`allInstructions`). The app randomly selects a subset for each session.
- **Feedback:** User feedback is shown via a message element, with color and visibility controlled by JS and Tailwind classes.

## Developer Workflows
- **No build or test steps:** All development is done directly in `Index.html`. Open the file in a browser to view changes.
- **Debugging:** Use browser DevTools for JS debugging and CSS inspection. No source maps or frameworks are present.
- **Hot reload:** Refresh the browser to see changes. No live reload tooling is present.

## Project-Specific Conventions
- **Tailwind via CDN:** Do not attempt to install Tailwind locally; use the CDN link in the `<head>`.
- **Font:** Uses Google Fonts (Inter) via CDN.
- **Instruction Format:** Each instruction is an object with `text` and `category` properties. Only two categories: `vague` and `specific`.
- **Accessibility:** No explicit ARIA roles or accessibility features are implemented.

## Integration Points
- **External dependencies:**
  - Tailwind CSS: `https://cdn.tailwindcss.com`
  - Google Fonts: Inter
- **No backend or API calls.**

## Example Patterns
- **Adding new instructions:** Update the `allInstructions` array in the JS block.
- **Changing UI layout:** Edit the HTML structure and Tailwind classes in `Index.html`.
- **Modifying drag-and-drop logic:** Update JS event listeners in the `<script>` block.

## Key File
- `Index.html`: Contains all code and markup for the app.

---
For questions or improvements, edit `Index.html` directly. No other files or configuration are required.
