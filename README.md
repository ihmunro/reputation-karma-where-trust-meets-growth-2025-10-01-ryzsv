# Reputation Karma Landing Page Maintenance Guide

This guide will help you maintain and customize the Reputation Karma landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions for common updates.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the company name and navigation menu. To modify:

1. **Company Name:**
```html
<div class="text-2xl font-bold bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
    Reputation Karma <!-- Change company name here -->
</div>
```

2. **Navigation Menu Items:**
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a> <!-- Update menu text here -->
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

### Hero Section
Located at the top of the page with the main headline:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-8 bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
    Reputation Karma: Where Trust Meets Growth <!-- Update main headline here -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">
    More trust. More clients. More growth. <!-- Update subheadline here -->
</p>
```

### Tailwind CSS Classes Explained
Common classes used throughout:
- `text-[size]`: Controls text size (e.g., `text-xl`, `text-2xl`)
- `font-[weight]`: Controls text weight (e.g., `font-bold`, `font-medium`)
- `mb-[size]`: Adds margin bottom (e.g., `mb-8`, `mb-12`)
- `py-[size]`: Adds padding top and bottom (e.g., `py-24`)
- `bg-[color]`: Sets background color (e.g., `bg-white`, `bg-gray-50`)

To modify responsive design:
- `md:`: Applies styles at medium screens (768px+)
- `lg:`: Applies styles at large screens (1024px+)

Example:
```html
<!-- Changes text size based on screen size -->
<h2 class="text-3xl md:text-4xl font-bold">
```

## Managing Links

### Navigation Menu Links
Current internal links in the navigation:
```html
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="#contact">Contact</a>
```

To update:
1. Locate the link in the navigation section
2. Change the `href` attribute to your desired destination
3. Update the link text between the `<a>` tags

Example updating an external link:
```html
<!-- Before -->
<a href="#contact">Contact</a>

<!-- After -->
<a href="https://example.com/contact">Contact</a>
```

### Call-to-Action Buttons
Main CTA buttons currently point to:
```html
<a href="https://reputationkarma.com" class="inline-block px-8 py-4 bg-gradient-to-r from-blue-600 to-purple-600">
    Transform Your Reputation Today
</a>
```

To update:
1. Locate the CTA button in the HTML
2. Change the `href` attribute to your desired URL
3. Update the button text as needed

## Adding Privacy and Terms Pages

### Footer Legal Links
Current placeholder links in the footer:
```html
<div>
    <h3 class="text-white text-lg font-semibold mb-4">Legal</h3>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To add proper links:
1. Create your privacy.html and terms.html files
2. Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

Common issues and solutions:

1. **Broken Links**
   - Check that all `href` attributes have correct paths
   - Ensure file names match exactly (case-sensitive)
   - Test all links after updating

2. **Responsive Design Issues**
   - Check media query classes (`md:`, `lg:`)
   - Test on different screen sizes
   - Maintain existing responsive classes when updating

3. **Styling Problems**
   - Keep gradient classes intact for branded elements
   - Maintain spacing classes for consistent layout
   - Don't remove important utility classes like `container` and `mx-auto`

Remember to:
- Always backup your files before making changes
- Test all updates in multiple browsers
- Maintain consistent styling across all pages
- Keep the responsive design intact by preserving Tailwind's responsive classes

Need more help? Contact the development team or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).