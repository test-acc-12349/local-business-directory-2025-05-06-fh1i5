# Local Business Directory

> Discover the best local businesses in one place

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization Guide](#customization-guide)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Resources & Support](#resources--support)

## Overview

Local Business Directory is a responsive, user-friendly directory website that showcases local businesses in a clean, three-column grid layout. The platform features categorized listings, search functionality, and easy-to-navigate business profiles.

## Features

- Responsive 3-column grid layout
- Category-based filtering
- Search functionality
- Business profile pages
- Contact forms
- Mobile-friendly design
- SEO optimized
- Fast loading times

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/local-business-directory

# Navigate to project directory
cd local-business-directory

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure

```
local-business-directory/
├── src/
│   ├── components/
│   ├── pages/
│   ├── styles/
│   └── utils/
├── public/
│   ├── images/
│   └── assets/
├── data/
│   └── businesses.json
├── config.js
└── package.json
```

## Customization Guide

### Adding/Editing Directory Items

1. Navigate to `data/businesses.json`
2. Add new business entries using the following format:

```json
{
  "id": "unique-id",
  "name": "Business Name",
  "category": "Category",
  "description": "Business description",
  "address": "Business address",
  "phone": "123-456-7890",
  "website": "https://example.com",
  "image": "/images/business-image.jpg"
}
```

### Modifying Category Labels

1. Open `src/utils/categories.js`
2. Edit the category array:

```javascript
export const categories = [
  "Restaurants",
  "Retail",
  "Services",
  "Entertainment",
  // Add more categories
];
```

### Updating Hero Section

1. Locate `src/components/Hero.js`
2. Modify the content:

```javascript
<div className="hero">
  <h1>Your Custom Heading</h1>
  <p>Your custom description</p>
  // Add more elements
</div>
```

### Customizing Colors and Styling

1. Find `src/styles/variables.css`
2. Update color variables:

```css
:root {
  --primary-color: #your-color;
  --secondary-color: #your-color;
  --text-color: #your-color;
  --background-color: #your-color;
}
```

## Deployment

### Building for Production

```bash
# Create production build
npm run build

# Test production build locally
npm run serve
```

### Deployment Platforms

- Vercel (Recommended)
- Netlify
- GitHub Pages

## Custom Domain Setup

1. Purchase domain from preferred registrar
2. Add domain in deployment platform
3. Configure DNS settings:
   - Add A record pointing to deployment platform
   - Add CNAME record for www subdomain
4. Wait for DNS propagation (24-48 hours)

## Troubleshooting

### Common Issues

1. **Images Not Loading**
   - Verify image paths in `businesses.json`
   - Check image formats (supported: jpg, png, webp)
   - Ensure images are in public directory

2. **Build Errors**
   - Clear npm cache: `npm cache clean --force`
   - Delete node_modules and reinstall
   - Check for syntax errors in JSON files

3. **Styling Issues**
   - Clear browser cache
   - Check CSS specificity
   - Verify media queries

## Resources & Support

- [Documentation](https://docs.example.com)
- [GitHub Issues](https://github.com/yourusername/local-business-directory/issues)
- [Support Email](mailto:support@example.com)

### Community
- [Discord Server](https://discord.gg/example)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/local-business-directory)

### Contributing
Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on contributing to this project.

### License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

---

Made with ❤️ by [Your Name](https://github.com/yourusername)