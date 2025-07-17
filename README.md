# Miami Community Redevelopment Agency Website

A modern, responsive web application showcasing the Miami Community Redevelopment Agency's three main districts. Built with HTML, Tailwind CSS, and Alpine.js for a seamless user experience.

## Features

* **Responsive Design**: Optimized for desktop, tablet, and mobile devices
* **Dark Mode Toggle**: User-friendly dark/light theme switching with persistent preferences
* **Modern UI/UX**: Clean, professional interface using Tailwind CSS
* **Interactive Elements**: Smooth mobile menu with animations and hover effects
* **Accessibility**: WCAG compliant with proper ARIA attributes and keyboard navigation
* **Performance**: Optimized loading with efficient CSS and JavaScript

## Available Content

### OMNI CRA
* **Executive Director**: H. Bert Gonzalez
* **Address**: 1401 North Miami Ave. Upstairs, Miami, Florida 33136
* **Phone**: 305-679-6869
* **Email**: hugonzalez@miamigov.com
* **Website**: www.omnicra.com

### Southeast Overtown / Park West CRA
* **Executive Director**: James McQueen (Interim)
* **Address**: 819 NW 2nd Ave., 3rd Floor, Miami, Florida 33136
* **Phone**: 305-679-6800
* **Website**: www.seopwcra.com

### Midtown CRA
* **Executive Director**: Anthony Balzebre
* **Email**: abalzebre@miamigov.com

## Technology Stack

* **HTML5**: Semantic markup structure
* **Tailwind CSS**: Utility-first CSS framework for styling
* **Alpine.js**: Lightweight JavaScript framework for interactivity
* **Google Fonts**: Inter font family for typography
* **Font Awesome**: Icon library for contact information and UI elements
* **Dark Mode**: User preference toggle with localStorage persistence

## Getting Started

1. **Clone the repository**:  
   ```bash
   git clone https://github.com/edgarvelr/miami-cra.git  
   cd miami-cra
   ```

2. **Open the application**:  
   * Simply open `miamicra.html` in your web browser  
   * No build process or server setup required

3. **Development**:  
   * Edit `miamicra.html` to modify content or styling  
   * The application uses CDN links for all dependencies

## Browser Support

* Chrome
* Firefox
* Safari
* Edge
* Mobile browsers (iOS Safari, Chrome Mobile)

## Content Management Guide

### Updating Contact Information

To update contact information for any CRA district:

1. **Locate the CRA Card** - Find the appropriate card section in the HTML
2. **Update Information** - Modify the contact details within the card
3. **Test Links** - Ensure all email and website links work correctly

#### Example: Updating OMNI CRA Information

```html
<!-- ========================================
     OMNI CRA CARD
     ======================================== -->
<div id="omni" class="bg-white rounded-xl shadow-lg overflow-hidden transform hover:-translate-y-2 transition-transform duration-300 flex flex-col">
    <div class="bg-blue-700 p-6">
        <h3 class="text-2xl font-bold text-white">OMNI CRA</h3>
    </div>
    <div class="p-8 space-y-4 text-gray-700 flex-grow">
        <!-- Executive Director Information -->
        <p class="font-semibold text-lg text-gray-800">H. Bert Gonzalez<br><span class="font-normal text-base">Executive Director</span></p>
        <!-- Office Address -->
        <div class="flex items-start"><i class="fas fa-map-marker-alt w-5 text-blue-600 mt-1 mr-4 flex-shrink-0"></i><div>1401 North Miami Ave. Upstairs<br>Miami, Florida 33136</div></div>
        <!-- Phone Number -->
        <div class="flex items-start"><i class="fas fa-phone w-5 text-blue-600 mt-1 mr-4 flex-shrink-0"></i><div>305-679-6869</div></div>
        <!-- Email Address -->
        <div class="flex items-start"><i class="fas fa-envelope w-5 text-blue-600 mt-1 mr-4 flex-shrink-0"></i><div><a href="mailto:hugonzalez@miamigov.com" class="hover:underline">hugonzalez@miamigov.com</a></div></div>
        <!-- Website Link -->
        <div class="flex items-start"><i class="fas fa-globe w-5 text-blue-600 mt-1 mr-4 flex-shrink-0"></i><div><a href="http://www.omnicra.com" target="_blank" rel="noopener noreferrer" class="hover:underline">www.omnicra.com</a></div></div>
    </div>
</div>
```

### Adding New CRA Districts

To add a new CRA district:

