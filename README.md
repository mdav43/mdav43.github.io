# Professional Portfolio Website

A clean, professional Jekyll website for showcasing your experience, skills, and blog posts.

## Overview

This is a Jekyll-based static website designed to serve as a professional portfolio and blog. It's optimized for GitHub Pages and is easy to maintain and update.

## Features

- **Home Page**: Professional landing page with call-to-action buttons
- **About Page**: Detailed information about your professional experience, skills, and education
- **Posts Page**: Blog listing page showing all your posts
- **Responsive Design**: Mobile-friendly and looks great on all devices
- **Fast Loading**: Static site generation ensures quick page loads
- **SEO Optimized**: Built-in SEO tags for better search engine visibility

## Getting Started

### Prerequisites

- Ruby (version 2.7 or higher)
- Bundler

### Local Development

1. Install dependencies:
   ```bash
   bundle install
   ```

2. Run the development server:
   ```bash
   bundle exec jekyll serve
   ```

3. Open your browser and navigate to `http://localhost:4000`

## Customization

### Update Your Information

Edit `_config.yml` to update:
- Site title
- Your name
- Email address
- Description

### Modify the About Page

Edit `about.md` to update:
- Professional experience
- Skills and technologies
- Education
- Certifications

### Add New Blog Posts

Create a new file in the `_posts` directory with the naming convention:
```
YYYY-MM-DD-title-of-post.md
```

Example:
```markdown
---
layout: post
title: "Your Post Title"
date: 2024-03-15
categories: [category1, category2]
---

Your post content here...
```

### Customize Styling

Edit `assets/css/style.css` to modify:
- Colors (see CSS variables in `:root`)
- Fonts
- Spacing
- Layout

## Site Structure

```
.
├── _config.yml           # Site configuration
├── _includes/            # Reusable components
│   ├── header.html
│   └── footer.html
├── _layouts/             # Page templates
│   ├── default.html
│   ├── page.html
│   └── post.html
├── _posts/               # Blog posts
├── assets/
│   └── css/
│       └── style.css     # Main stylesheet
├── about.md              # About page
├── posts.md              # Posts listing page
├── index.md              # Home page
└── Gemfile               # Ruby dependencies
```

## Deployment

This site is configured for GitHub Pages. Simply push your changes to the main branch, and GitHub will automatically build and deploy your site.

### GitHub Pages Setup

1. Go to your repository settings
2. Navigate to "Pages"
3. Select the branch to deploy from (usually `main`)
4. Your site will be available at `https://yourusername.github.io`

## Adding Content

### Quick Updates

- **Update your experience**: Edit `about.md`
- **Add a new post**: Create a file in `_posts/` following the naming convention
- **Change site colors**: Modify CSS variables in `assets/css/style.css`
- **Update navigation**: Edit `_includes/header.html`

## Tips for Maintaining Your Site

1. **Write regularly**: Consistent blog posts keep your site active and engaging
2. **Keep information current**: Update your about page as you gain new experiences
3. **Use descriptive titles**: Make your blog post titles clear and searchable
4. **Add categories**: Organize posts with relevant categories for easier navigation
5. **Optimize images**: If you add images, compress them for faster loading

## Troubleshooting

### Site not building?
- Check `_config.yml` for syntax errors
- Ensure all front matter in posts has proper YAML formatting
- Verify Ruby and Bundler are properly installed

### Styling not applying?
- Clear your browser cache
- Check for CSS syntax errors
- Ensure the stylesheet path in `_layouts/default.html` is correct

## Support

For Jekyll documentation, visit: https://jekyllrb.com/docs/

For GitHub Pages documentation, visit: https://docs.github.com/en/pages

## License

This project is open source and available under the MIT License.
