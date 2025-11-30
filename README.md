# CSS Framework

A comprehensive, token-based CSS framework featuring components, utilities, and animation effects. Built with design tokens for consistency and maintainability.

[![Documentation](https://img.shields.io/badge/docs-GitHub%20Pages-blue)](https://yourusername.github.io/css-framework/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

## ✨ Features

- **🎨 Design Tokens**: Comprehensive design system with colors, typography, spacing, shadows, and component tokens
- **🧩 Components**: Ready-to-use UI components including buttons, forms, cards, modals, and navigation
- **🔧 Utilities**: Low-level utility classes for rapid styling (spacing, typography, flexbox, etc.)
- **✨ Effects**: Animation effects including fade, bounce, scale, slide, and more
- **📱 Responsive**: Mobile-first design with responsive utilities
- **♿ Accessible**: Built with accessibility in mind
- **🎯 Consistent**: Design tokens ensure visual consistency across all components

## 🚀 Quick Start

1. **Download** the CSS files from the `css/` directory
2. **Include** the core styles in your HTML:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Project</title>

  <!-- Core framework styles -->
  <link rel="stylesheet" href="css/globals.css">
  <link rel="stylesheet" href="css/tokens.css">

  <!-- Add components as needed -->
  <link rel="stylesheet" href="css/components/btn.css">
  <link rel="stylesheet" href="css/components/card.css">
</head>
<body>
  <btn data-variant="primary">Click me!</btn>
</body>
</html>
```

3. **Use components** with data attributes:

```html
<!-- Buttons -->
<btn data-variant="primary">Primary</btn>
<btn data-variant="secondary" data-size="lg">Large Secondary</btn>

<!-- Cards -->
<card>
  <card-body>
    <card-title>Card Title</card-title>
    <p>Card content goes here.</p>
  </card-body>
</card>

<!-- Utilities -->
<div class="d-flex justify-center items-center p-4">
  <p class="text-lg font-bold">Centered content</p>
</div>
```

## 📁 File Structure

```
css-framework/
├── globals.css          # Global reset and base styles
├── tokens.css           # Design tokens (colors, spacing, etc.)
├── components/          # Component-specific styles
│   ├── btn.css         # Button component
│   ├── card.css        # Card component
│   ├── input.css       # Form inputs
│   └── ...             # Other components
├── utils/              # Utility classes
│   ├── spacing.css     # Margin and padding utilities
│   ├── text.css        # Typography utilities
│   ├── flex.css        # Flexbox utilities
│   └── ...             # Other utilities
├── effects/            # Animation effects
│   ├── fade.css        # Fade animations
│   ├── bounce.css      # Bounce animations
│   └── ...             # Other effects
└── website/            # Documentation website
```

## 🎨 Design Tokens

The framework uses CSS custom properties (variables) for all design values:

```css
/* Colors */
--color-primary-500: #0ea5e9;
--color-text-primary: #111827;

/* Spacing */
--spacing-4: 1rem;  /* 16px */
--spacing-6: 1.5rem; /* 24px */

/* Typography */
--font-size-lg: 1.125rem; /* 18px */
--font-weight-semibold: 600;
```

## 🧩 Components

### Buttons
```html
<btn>Default</btn>
<btn data-variant="primary">Primary</btn>
<btn data-variant="secondary" data-size="lg">Large Secondary</btn>
<btn disabled>Disabled</btn>
```

### Form Inputs
```html
<input-field placeholder="Text input" />
<select-field>
  <option>Option 1</option>
</select-field>
<checkbox-field>
  <input type="checkbox" id="check" />
  <label for="check">Checkbox</label>
</checkbox-field>
```

### Cards
```html
<card>
  <card-header>
    <card-title>Card Title</card-title>
  </card-header>
  <card-body>
    <p>Card content</p>
  </card-body>
  <card-footer>
    <btn>Action</btn>
  </card-footer>
</card>
```

## 🔧 Utilities

Utility classes follow a consistent naming pattern:

```html
<!-- Spacing -->
<p class="m-4">Margin all sides</p>
<p class="mt-2 mb-4">Margin top and bottom</p>
<p class="px-6 py-3">Padding horizontal and vertical</p>

<!-- Typography -->
<p class="text-lg font-bold text-center">Large bold centered text</p>

<!-- Layout -->
<div class="d-flex justify-between items-center">
  <div>Left</div>
  <div>Right</div>
</div>

<!-- Colors -->
<p class="text-primary">Primary text color</p>
<div class="bg-secondary">Secondary background</div>
```

## ✨ Effects

Add animations to elements:

```html
<!-- Include effect CSS -->
<link rel="stylesheet" href="css/effects/fade.css">

<!-- Use effects -->
<div class="fade-in">Fades in on load</div>
<div class="bounce-gentle">Gentle bouncing animation</div>
<button onclick="this.classList.add('scale-in')">Click for scale effect</button>
```

## 📚 Documentation

Complete documentation is available at: [https://yourusername.github.io/css-framework/](https://yourusername.github.io/css-framework/)

The documentation includes:
- **Getting Started**: Installation and basic usage
- **Design Tokens**: Complete token reference
- **Components**: All available components with examples
- **Utilities**: Utility class reference
- **Effects**: Animation effects guide
- **Examples**: Real-world usage examples

## 🔧 Development

### Building the Documentation

The documentation website is located in the `website/` directory. To deploy:

1. **Enable GitHub Pages** in your repository settings
2. **Choose deployment source**:
   - Option A: Copy `website/` contents to repository root
   - Option B: Rename `website/` to `docs/` and select `/docs` folder

### Modifying the Framework

- **Design Tokens**: Edit `tokens.css` to change colors, spacing, etc.
- **Components**: Modify individual component CSS files
- **Utilities**: Add new utility classes following existing patterns
- **Effects**: Create new animation effects

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test with the documentation site
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with modern CSS features and design tokens
- Inspired by utility-first frameworks and design systems
- Focus on accessibility and performance