1. **Add Card to Grid** - Insert a new card in the grid layout
2. **Update Navigation** - Add link to the header navigation
3. **Add Mobile Menu Item** - Include in mobile navigation menu
4. **Test Responsive Design** - Ensure it works on all screen sizes

#### Example: Adding a New CRA District

```html
<!-- ========================================
     NEW CRA DISTRICT CARD
     ======================================== -->
<div id="new-cra" class="bg-white rounded-xl shadow-lg overflow-hidden transform hover:-translate-y-2 transition-transform duration-300 flex flex-col">
    <div class="bg-blue-700 p-6">
        <h3 class="text-2xl font-bold text-white">New CRA District</h3>
    </div>
    <div class="p-8 space-y-4 text-gray-700 flex-grow">
        <!-- Executive Director Information -->
        <p class="font-semibold text-lg text-gray-800">Director Name<br><span class="font-normal text-base">Executive Director</span></p>
        <!-- Office Address -->
        <div class="flex items-start"><i class="fas fa-map-marker-alt w-5 text-blue-600 mt-1 mr-4 flex-shrink-0"></i><div>Address Line 1<br>City, State ZIP</div></div>
        <!-- Phone Number -->
        <div class="flex items-start"><i class="fas fa-phone w-5 text-blue-600 mt-1 mr-4 flex-shrink-0"></i><div>Phone Number</div></div>
        <!-- Email Address -->
        <div class="flex items-start"><i class="fas fa-envelope w-5 text-blue-600 mt-1 mr-4 flex-shrink-0"></i><div><a href="mailto:email@domain.com" class="hover:underline">email@domain.com</a></div></div>
        <!-- Website Link -->
        <div class="flex items-start"><i class="fas fa-globe w-5 text-blue-600 mt-1 mr-4 flex-shrink-0"></i><div><a href="http://www.website.com" target="_blank" rel="noopener noreferrer" class="hover:underline">www.website.com</a></div></div>
    </div>
</div>
```

### Updating Navigation Links

To update navigation links in the header:

1. **Desktop Navigation** - Update the desktop menu links
2. **Mobile Navigation** - Update the mobile menu links
3. **Test Both Menus** - Ensure links work in both desktop and mobile views

#### Example: Updating Navigation

```html
<!-- ========================================
     DESKTOP NAVIGATION MENU
     ======================================== -->
<nav class="hidden md:flex space-x-8">
    <!-- OMNI CRA - External link to official website -->
    <a href="http://www.omnicra.com" target="_blank" rel="noopener noreferrer" class="text-gray-700 hover:text-gray-900 dark:text-gray-300 dark:hover:text-white px-3 py-2 text-sm font-medium transition-colors">OMNI</a>
    <!-- Southeast Overtown/Park West CRA - External link to official website -->
    <a href="http://www.seopwcra.com/" target="_blank" rel="noopener noreferrer" class="text-gray-700 hover:text-gray-900 dark:text-gray-300 dark:hover:text-white px-3 py-2 text-sm font-medium transition-colors">SEOPW</a>
    <!-- Midtown CRA - Internal anchor link to card section -->
    <a href="#midtown" class="text-gray-700 hover:text-gray-900 dark:text-gray-300 dark:hover:text-white px-3 py-2 text-sm font-medium transition-colors">Midtown</a>
    <!-- New CRA District - Add new navigation item -->
    <a href="#new-cra" class="text-gray-700 hover:text-gray-900 dark:text-gray-300 dark:hover:text-white px-3 py-2 text-sm font-medium transition-colors">New CRA</a>
</nav>
```

### Modifying the Hero Section

To update the hero section content:

1. **Update Headline** - Modify the main "BUILDING" text
2. **Update Subtitle** - Change the "A Better Community" text
3. **Update Background** - Replace the background image URL

#### Example: Updating Hero Content

```html
<!-- ========================================
     HERO SECTION
     ======================================== -->
<section class="hero-bg text-white">
    <div class="bg-black bg-opacity-50">
        <div class="container mx-auto px-6 py-32 md:py-48 text-center">
            <!-- Main hero headline -->
            <h2 class="text-5xl md:text-7xl font-extrabold tracking-tight leading-tight">BUILDING</h2>
            <!-- Hero subtitle -->
            <p class="text-4xl md:text-6xl font-semibold mt-2">A Better Community</p>
        </div>
    </div>
</section>
```

### Customizing Dark Mode

To modify dark mode behavior:

