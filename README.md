# Oakland Accident Care Landing Page - Maintenance & Customization Guide

## Table of Contents
1. [Overview](#overview)
2. [Updating Text and Content](#updating-text-and-content)
3. [Working with Tailwind CSS Classes](#working-with-tailwind-css-classes)
4. [Fixing Broken Links](#fixing-broken-links)
5. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
6. [Troubleshooting Guide](#troubleshooting-guide)
7. [Best Practices](#best-practices)

---

## Overview

This landing page is built using:
- **HTML5** - The structure and content
- **Tailwind CSS** - A utility-first CSS framework for styling
- **Font Awesome Icons** - For visual icons throughout the page
- **Vanilla JavaScript** - For interactive features like mobile menu and FAQ accordion

The page is organized into clear sections that you can modify independently:
- Header/Navigation
- Hero Section
- Features Section
- Benefits Section
- About Us Section
- Call-to-Action Section
- Testimonials Section
- FAQ Section
- Contact Section
- Footer

---

## Updating Text and Content

### Understanding the File Structure

Before making changes, locate your `index.html` file. This is the main file you'll be editing. Open it with a text editor like:
- **Visual Studio Code** (recommended for beginners)
- **Sublime Text**
- **Notepad++**
- Or any basic text editor

### How to Find and Replace Text

**Step 1: Open the file in your text editor**

**Step 2: Use Find & Replace (Ctrl+H on Windows, Cmd+Option+F on Mac)**

This is the fastest way to update multiple instances of text throughout the page.

---

### Section-by-Section Text Updates

#### 1. **Header/Navigation Bar**

**Location:** Lines 51-75 (approximately)

```html
<!-- CURRENT CODE -->
<a href="#" class="text-2xl font-bold text-gray-900">
    <i class="fas fa-clinic-medical text-blue-600 mr-2"></i>
    <span class="hidden sm:inline">Oakland Accident Care</span>
    <span class="sm:hidden">OAC</span>
</a>
```

**To change the business name:**
1. Find: `Oakland Accident Care`
2. Replace with: Your business name
3. Update the short version (OAC) if needed

**To change the logo icon:**
Replace `fa-clinic-medical` with another Font Awesome icon from [fontawesome.com](https://fontawesome.com)

Common alternatives:
- `fa-heart` - Heart icon
- `fa-shield-heart` - Protected health icon
- `fa-stethoscope` - Medical stethoscope

---

#### 2. **Hero Section (Main Headline)**

**Location:** Lines 116-135

```html
<!-- CURRENT CODE -->
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight tracking-tight mb-6">
    Same Day Chiropractor in Oakland, CA
</h1>
<p class="text-xl md:text-2xl text-gray-700 mb-4 font-semibold">
    Oakland Car Accident Chiropractor
</p>
```

**To update the main headline:**
1. Find the text: `Same Day Chiropractor in Oakland, CA`
2. Replace with your headline
3. Keep the HTML tags (`<h1>`, `</h1>`) intact

**To update the subheading:**
1. Find: `Oakland Car Accident Chiropractor`
2. Replace with your subheading

**Important:** Do NOT delete or modify the class names (like `text-4xl`, `font-bold`, etc.). These control the styling and responsive design.

---

#### 3. **Hero Section Description**

**Location:** Lines 136-141

```html
<!-- CURRENT CODE -->
<p class="text-lg md:text-xl text-gray-600 mb-10 max-w-2xl mx-auto leading-relaxed">
    Get professional chiropractic care the same day you need it. Zero payment required upfront. 
    Our Spanish-speaking staff is ready to help you recover from your car accident injuries with 
    compassionate, expert care.
</p>
```

**To update this text:**
1. Select all the text between `>` and `</p>`
2. Replace with your description
3. Keep the paragraph tags and class names

---

#### 4. **Features Section**

**Location:** Lines 169-220

The Features section has three cards. Each card follows this pattern:

```html
<!-- FEATURE CARD TEMPLATE -->
<div class="feature-card bg-white border border-gray-200 rounded-xl p-8 hover-lift">
    <div class="bg-blue-100 w-16 h-16 rounded-lg flex items-center justify-center mb-6">
        <i class="fas fa-clock text-blue-600 text-2xl"></i>
    </div>
    <h3 class="text-xl font-bold text-gray-900 mb-3">Same-Day Appointments</h3>
    <p class="text-gray-600 leading-relaxed">
        Don't wait weeks for relief. We prioritize urgent...
    </p>
</div>
```

**To update Feature 1 (Same-Day Appointments):**

1. **Change the title:**
   - Find: `Same-Day Appointments`
   - Replace with your feature title

2. **Change the description:**
   - Find the paragraph starting with: `Don't wait weeks for relief...`
   - Replace with your description

3. **Change the icon:**
   - Find: `fa-clock`
   - Replace with another Font Awesome icon (e.g., `fa-bolt`, `fa-rocket`)

4. **Change the background color:**
   - Find: `bg-blue-100` and `text-blue-600`
   - Replace both with matching colors:
     - Blue: `bg-blue-100` / `text-blue-600`
     - Green: `bg-green-100` / `text-green-600`
     - Purple: `bg-purple-100` / `text-purple-600`
     - Orange: `bg-orange-100` / `text-orange-600`

**Repeat for Features 2 and 3** (lines 200-220)

---

#### 5. **Benefits Section**

**Location:** Lines 245-310

This section has four benefit items with a different layout:

```html
<!-- BENEFIT ITEM TEMPLATE -->
<div class="flex gap-6 items-start">
    <div class="flex-shrink-0">
        <div class="flex items-center justify-center h-12 w-12 rounded-md bg-blue-600 text-white">
            <i class="fas fa-check-circle text-lg"></i>
        </div>
    </div>
    <div>
        <h3 class="text-xl font-bold text-gray-900 mb-2">Same-Day Care</h3>
        <p class="text-gray-600 leading-relaxed">
            Don't suffer through the weekend...
        </p>
    </div>
</div>
```

**To update each benefit:**

1. **Change the title:**
   - Find: `Same-Day Care`
   - Replace with your benefit title

2. **Change the description:**
   - Find the paragraph and replace the text

3. **Change the background color:**
   - Find: `bg-blue-600`
   - Replace with:
     - `bg-green-600` (green)
     - `bg-purple-600` (purple)
     - `bg-orange-600` (orange)

---

#### 6. **About Us Section**

**Location:** Lines 324-345

```html
<!-- ABOUT SECTION -->
<h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-6 tracking-tight">
    About Oakland Accident Care
</h2>
<p class="text-lg text-gray-600 leading-relaxed mb-6">
    Founded in 2015, Oakland Accident Care emerged from a simple mission...
</p>
```

**To update:**
1. Change the heading to your company name
2. Replace the paragraphs with your company's story

**To change the image:**
- Find: `https://images.unsplash.com/photo-1631217b9201-d5ffd007d93e?w=600&h=400&fit=crop`
- Replace with your image URL
- The image should be at least 600x400 pixels

---

#### 7. **Testimonials Section**

**Location:** Lines 413-510

Each testimonial follows this structure:

```html
<!-- TESTIMONIAL TEMPLATE -->
<div class="testimonial-card bg-white rounded-xl shadow-md p-8 border border-gray-200">
    <div class="flex items-center mb-4">
        <i class="fas fa-star star"></i>
        <i class="fas fa-star star"></i>
        <i class="fas fa-star star"></i>
        <i class="fas fa-star star"></i>
        <i class="fas fa-star star"></i>
    </div>
    <p class="text-gray-700 leading-relaxed mb-6">
        "I was hit by another car at a red light..."
    </p>
    <div>
        <p class="font-bold text-gray-900">Maria Santos</p>
        <p class="text-gray-600 text-sm">Oakland, CA</p>
    </div>
</div>
```

**To update a testimonial:**

1. **Change the review text:**
   - Find the quoted text
   - Replace with your customer's review
   - Keep the quotation marks

2. **Change the customer name:**
   - Find: `Maria Santos`
   - Replace with the customer's name

3. **Change the location/title:**
   - Find: `Oakland, CA`
   - Replace with customer's title or location

4. **Adjust star rating:**
   - To remove a star: Delete one `<i class="fas fa-star star"></i>` line
   - To add a star: Duplicate one `<i class="fas fa-star star"></i>` line

---

#### 8. **FAQ Section**

**Location:** Lines 535-625

Each FAQ item follows this pattern:

```html
<!-- FAQ ITEM TEMPLATE -->
<div class="faq-item border border-gray-200 rounded-lg overflow-hidden">
    <button class="faq-question w-full px-6 py-4 flex justify-between items-center bg-gray-50 hover:bg-gray-100 transition-colors duration-300">
        <span class="text-lg font-semibold text-gray-900 text-left">
            How quickly can I get an appointment?
        </span>
        <i class="fas fa-chevron-down faq-icon text-gray-600"></i>
    </button>
    <div class="faq-answer hidden px-6 py-4 bg-white border-t border-gray-200">
        <p class="text-gray-700 leading-relaxed">
            We specialize in same-day appointments...
        </p>
    </div>
</div>
```

**To update a FAQ item:**

1. **Change the question:**
   - Find: `How quickly can I get an appointment?`
   - Replace with your question

2. **Change the answer:**
   - Find the paragraph in the `faq-answer` div
   - Replace with your answer

---

#### 9. **Contact Section**

**Location:** Lines 637-705

```html
<!-- CONTACT INFO -->
<a href="mailto:frontdesk@oaklandaccidentcare.com" class="text-blue-600 hover:text-blue-700 transition-colors duration-300">
    frontdesk@oaklandaccidentcare.com
</a>
```

**To update contact information:**

1. **Change email:**
   - Find: `frontdesk@oaklandaccidentcare.com`
   - Replace with your email address
   - Update in TWO places (href and display text)

2. **Change location:**
   - Find: `Oakland, California`
   - Replace with your location

---

#### 10. **Footer Section**

**Location:** Lines 720-800

```html
<!-- FOOTER DESCRIPTION -->
<p class="text-gray-400 leading-relaxed">
    Professional chiropractic care for car accident injuries in Oakland, CA...
</p>
```

**To update:**
1. Replace the description text
2. Update company name in footer
3. Update contact email

---

## Working with Tailwind CSS Classes

### What is Tailwind CSS?

Tailwind CSS is a "utility-first" framework. Instead of writing custom CSS, you use pre-made class names that control styling. Think of them as building blocks.

### Key Tailwind Classes Used in This Landing Page

#### **Text Sizing**

```html
<!-- EXAMPLE -->
<h1 class="text-4xl md:text-5xl lg:text-6xl">
    Headline
</h1>
```

- `text-4xl` - Extra large (mobile)
- `md:text-5xl` - Larger on medium screens
- `lg:text-6xl` - Largest on large screens

**Common text sizes:**
- `text-sm` - Small
- `text-base` - Normal
- `text-lg` - Large
- `text-xl` - Extra large
- `text-2xl`, `text-3xl`, `text-4xl`, `text-5xl`, `text-6xl` - Progressively larger

#### **Colors**

```html
<!-- TEXT COLOR EXAMPLES -->
<p class="text-gray-900">Dark text</p>
<p class="text-gray-600">Medium text</p>
<p class="text-blue-600">Blue text</p>
```

**Color families available:**
- Gray: `text-gray-900`, `text-gray-700`, `text-gray-600`, `text-gray-400`
- Blue: `text-blue-600`, `text-blue-700`
- Green: `text-green-600`
- Purple: `text-purple-600`
- Orange: `text-orange-600`

**Background colors:**
```html
<div class="bg-blue-600">Blue background</div>
<div class="bg-gray-50">Light gray background</div>
<div class="bg-blue-100">Very light blue</div>
```

#### **Spacing (Padding & Margins)**

```html
<!-- PADDING (inside) -->
<div class="p-8">Padding all sides</div>
<div class="px-4 py-2">Padding horizontal and vertical</div>

<!-- MARGINS (outside) -->
<div class="mb-6">Margin bottom</div>
<div class="mt-4">Margin top</div>
```

**Spacing scale:** 0, 1, 2, 3, 4, 6, 8, 10, 12, 16, 20, 24, 32, etc.

#### **Responsive Design**

```html
<!-- EXAMPLE -->
<div class="hidden md:flex">
    This is hidden on mobile, shows on medium+ screens
</div>
```

**Breakpoint prefixes:**
- `sm:` - Small screens (640px+)
- `md:` - Medium screens (768px+)
- `lg:` - Large screens (1024px+)
- `xl:` - Extra large screens (1280px+)

#### **Width & Height**

```html
<div class="w-16 h-16">Square box</div>
<div class="w-full">Full width</div>
<div class="max-w-7xl">Maximum width container</div>
```

#### **Borders & Shadows**

```html
<div class="border border-gray-200">Light border</div>
<div class="rounded-lg">Rounded corners</div>
<div class="shadow-lg">Large shadow</div>
<div class="shadow-md">Medium shadow</div>
```

### How to Modify Tailwind Classes While Maintaining Responsive Design

#### **Example: Making the Hero Headline Smaller**

**Current code:**
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900">
    Same Day Chiropractor in Oakland, CA
</h1>
```

**To make it smaller:**
```html
<h1 class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-900">
    Same Day Chiropractor in Oakland, CA
</h1>
```

**What changed:**
- `text-4xl` → `text-3xl` (smaller on mobile)
- `md:text-5xl` → `md:text-4xl` (smaller on tablets)
- `lg:text-6xl` → `lg:text-5xl` (smaller on desktops)

#### **Example: Changing Button Color**

**Current code:**
```html
<a href="https://oaklandaccidentcare.com" class="bg-blue-600 text-white px-8 py-4 rounded-lg">
    Start Your Recovery Today
</a>
```

**To change to green:**
```html
<a href="https://oaklandaccidentcare.com" class="bg-green-600 text-white px-8 py-4 rounded-lg">
    Start Your Recovery Today
</a>
```

**To change to purple:**
```html
<a href="https://oaklandaccidentcare.com" class="bg-purple-600 text-white px-8 py-4 rounded-lg">
    Start Your Recovery Today
</a>
```

#### **Example: Adjusting Spacing**

**Current code:**
```html
<div class="py-16 md:py-24 bg-white">
    Section content
</div>
```

**To add more space:**
```html
<div class="py-20 md:py-32 bg-white">
    Section content
</div>
```

**To add less space:**
```html
<div class="py-12 md:py-16 bg-white">
    Section content
</div>
```

### Important: Do NOT Delete Class Names

**WRONG:**
```html
<!-- BAD - Removes all styling -->
<h1>Same Day Chiropractor in Oakland, CA</h1>
```

**CORRECT:**
```html
<!-- GOOD - Keeps styling -->
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900">
    Same Day Chiropractor in Oakland, CA
</h1>
```

### Testing Responsive Design

After making changes, test your page on different screen sizes:

1. **Desktop:** View normally in your browser
2. **Tablet:** Press F12 (or Cmd+Option+I on Mac), click the device icon, select "iPad"
3. **Mobile:** In developer tools, select "iPhone 12" or similar

---

## Fixing Broken Links

### Understanding Links in HTML

A link in HTML looks like this:

```html
<a href="DESTINATION">Link Text</a>
```

- `href` = Where the link goes
- Link Text = What the user sees and clicks

### All Current Links in This Landing Page

#### **Navigation Menu Links (Header)**

**Location:** Lines 58-65

```html
<!-- DESKTOP MENU -->
<a href="#features" class="...">Features</a>
<a href="#benefits" class="...">Benefits</a>
<a href="#testimonials" class="...">Testimonials</a>
<a href="#faq" class="...">FAQ</a>
<a href="https://oaklandaccidentcare.com" class="...">Get Started</a>
```

**Mobile Menu Links:** Lines 72-77 (identical links)

#### **Hero Section Buttons**

**Location:** Lines 142-149

```html
<a href="https://oaklandaccidentcare.com" class="...">
    Start Your Recovery Today
</a>
<a href="#contact" class="...">
    Learn More
</a>
```

#### **CTA Section Button**

**Location:** Line 363

```html
<a href="https://oaklandaccidentcare.com" class="...">
    Schedule Your Appointment Now
</a>
```

#### **Contact Section Buttons**

**Location:** Lines 702-703

```html
<a href="mailto:frontdesk@oaklandaccidentcare.com" class="...">
    frontdesk@oaklandaccidentcare.com
</a>

<a href="https://oaklandaccidentcare.com" class="...">
    Schedule Now
</a>
```

#### **Footer Links**

**Location:** Lines 738-749

```html
<!-- QUICK LINKS -->
<a href="#features" class="...">Features</a>
<a href="#benefits" class="...">Benefits</a>
<a href="#testimonials" class="...">Testimonials</a>
<a href="#faq" class="...">FAQ</a>

<!-- LEGAL LINKS -->
<a href="privacy.html" class="...">Privacy Policy</a>
<a href="terms.html" class="...">Terms of Service</a>
<a href="blog.html" class="...">Blog</a>

<!-- CONTACT LINKS -->
<a href="mailto:frontdesk@oaklandaccidentcare.com" class="...">
    frontdesk@oaklandaccidentcare.com
</a>
```

### Step-by-Step: Fixing Each Link

#### **1. Update the "Get Started" Button**

This button appears multiple times and links to your main website.

**Find all instances:**
- Line 65 (Desktop menu)
- Line 77 (Mobile menu)
- Line 143 (Hero section)
- Line 362 (CTA section)
- Line 702 (Contact section)

**Current:**
```html
href="https://oaklandaccidentcare.com"
```

**To update:**
1. Replace with your actual website URL
2. Example: `href="https://www.yourwebsite.com"`
3. Or to an appointment booking page: `href="https://www.yourwebsite.com/book"`

**How to find and replace all at once:**
1. Press Ctrl+H (Windows) or Cmd+Option+F (Mac)
2. Find: `https://oaklandaccidentcare.com`
3. Replace with: Your URL
4. Click "Replace All"

#### **2. Update Internal Navigation Links**

These links jump to sections on the same page (using the `#` symbol).

**Current links:**
- `#features` - Points to Features section
- `#benefits` - Points to Benefits section
- `#testimonials` - Points to Testimonials section
- `#faq` - Points to FAQ section
- `#contact` - Points to Contact section

**These should work as-is.** The `#` symbol tells the browser to find a section with that ID.

**If you rename a section, update the ID:**

Example: If you want to rename "Benefits" to "Why Us"

**Step 1:** Find the Benefits section heading (around line 235)
```html
<section id="benefits" class="...">
```

**Step 2:** Change the ID
```html
<section id="why-us" class="...">
```

**Step 3:** Update all links pointing to it
- Find: `href="#benefits"`
- Replace with: `href="#why-us"`

#### **3. Update Email Link**

**Current:**
```html
<a href="mailto:frontdesk@oaklandaccidentcare.com">
    frontdesk@oaklandaccidentcare.com
</a>
```

**To update:**
1. Replace `frontdesk@oaklandaccidentcare.com` with your email
2. Update in BOTH places (the href AND the display text)

**Example:**
```html
<a href="mailto:contact@yourcompany.com">
    contact@yourcompany.com
</a>
```

#### **4. Fix Social Media Links**

**Location:** Lines 769-783

**Current:**
```html
<a href="#" class="...">
    <i class="fab fa-facebook-f text-xl"></i>
</a>
```

**To update:**
Replace `#` with your social media URL:

```html
<!-- Facebook -->
<a href="https://www.facebook.com/yourpage" class="...">
    <i class="fab fa-facebook-f text-xl"></i>
</a>

<!-- Twitter -->
<a href="https://www.twitter.com/yourhandle" class="...">
    <i class="fab fa-twitter text-xl"></i>
</a>

<!-- Instagram -->
<a href="https://www.instagram.com/yourhandle" class="...">
    <i class="fab fa-instagram text-xl"></i>
</a>

<!-- LinkedIn -->
<a href="https://www.linkedin.com/company/yourcompany" class="...">
    <i class="fab fa-linkedin-in text-xl"></i>
</a>
```

---

## Linking Privacy and Terms Pages

### Understanding the Current Setup

The footer currently has links to three pages:
- `privacy.html` - Privacy Policy
- `terms.html` - Terms of Service
- `blog.html` - Blog

These are placeholder links. You need to:
1. Create these pages
2. Ensure they're in the same folder as `index.html`
3. Verify the links work correctly

### Step 1: Create the Privacy Policy Page

**Create a new file:**
1. In your text editor, select File → New File
2. Save it as `privacy.html` in the same folder as `index.html`

**Paste this template:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy for Oakland Accident Care">
    <title>Privacy Policy | Oakland Accident Care</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body class="bg-white text-gray-900">
    <!-- Header -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <a href="index.html" class="text-2xl font-bold text-gray-900">
                    <i class="fas fa-clinic-medical text-blue-600 mr-2"></i>
                    <span class="hidden sm:inline">Oakland Accident Care</span>
                    <span class="sm:hidden">OAC</span>
                </a>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-16 md:py-24 bg-white">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-4xl font-bold text-gray-900 mb-8">Privacy Policy</h1>
            
            <div class="prose prose-lg text-gray-700">
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Introduction</h2>
                <p>
                    Oakland Accident Care ("we," "us," "our," or "Company") is committed to protecting your privacy. 
                    This Privacy Policy explains how we collect, use, disclose, and otherwise process your personal information 
                    in connection with our websites, mobile applications, and services.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Information We Collect</h2>
                <p>
                    We collect information you provide directly to us, such as when you contact us for an appointment, 
                    fill out forms, or communicate with us via email or phone. This may include your name, contact information, 
                    medical history, and insurance details.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">How We Use Your Information</h2>
                <p>
                    We use the information we collect to provide, maintain, and improve our services, process appointments, 
                    communicate with you, and comply with legal obligations.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Contact Us</h2>
                <p>
                    If you have questions about this Privacy Policy, please contact us at 
                    <a href="mailto:frontdesk@oaklandaccidentcare.com" class="text-blue-600 hover:text-blue-700">
                        frontdesk@oaklandaccidentcare.com
                    </a>
                </p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p>&copy; 2025 Oakland Accident Care. All rights reserved.</p>
            <div class="mt-4">
                <a href="index.html" class="text-gray-400 hover:text-blue-500 mr-4">Home</a>
                <a href="privacy.html" class="text-gray-400 hover:text-blue-500 mr-4">Privacy</a>
                <a href="terms.html" class="text-gray-400 hover:text-blue-500">Terms</a>
            </div>
        </div>
    </footer>
</body>
</html>
```

### Step 2: Create the Terms of Service Page

**Create a new file:**
1. File → New File
2. Save as `terms.html`

**Paste this template:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service for Oakland Accident Care">
    <title>Terms of Service | Oakland Accident Care</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body class="bg-white text-gray-900">
    <!-- Header -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <a href="index.html" class="text-2xl font-bold text-gray-900">
                    <i class="fas fa-clinic-medical text-blue-600 mr-2"></i>
                    <span class="hidden sm:inline">Oakland Accident Care</span>
                    <span class="sm:hidden">OAC</span>
                </a>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-16 md:py-24 bg-white">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-4xl font-bold text-gray-900 mb-8">Terms of Service</h1>
            
            <div class="prose prose-lg text-gray-700">
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Agreement to Terms</h2>
                <p>
                    By accessing and using this website and services provided by Oakland Accident Care, 
                    you accept and agree to be bound by the terms and provision of this agreement.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Use License</h2>
                <p>
                    Permission is granted to temporarily download one copy of the materials (information or software) 
                    on Oakland Accident Care's website for personal, non-commercial transitory viewing only. 
                    This is the grant of a license, not a transfer of title.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Disclaimer</h2>
                <p>
                    The materials on Oakland Accident Care's website are provided on an 'as is' basis. 
                    Oakland Accident Care makes no warranties, expressed or implied, and hereby disclaims and negates 
                    all other warranties including, without limitation, implied warranties or conditions of merchantability, 
                    fitness for a particular purpose, or non-infringement of intellectual property or other violation of rights.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Limitations</h2>
                <p>
                    In no event shall Oakland Accident Care or its suppliers be liable for any damages 
                    (including, without limitation, damages for loss of data or profit, or due to business interruption) 
                    arising out of the use or inability to use the materials on Oakland Accident Care's website.
                </p>

                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Contact Us</h2>
                <p>
                    If you have any questions about these Terms of Service, please contact us at 
                    <a href="mailto:frontdesk@oaklandaccidentcare.com" class="text-blue-600 hover:text-blue-700">
                        frontdesk@oaklandaccidentcare.com
                    </a>
                </p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p>&copy; 2025 Oakland Accident Care. All rights reserved.</p>
            <div class="mt-4">
                <a href="index.html" class="text-gray-400 hover:text-blue-500 mr-4">Home</a>
                <a href="privacy.html" class="text-gray-400 hover:text-blue-500 mr-4">Privacy</a>
                <a href="terms.html" class="text-gray-400 hover:text-blue-500">Terms</a>
            </div>
        </div>
    </footer>
</body>
</html>
```

### Step 3: Create the Blog Page (Optional)

**Create a new file:**
1. File → New File
2. Save as `blog.html`

**Paste this template:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Blog | Oakland Accident Care">
    <title>Blog | Oakland Accident Care</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body class="bg-white text-gray-900">
    <!-- Header -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <a href="index.html" class="text-2xl font-bold text-gray-900">
                    <i class="fas fa-clinic-medical text-blue-600 mr-2"></i>
                    <span class="hidden sm:inline">Oakland Accident Care</span>
                    <span class="sm:hidden">OAC</span>
                </a>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-16 md:py-24 bg-white">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-4xl font-bold text-gray-900 mb-8">Blog</h1>
            
            <div class="bg-gray-50 rounded-lg p-8 text-center">
                <p class="text-lg text-gray-600 mb-4">
                    Welcome to the Oakland Accident Care Blog. Here you'll find helpful articles about 
                    car accident injuries, chiropractic care, and recovery tips.
                </p>
                <p class="text-gray-600">
                    Check back soon for our latest articles and insights.
                </p>
            </div>

            <!-- Blog Post Example (Optional) -->
            <div class="mt-12 border-b border-gray-200 pb-8">
                <h2 class="text-2xl font-bold text-gray-900 mb-2">
                    Understanding Whiplash: Symptoms and Treatment
                </h2>
                <p class="text-gray-600 text-sm mb-4">Published on January 15, 2025</p>
                <p class="text-gray-700 leading-relaxed">
                    Whiplash is one of the most common injuries sustained in car accidents. 
                    In this article, we'll explore what whiplash is, how to recognize its symptoms, 
                    and what treatment options are available...
                </p>
                <a href="#" class="text-blue-600 hover:text-blue-700 font-semibold mt-4 inline-block">
                    Read More →
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p>&copy; 2025 Oakland Accident Care. All rights reserved.</p>
            <div class="mt-4">
                <a href="index.html" class="text-gray-400 hover:text-blue-500 mr-4">Home</a>
                <a href="privacy.html" class="text-gray-400 hover:text-blue-500 mr-4">Privacy</a>
                <a href="terms.html" class="text-gray-400 hover:text-blue-500">Terms</a>
            </div>
        </div>
    </footer>
</body>
</html>
```

### Step 4: Verify File Structure

Your folder should now look like this:

```
your-project-folder/
├── index.html (main landing page)
├── privacy.html (privacy policy)
├── terms.html (terms of service)
└── blog.html (blog page)
```

### Step 5: Test the Links

1. **In your index.html footer**, verify these links are present (they should be):

```html
<a href="privacy.html" class="...">Privacy Policy</a>
<a href="terms.html" class="...">Terms of Service</a>
<a href="blog.html" class="...">Blog</a>
```

2. **Open index.html in your browser**

3. **Scroll to the footer**

4. **Click each link to verify it works:**
   - "Privacy Policy" should open privacy.html
   - "Terms of Service" should open terms.html
   - "Blog" should open blog.html

### Step 6: Add Return Links to Policy Pages

The policy pages include a link back to the home page. To ensure consistency, add a footer navigation to each policy page:

**In privacy.html and terms.html, the footer already includes:**

```html
<a href="index.html" class="text-gray-400 hover:text-blue-500 mr-4">Home</a>
```

This allows users to navigate back to the main page.

### Customizing the Policy Pages

**To add your own content to privacy.html:**

1. Open `privacy.html`
2. Find the section that says:
   ```html
   <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">Introduction</h2>
   <p>Oakland Accident Care ("we," "us," "our," or "Company")...</p>
   ```
3. Replace the text with your actual privacy policy
4. Add or remove sections as needed

**Same process for terms.html and blog.html**

---

## Troubleshooting Guide

### Problem: Links Don't Work

**Symptom:** Clicking a link does nothing or shows a 404 error

**Solution:**

1. **Check file names are spelled correctly:**
   - Should be: `privacy.html` (not `Privacy.html` or `privacypolicy.html`)
   - Should be: `terms.html` (not `Terms.html` or `terms-of-service.html`)

2. **Verify files are in the same folder as index.html**

3. **Check href attribute spelling:**
   ```html
   <!-- CORRECT -->
   <a href="privacy.html">Privacy</a>
   
   <!-- WRONG -->
   <a href="Privacy.html">Privacy</a>
   <a href="./privacy.html">Privacy</a> <!-- This might work, but not necessary -->
   ```

4. **For external links, ensure full URL:**
   ```html
   <!-- CORRECT for external links -->
   <a href="https://www.yourwebsite.com">Website</a>
   
   <!-- WRONG - missing https:// -->
   <a href="www.yourwebsite.com">Website</a>
   ```

### Problem: Styling Looks Broken

**Symptom:** Page looks unstyled or formatting is off

**Solution:**

1. **Check that you didn't delete Tailwind CSS link:**
   ```html
   <!-- This line should be in the <head> -->
   <script src="https://cdn.tailwindcss.com"></script>
   ```

2. **Verify Font Awesome link is present:**
   ```html
   <!-- This line should also be in the <head> -->
   <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
   ```

3. **Check that class names weren't accidentally deleted:**
   - Don't delete anything in the `class="..."` attribute
   - Only modify the text content between tags

### Problem: Text Looks Wrong on Mobile

**Symptom:** Text is too small or too large on phone/tablet

**Solution:**

1. **Don't remove responsive classes:**
   ```html
   <!-- CORRECT - responsive -->
   <h1 class="text-4xl md:text-5xl lg:text-6xl">Heading</h1>
   
   <!-- WRONG - only one size -->
   <h1 class="text-4xl">Heading</h1>
   ```

2. **Test on mobile:**
   - Press F12 in browser
   - Click device icon
   - Select "iPhone 12" or similar
   - Verify text is readable at different sizes

### Problem: Images Not Showing

**Symptom:** Image placeholder or broken image icon appears

**Solution:**

1. **Check image URL is valid:**
   ```html
   <!-- CORRECT -->
   <img src="https://images.unsplash.com/photo-1631217b9201-d5ffd007d93e?w=600&h=400&fit=crop" alt="Clinic">
   
   <!-- WRONG - invalid URL -->
   <img src="image.jpg" alt="Clinic">
   ```

2. **For local images:**
   - Save image in same folder as HTML files
   - Use: `<img src="image.jpg" alt="Description">`

3. **Verify image dimensions:**
   - Images should be at least the width specified in the URL
   - Example: `w=600` means image should be 600+ pixels wide

### Problem: FAQ Accordion Not Opening

**Symptom:** Clicking FAQ questions doesn't expand answers

**Solution:**

1. **Verify JavaScript section is intact:**
   - Don't delete the `<script>` section at the bottom of index.html
   - It should start around line 785

2. **Check that FAQ HTML structure is correct:**
   ```html
   <!-- CORRECT STRUCTURE -->
   <div class="faq-item">
       <button class="faq-question">Question?</button>
       <div class="faq-answer hidden">Answer text</div>
   </div>
   ```

3. **Ensure class names match:**
   - `faq-item` - Container
   - `faq-question` - The clickable question
   - `faq-answer` - The hidden answer
   - `hidden` - Initially hidden (this is correct)

### Problem: Mobile Menu Not Working

**Symptom:** Hamburger menu doesn't open on mobile

**Solution:**

1. **Verify JavaScript is present and intact**
   - The mobile menu toggle code should be in the `<script>` section

2. **Check mobile menu HTML structure:**
   ```html
   <!-- CORRECT -->
   <button class="mobile-menu-button">
       <i class="fas fa-bars"></i>
   </button>
   <div class="mobile-menu hidden">
       <!-- Menu items -->
   </div>
   ```

3. **Test on actual mobile or use browser dev tools:**
   - Press F12
   - Click device icon
   - Select mobile device
   - Refresh page

### Problem: Colors Look Different

**Symptom:** Colors don't match what you expect

**Solution:**

1. **Verify Tailwind color names:**
   - `blue-600` is different from `blue-400`
   - Darker numbers = darker colors (900 is darkest, 100 is lightest)

2. **Test color combinations:**
   - Ensure text has enough contrast with background
   - Dark text on light background (good)
   - Light text on dark background (good)
   - Light text on light background (bad - unreadable)

3. **Check for typos:**
   ```html
   <!-- CORRECT -->
   <div class="bg-blue-600">Content</div>
   
   <!-- WRONG -->
   <div class="bg-bluu-600">Content</div>
   ```

---

## Best Practices

### 1. **Always Back Up Before Making Changes**

Before editing your HTML file:

```
1. Right-click index.html
2. Select "Copy"
3. Paste it as "index-backup.html"
4. Now edit index.html safely
```

### 2. **Make One Change at a Time**

- Change one section, save, and test
- Don't change multiple things at once
- Easier to identify what broke

### 3. **Use Find & Replace Carefully**

When using Find & Replace:
- Always preview changes first
- Don't replace with empty text (you'll delete things)
- Use "Replace All" only if you're certain

### 4. **Keep Consistent Styling**

- Use the same color scheme throughout
- Keep similar spacing between sections
- Maintain the same font sizes for similar elements

### 5. **Test on Multiple Devices**

After making changes, test on:
- Desktop (large screen)
- Tablet (medium screen)
- Mobile (small screen)

### 6. **Maintain Responsive Design**

Always keep responsive classes:

```html
<!-- GOOD - works on all devices -->
<h1 class="text-3xl md:text-4xl lg:text-5xl">Heading</h1>

<!-- BAD - only works on one size -->
<h1 class="text-3xl">Heading</h1>
```

### 7. **Use Meaningful Alt Text for Images**

```html
<!-- GOOD - descriptive -->
<img src="clinic.jpg" alt="Oakland Accident Care clinic reception area">

<!-- BAD - not descriptive -->
<img src="clinic.jpg" alt="image">
```

### 8. **Keep Links Updated**

When you change:
- Business name → Update in header, footer, all pages
- Email address → Update everywhere it appears
- Website URL → Update all "Get Started" buttons

### 9. **Organize Your File Structure**

```
your-website/
├── index.html (main page)
├── privacy.html
├── terms.html
├── blog.html
├── css/ (if you add custom CSS)
│   └── style.css
└── images/ (if you use local images)
    ├── logo.png
    └── clinic.jpg
```

### 10. **Regular Maintenance Checklist**

Every month, verify:

- [ ] All links work correctly
- [ ] Contact information is current
- [ ] Phone numbers are correct
- [ ] Email addresses are correct
- [ ] No broken images
- [ ] Page loads quickly
- [ ] Mobile version looks good
- [ ] Testimonials are current
- [ ] FAQ answers are accurate

---

## Additional Resources

### Learning Resources

- **Tailwind CSS Documentation:** https://tailwindcss.com/docs
- **Font Awesome Icons:** https://fontawesome.com/icons
- **HTML Basics:** https://developer.mozilla.org/en-US/docs/Web/HTML
- **CSS Basics:** https://developer.mozilla.org/en-US/docs/Web/CSS

### Tools You'll Need

- **Text Editor:** Visual Studio Code (free, recommended)
- **Browser:** Chrome, Firefox, or Safari
- **Image Editor:** Canva (free) or Photoshop
- **Color Picker:** https://htmlcolorcodes.com

### Getting Help

If you encounter issues:

1. **Check the Troubleshooting Guide** above
2. **Copy the error message** and search Google
3. **Use browser developer tools:**
   - Press F12
   - Look at the "Console" tab for errors
   - Check the "Elements" tab to inspect HTML

---

## Summary

You now have a complete guide to maintaining and customizing your Oakland Accident Care landing page. Remember:

✅ **DO:**
- Back up your files before editing
- Make one change at a time
- Test on mobile devices
- Keep class names intact
- Update links consistently

❌ **DON'T:**
- Delete class names from HTML tags
- Remove the Tailwind CSS or Font Awesome links
- Delete the JavaScript section
- Use special characters in file names
- Forget to test your changes

**Need help?** Refer back to the specific section that matches your issue, and follow the step-by-step instructions provided.