# Hero Section Image Replacement Guide

This guide explains how to replace the placeholder images in the hero section with your company's professional photos.

## Overview

The enhanced hero section includes several placeholder elements designed to showcase your team and company culture:

- 4 Floating cards with themed placeholders
- 3 Talent profile placeholders in the talent showcase
- Modern SVG icons throughout the section

## Image Specifications

### Floating Cards
- **Format**: JPG, WebP, or PNG
- **Dimensions**: 400×300px minimum (4:3 aspect ratio recommended)
- **File Size**: < 200KB each for optimal loading
- **Quality**: High-resolution, professional photography

### Profile Photos
- **Format**: JPG or WebP
- **Dimensions**: 80×80px minimum (1:1 square aspect ratio)
- **File Size**: < 50KB each
- **Quality**: Clear headshots with good lighting

## Replacement Instructions

### 1. Business Meeting Card (Top-Right Floating Card)

**Current placeholder location**: Lines ~125-135 in `index.html`

**Find this code:**
```html
<div class="absolute inset-0 bg-gradient-to-br from-brand-600/20 to-brand-800/30 flex items-center justify-center">
  <svg class="w-8 h-8 text-brand-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z" />
  </svg>
</div>
```

**Replace with:**
```html
<img src="assets/business-meeting.jpg" alt="Business Meeting" class="absolute inset-0 w-full h-full object-cover" />
```

**Recommended image**: Professional business meeting scene showing diverse team collaboration.

### 2. Tech Team Card (Bottom-Left Floating Card)

**Current placeholder location**: Lines ~145-155 in `index.html`

**Find this code:**
```html
<div class="absolute inset-0 bg-gradient-to-br from-brand-600/20 to-brand-800/30 flex items-center justify-center">
  <svg class="w-10 h-10 text-brand-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
  </svg>
</div>
```

**Replace with:**
```html
<img src="assets/tech-team.jpg" alt="Tech Team" class="absolute inset-0 w-full h-full object-cover" />
```

**Recommended image**: IT professionals working with computers, servers, or in a modern office environment.

### 3. Remote Work Card (Top-Left Floating Card)

**Current placeholder location**: Lines ~165-175 in `index.html`

**Find this code:**
```html
<div class="absolute inset-0 bg-gradient-to-br from-brand-600/20 to-brand-800/30 flex items-center justify-center">
  <svg class="w-6 h-6 text-brand-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 7v10a2 2 0 002 2h14a2 2 0 002-2V9a2 2 0 00-2-2H5a2 2 0 00-2-2v0" />
  </svg>
</div>
```

**Replace with:**
```html
<img src="assets/remote-work.jpg" alt="Remote Work" class="absolute inset-0 w-full h-full object-cover" />
```

**Recommended image**: Professional working remotely on laptop, home office setup, or video conference scene.

### 4. Diversity Team Card (Bottom-Right Floating Card)

**Current placeholder location**: Lines ~185-195 in `index.html`

**Find this code:**
```html
<div class="absolute inset-0 bg-gradient-to-br from-brand-600/20 to-brand-800/30 flex items-center justify-center">
  <svg class="w-8 h-8 text-brand-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 4.354a4 4 0 110 5.292M15 21H3v-1a6 6 0 0112 0v1zm0 0h6v-1a6 6 0 00-9-5.197m13.5-9a2.5 2.5 0 11-5 0 2.5 2.5 0 015 0z" />
  </svg>
</div>
```

**Replace with:**
```html
<img src="assets/diverse-team.jpg" alt="Diverse Team" class="absolute inset-0 w-full h-full object-cover" />
```

**Recommended image**: Diverse group of professionals representing different backgrounds, ages, and roles.

### 5. Talent Profile Photos

**Current placeholder locations**: Lines ~260-280, ~290-310, ~320-340 in `index.html`

**Find this pattern (appears 3 times):**
```html
<div class="h-full w-full rounded-full bg-brand-600/10 text-brand-700 grid place-items-center font-extrabold text-sm">QA</div>
```

**Replace each with:**
```html
<img src="assets/candidate-1.jpg" alt="QA Specialist" class="w-full h-full object-cover rounded-full" />
```

**Note**: Use different image files for each candidate (candidate-1.jpg, candidate-2.jpg, candidate-3.jpg).

## File Organization

Create an `assets` folder in your root directory:
```
/
├── assets/
│   ├── business-meeting.jpg
│   ├── tech-team.jpg
│   ├── remote-work.jpg
│   ├── diverse-team.jpg
│   ├── candidate-1.jpg
│   ├── candidate-2.jpg
│   └── candidate-3.jpg
├── index.html
└── HERO_IMAGES_README.md
```

## Image Optimization Tips

1. **Compress images** using tools like TinyPNG or ImageOptim
2. **Use WebP format** when possible for better compression
3. **Implement lazy loading** for performance
4. **Provide alt text** for accessibility
5. **Test on multiple devices** to ensure images display correctly

## Professional Photography Recommendations

### Business Meeting Photos
- Conference room discussions
- Whiteboard planning sessions
- Team collaboration moments
- Client presentation scenes

### Tech Team Photos  
- Developers coding
- System administrators working
- IT support interactions
- Modern office environments

### Remote Work Photos
- Home office setups
- Video conferencing
- Mobile work scenarios
- Flexible workspace arrangements

### Diverse Team Photos
- Multi-cultural team gatherings
- Different age groups
- Various professional roles
- Inclusive workplace moments

### Candidate Profile Photos
- Professional headshots
- Consistent lighting and background
- Clear, friendly expressions
- High-quality resolution

## Responsive Behavior

- **Desktop (≥1024px)**: All floating cards visible with rotation effects
- **Tablet (768px-1023px)**: Floating cards hidden, main content responsive
- **Mobile (<768px)**: Floating cards hidden, optimized mobile layout

## Testing Checklist

After replacing images:

- [ ] All images load correctly on desktop
- [ ] Mobile view displays properly (floating cards hidden)
- [ ] Tablet view is responsive
- [ ] Images are optimized for web
- [ ] Alt text is descriptive and accessible
- [ ] File sizes are reasonable for fast loading
- [ ] Images maintain professional appearance
- [ ] Brand colors and styling are preserved

## Support

If you need assistance with image replacement or encounter any issues, please refer to the HTML comments in the source code or contact your development team.