1. **Update Toggle Function** - Modify the `toggleDarkMode()` function
2. **Customize Colors** - Update dark mode CSS variables
3. **Add New Elements** - Ensure new elements have dark mode styles

#### Example: Adding Dark Mode for New Elements

```css
/* Dark mode styles for new custom elements */
body.dark .custom-element {
    background-color: #374151 !important;
    color: #f9fafb !important;
}

body.dark .custom-element:hover {
    background-color: #4b5563 !important;
}
```

### Advanced Customization

#### Adding Custom Styling

To add custom styles for new content:

1. **Add CSS to the `<style>` section**:
```css
/* Custom styling for new content type */
.custom-content-link {
    /* Your custom styles here */
    background-color: #f3f4f6;
    border-radius: 0.5rem;
    padding: 1rem;
    transition: all 0.2s ease;
}

.custom-content-link:hover {
    background-color: #e5e7eb;
    transform: translateY(-2px);
}
```

2. **Apply the class to your HTML**:
```html
<div class="custom-content-link">
    <!-- Your custom content here -->
</div>
```

#### Modifying Animations

To change animation speeds or effects:

```html
<!-- Faster hover animations -->
<div class="transform hover:-translate-y-1 transition-transform duration-200">

<!-- Slower hover animations -->
<div class="transform hover:-translate-y-3 transition-transform duration-500">

<!-- Different easing functions -->
<div class="transform hover:-translate-y-2 transition-transform duration-300 ease-in-out">
```

#### Adding New Icons

To add custom icons to contact information:

```html
<!-- Custom icon example -->
<div class="flex items-start">
    <i class="fas fa-custom-icon w-5 text-blue-600 mt-1 mr-4 flex-shrink-0"></i>
    <div>Custom Information</div>
</div>
```

## Troubleshooting

### Common Issues

1. **Dark Mode Not Working**: Ensure Alpine.js is loaded and `toggleDarkMode()` function is defined
2. **Mobile Menu Not Opening**: Check that Alpine.js is loaded and `mobileMenuOpen` state is properly initialized
3. **Styling Issues**: Verify Tailwind CSS is loading properly from CDN
4. **Links Not Working**: Test URLs in browser and ensure they're accessible
5. **Logo Not Displaying**: Check that the logo file exists at `images/logo.png`

### Debugging Tips

* Use browser developer tools to check for JavaScript errors
* Verify that all Alpine.js attributes are properly formatted
* Test responsive behavior on different screen sizes
* Check that dark mode toggle works with new content
* Ensure all external links open in new tabs with proper security attributes

### Performance Optimization

* **Image Optimization**: Compress logo and background images
* **CDN Usage**: All external dependencies use CDN for faster loading
* **Minification**: Consider minifying CSS and JavaScript for production
* **Caching**: Implement browser caching for static assets

## Styling Modifications

### Dark Mode Customization

* Modify the `<style>` section in the HTML file
* Update Tailwind classes for layout changes
* Customize dark mode colors in the CSS variables
* Test dark mode on all new content additions

### Responsive Design

* Test on mobile, tablet, and desktop devices
* Use Tailwind's responsive prefixes (sm:, md:, lg:, xl:)
* Ensure content is readable on all screen sizes
* Verify mobile menu functionality on touch devices

### Color Scheme

* **Primary Blue**: #2563eb (used for links and accents)
* **Dark Blue**: #1e40af (used for card headers)
* **Gray Scale**: Various gray shades for text and backgrounds
* **Dark Mode**: Dark grays (#111827, #374151) for dark theme

## Browser Compatibility

### Supported Browsers

* **Chrome**: 90+
* **Firefox**: 88+
* **Safari**: 14+
* **Edge**: 90+
* **Mobile Safari**: iOS 14+
* **Chrome Mobile**: Android 8+

### Feature Support

* **CSS Grid**: Used for responsive card layout
* **CSS Flexbox**: Used for header and card content layout
* **CSS Transitions**: Used for hover effects and animations
* **localStorage**: Used for dark mode preference persistence
* **ES6+ JavaScript**: Used for Alpine.js functionality

## License

This project is maintained by the Miami Community Redevelopment Agency. All rights reserved.

## Contributing

For questions or suggestions regarding the Miami CRA website, please contact the appropriate department through the official City of Miami website.

## Contact

* **Website**: www.miamigov.com
* **Email**: webmaster@miamigov.com
* **ADA Support**: ADA Public Notice

---

_Last updated: January 2025_ 