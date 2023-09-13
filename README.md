# Card Component Documentation

This document provides instructions on how to use the AI-themed blog card component and apply different themes. Additionally, it details the accessibility features implemented in line with WCAG standards.

## Table of Contents
- [Usage](#usage)
- [Theming](#theming)
- [Accessibility](#accessibility)

## Usage
Include the Component: Ensure the component's HTML and associated CSS are included in your project.

Content Customization:
- Replace the src attribute of the `<img>` tag with the desired image path.
- Adjust the content of the `<h2>` and `<p>` tags for the title and paragraph respectively.
- Modify the aria-label attribute of the `<button>` to reflect the button's purpose.

Adding Interactivity:
- Attach any desired JavaScript event handlers to the button for added interactivity.

## Theming
The card component supports multiple themes. Currently, there are two primary themes: light-theme and dark-theme.

Light Theme: To use the light theme, add the `light-theme` class to the `<body>` tag:

```html
<body class="light-theme">...</body>
```

Dark Theme: To use the dark theme, replace `light-theme` with `dark-theme`:

```html
<body class="dark-theme">...</body>
```

Feel free to add or modify themes in the associated CSS file.

## Accessibility
The card component is designed with accessibility in mind and adheres to WCAG standards:

- Images: The component uses the `alt` attribute for images. If the image is content-relevant, provide a descriptive alt text. For decorative images, the `alt` attribute should still be included but left empty (`alt=""`).
- Semantic HTML: Elements like `<article>`, `<h2>`, and `<button>` are used to ensure content is presented with proper hierarchy and meaning.
- Interactive Elements: The button within the component is keyboard-accessible and focusable. Clear focus styles are implemented in the CSS to provide visual feedback for keyboard navigation.
- ARIA Attributes: The `aria-label` attribute gives context to screen readers about the purpose of the button. Additionally, the decorative icon inside the button uses `role="img"` and `aria-hidden="true"` to be treated as a decorative image, ensuring screen readers provide the intended content.
- Color Contrast: Ensure that the color contrast between text and its background meets WCAG recommendations for readability.