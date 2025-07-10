# Water Damage Landing Page - Maintenance Guide

This guide will help you maintain and customize the Water Damage Restoration landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions for common updates.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Navigation Links](#managing-navigation-links)
3. [Privacy and Terms Pages](#privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Hero Section
The main headline and hero content are located in the first section after the header:

```html
<section class="pt-32 pb-24 bg-gradient-to-b from-blue-50 to-white">
    <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold tracking-tight mb-6">
        Water Damage Restoration Fort Lauderdale
    </h1>
    <p class="text-2xl md:text-3xl text-gray-600 mb-12">{hero_statement}</p>
```

To update:
1. Replace the h1 text between the tags
2. Replace `{hero_statement}` with your actual hero statement
3. Maintain the existing classes to preserve responsive design

### Service Cards
Located in the "Our Professional Services" section:

```html
<div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-xl transition-shadow duration-300">
    <h3 class="text-xl font-semibold mb-4">Fast Service</h3>
    <p class="text-gray-600">24/7 emergency response...</p>
</div>
```

To modify service cards:
1. Locate the service card div you want to update
2. Change the h3 text for the title
3. Update the p tag content for the description
4. Keep the existing classes for consistent styling

### Tailwind CSS Class Guide
Common classes used throughout:
- `text-[size]`: Controls text size (xl, 2xl, 3xl, etc.)
- `font-[weight]`: Controls text weight (semibold, bold)
- `mb-[size]`: Adds bottom margin (4, 6, 8, etc.)
- `bg-[color]`: Sets background color
- `p-[size]`: Adds padding

## Managing Navigation Links

### Header Navigation
The main navigation is in the header:

```html
<div class="hidden lg:flex space-x-8">
    <a href="#services" class="text-gray-600 hover:text-gray-900 transition-colors">Services</a>
    <a href="#benefits" class="text-gray-600 hover:text-gray-900 transition-colors">Benefits</a>
    <a href="#faq" class="text-gray-600 hover:text-gray-900 transition-colors">FAQ</a>
    <a href="#contact" class="text-gray-600 hover:text-gray-900 transition-colors">Contact</a>
</div>
```

To update navigation links:
1. Locate the link you want to change
2. Update the `href` attribute to point to your new destination
3. Update the link text between the `<a>` tags
4. Maintain the existing classes for hover effects

### Footer Links
Footer links are organized in columns:

```html
<div>
    <h4 class="text-lg font-semibold mb-4">Quick Links</h4>
    <ul class="space-y-2">
        <li><a href="#services" class="text-gray-400 hover:text-white transition-colors">Services</a></li>
```

To update footer links:
1. Find the appropriate footer column
2. Update the `href` attributes
3. Change the link text
4. Keep the existing classes for consistent styling

## Privacy and Terms Pages

### Adding Privacy and Terms Links
Located in the footer's legal section:

```html
<div>
    <h4 class="text-lg font-semibold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Terms of Service</a></li>
    </ul>
</div>
```

To link privacy and terms pages:
1. Create your privacy.html and terms.html files
2. Update the href attributes:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues and Solutions

1. **Broken Links**
   - Check that all href attributes start with "#" for internal links
   - Verify file names match exactly for external page links
   - Ensure all files are in the correct directory

2. **Styling Problems**
   - Don't remove existing Tailwind classes unless you're replacing them
   - Keep responsive classes (md:, lg:) to maintain mobile compatibility
   - Check for typos in class names

3. **Contact Form Issues**
   - Update the form action attribute when adding form functionality
   - Ensure all input fields have unique name attributes
   - Test the form submission process

### Need Help?
- Check the [Tailwind CSS documentation](https://tailwindcss.com/docs) for styling references
- Validate your HTML using [W3C Validator](https://validator.w3.org/)
- Test your page on multiple devices and browsers

Remember to always make a backup of your files before making significant changes.