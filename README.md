# GlucoTonic Landing Page Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the GlucoTonic landing page. Whether you're new to web development or need a quick reference, you'll find step-by-step guidance for common maintenance tasks.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Text Content Updates

#### Header Section
```html
<div class="text-2xl font-bold text-indigo-600">GlucoTonic</div>
```
To update the logo text:
1. Locate this div in the header section
2. Replace "GlucoTonic" with your desired text
3. Maintain the surrounding div tags

#### Hero Section
```html
<h1 class="text-4xl md:text-6xl font-bold mb-6">GlucoTonic Reviews</h1>
<p class="text-xl md:text-2xl mb-8">The #1 Rated Blood Sugar Formula...</p>
```
To modify hero content:
1. Find the hero section (first full-screen section)
2. Update text between the `<h1>` tags for the main heading
3. Modify text between the `<p>` tags for the subheading

### Tailwind CSS Classes Explained

#### Responsive Design Classes
- `md:` prefix indicates styles apply only on medium screens and larger
- Example: `text-4xl md:text-6xl` means:
  - `text-4xl` (smaller text) on mobile
  - `text-6xl` (larger text) on medium screens and up

#### Common Class Patterns
```html
<div class="bg-white rounded-xl p-8 shadow-lg hover:shadow-xl transition-shadow duration-300">
```
Breaking down the classes:
- `bg-white`: White background
- `rounded-xl`: Rounded corners
- `p-8`: Padding on all sides
- `shadow-lg`: Large shadow effect
- `hover:shadow-xl`: Larger shadow on hover
- `transition-shadow duration-300`: Smooth shadow transition

## Managing Links

### Navigation Menu Links
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
</div>
```
To update navigation links:
1. Locate the navigation div in the header
2. Modify `href` attributes to point to new sections
3. Update link text between `<a>` tags

### Call-to-Action (CTA) Links
```html
<a href="https://getglucotonic.com/d/order-now.php#aff=MichaelMica" class="bg-indigo-600 text-white px-6 py-2 rounded-full">Buy Now</a>
```
To update CTA links:
1. Find all instances of the order URL
2. Replace with your new URL
3. Keep the existing classes for consistent styling

### Social Media Links
```html
<div class="flex space-x-4">
    <a href="#" class="text-gray-400 hover:text-white">
        <i class="fab fa-facebook"></i>
    </a>
    <!-- Similar structure for Twitter and Instagram -->
</div>
```
To add social media links:
1. Locate the social media section in the footer
2. Replace `#` with your social media URLs
3. Maintain the icon classes (`fab fa-facebook`, etc.)

## Adding Privacy and Terms Pages

### Footer Policy Links
```html
<ul class="space-y-4 text-gray-400">
    <li>Privacy Policy</li>
    <li>Terms of Service</li>
    <li>Refund Policy</li>
</ul>
```
To link policy pages:
1. Update the list items to include links:
```html
<ul class="space-y-4 text-gray-400">
    <li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
    <li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    <li><a href="refund.html" class="hover:text-white transition-colors duration-300">Refund Policy</a></li>
</ul>
```

## Troubleshooting

### Common Issues and Solutions

1. **Broken Images**
   - Check image URLs in the `src` attributes
   - Ensure images exist at the specified paths
   - Verify image formats are supported (jpg, png, etc.)

2. **Responsive Design Issues**
   - Check `md:` prefixed classes
   - Test on different screen sizes
   - Ensure viewport meta tag is present:
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

3. **Link Issues**
   - Verify all `href` attributes
   - Test internal links (starting with #)
   - Confirm external URLs are complete and correct

### Need Help?
- Check the [Tailwind CSS documentation](https://tailwindcss.com/docs)
- Validate HTML at [W3C Validator](https://validator.w3.org/)
- Test responsive design using browser developer tools

Remember to always backup your files before making changes, and test thoroughly across different devices and browsers.