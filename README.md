# SEA Invest Landing Page - Maintenance Guide

This guide will help you maintain and customize the SEA Invest landing page. It's written for beginners with no prior coding experience.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the main navigation and logo. To update:

1. **Logo Text**: Find this line and change "SEA Invest":
```html
<a href="/" class="text-2xl font-bold bg-gradient-to-r from-blue-500 to-teal-400 bg-clip-text text-transparent">SEA Invest</a>
```

2. **Navigation Items**: Locate these lines to modify menu items:
```html
<a href="#features" class="text-gray-300 hover:text-white transition-colors duration-300">Features</a>
<a href="#benefits" class="text-gray-300 hover:text-white transition-colors duration-300">Benefits</a>
<a href="#contact" class="text-gray-300 hover:text-white transition-colors duration-300">Contact</a>
```

### Hero Section
Update the main headline and subtext:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-8 leading-tight">Bridging Investment Opportunities in SEA</h1>
<p class="text-xl md:text-2xl text-gray-300 mb-12">Connecting Singapore VCs & Private Investment</p>
```

### Tailwind CSS Classes Explained
Common classes used throughout:
- `text-4xl`: Large text (increases with screen size)
- `md:text-5xl`: Applies different size on medium screens
- `font-bold`: Makes text bold
- `mb-8`: Adds margin bottom (spacing)
- `text-gray-300`: Sets text color
- `hover:text-white`: Changes text color on hover

## Managing Links

### External Links
Replace these placeholder URLs with your actual links:

1. **Get Started Button**:
```html
<!-- Find and replace this URL -->
<a href="https://www.wellnessdiscoveryhub.com" class="hidden md:block px-6 py-2 bg-gradient-to-r from-blue-600 to-teal-500 rounded-full">Get Started</a>
```

2. **Contact Email**:
```html
<!-- Update email address here -->
<p class="text-gray-400">djjoi@yahoo.com</p>
```

### Internal Navigation
Internal links use hashtags (#) to scroll to sections:
```html
<!-- These link to sections with matching IDs -->
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#contact">Contact</a>
```

To ensure proper linking:
1. Check that section IDs match exactly
2. Maintain the same spelling and case
3. Remove any spaces in IDs

## Adding Privacy and Terms Pages

### Step 1: Create New Pages
Create two new files in your project folder:
- `privacy.html`
- `terms.html`

### Step 2: Update Footer Links
Replace these placeholder links:
```html
<!-- Before -->
<li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>

<!-- After -->
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

### Step 3: Style Consistency
Copy these classes to maintain consistent styling:
```html
class="text-gray-400 hover:text-white transition-colors duration-300"
```

## Troubleshooting

Common issues and solutions:

1. **Links Not Working**
   - Check for typos in href attributes
   - Verify file names match exactly
   - Ensure files are in the same directory

2. **Styles Not Applying**
   - Confirm Tailwind CSS is properly linked
   - Check for typos in class names
   - Verify class combinations are valid

3. **Responsive Design Issues**
   - Test different screen sizes
   - Check for proper `md:` and `lg:` prefixes
   - Ensure viewport meta tag is present

Need help? Contact your developer or refer to:
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [HTML MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/HTML)

Remember to always test changes in multiple browsers and screen sizes before publishing.