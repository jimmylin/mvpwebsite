# Volleyball Club Jekyll Theme

A professional, responsive Jekyll theme designed specifically for volleyball clubs. Perfect for GitHub Pages hosting!

## Features

- 🏐 Clean, modern design with volleyball-themed colors
- 📱 Fully responsive (mobile, tablet, desktop)
- 🎯 Pre-built sections for:
  - About the Club
  - Teams (with individual team pages)
  - Clinics & Camps
  - Travel Information
  - Contact
- 🎨 Easy to customize colors and content
- ⚡ Fast loading and SEO optimized
- 📄 Multiple page layouts (home, page, team, clinic)
- 🔍 SEO-friendly with jekyll-seo-tag

## Quick Start

### 1. Copy to Your GitHub Repository

1. Create a new repository on GitHub named `yourusername.github.io` (or use an existing repo)
2. Copy all files from this theme to your repository
3. Enable GitHub Pages in your repository settings

### 2. Customize Your Site

Edit `_config.yml` to update your club information:

```yaml
title: "Your Volleyball Club Name"
description: "Your club description"
club_name: "Your Volleyball Club"
club_email: "info@yourclub.com"
club_phone: "(555) 123-4567"
club_address: "123 Sports Complex Dr, Your City, ST 12345"

# Update your social media links
facebook_url: "https://facebook.com/yourclub"
instagram_url: "https://instagram.com/yourclub"
twitter_url: "https://twitter.com/yourclub"
```

### 3. Customize Content

#### Update the About Page
Edit `about.md` with your club's history, mission, and coaching staff information.

#### Add Your Teams
1. Create new files in the `_teams` folder
2. Copy the format from existing team files (e.g., `18u-elite.md`)
3. Update the front matter and content:

```yaml
---
layout: team
title: Your Team Name
age_group: 16U (Born 2008-2009)
coach: Coach Name
practice_schedule: Days and times
season: Season dates
---

Your team description and details here...
```

#### Add Clinics and Camps
1. Create new files in the `_clinics` folder
2. Use the existing clinic files as templates
3. Update with your clinic details

#### Update Travel Information
Edit `travel.md` with your club's specific tournament schedule and travel policies.

#### Update Contact Information
Edit `contact.md` with your specific contact details and FAQs.

### 4. Customize Colors

To change the color scheme, edit `assets/css/style.css` and update the CSS variables at the top:

```css
:root {
  --primary-color: #d32f2f;      /* Main brand color (red) */
  --secondary-color: #1976d2;    /* Secondary brand color (blue) */
  --dark-color: #212121;         /* Dark backgrounds */
  --light-color: #f5f5f5;        /* Light backgrounds */
  --text-color: #333;            /* Main text color */
  --accent-color: #ffa000;       /* Accent/button color (orange) */
}
```

## File Structure

```
volleyball-club-theme/
├── _config.yml           # Main configuration file
├── _layouts/             # Page layouts
│   ├── default.html      # Base layout
│   ├── home.html         # Home page layout
│   ├── page.html         # Standard page layout
│   ├── team.html         # Team page layout
│   └── clinic.html       # Clinic page layout
├── _includes/            # Reusable components
│   ├── header.html       # Site header/navigation
│   └── footer.html       # Site footer
├── _teams/               # Team pages (collection)
│   ├── 18u-elite.md
│   └── 14u-regional.md
├── _clinics/             # Clinic pages (collection)
│   ├── summer-camp.md
│   └── setter-clinic.md
├── assets/
│   └── css/
│       └── style.css     # Main stylesheet
├── index.md              # Home page
├── about.md              # About page
├── teams.md              # Teams index page
├── clinics.md            # Clinics index page
├── travel.md             # Travel information page
├── contact.md            # Contact page
├── Gemfile               # Ruby dependencies
└── README.md             # This file
```

## Adding New Pages

To add a new page:

1. Create a new `.md` file in the root directory
2. Add front matter:

```yaml
---
layout: page
title: Your Page Title
permalink: /your-page-url/
---

Your page content here...
```

3. Add a link to the navigation in `_includes/header.html`

## Local Development

To preview your site locally:

1. Install Ruby and Bundler
2. Run these commands:

```bash
bundle install
bundle exec jekyll serve
```

3. Visit `http://localhost:4000` in your browser

## Deployment to GitHub Pages

1. Commit all your changes to your repository
2. Push to GitHub
3. Go to your repository Settings → Pages
4. Select the branch (usually `main` or `master`)
5. Your site will be published at `https://yourusername.github.io`

## Adding Photos

To add photos:

1. Create an `assets/images` folder
2. Add your images there
3. Reference them in your markdown:

```markdown
![Alt text](/assets/images/your-image.jpg)
```

Or in HTML:
```html
<img src="/assets/images/your-image.jpg" alt="Alt text">
```

## Customization Tips

### Change the Hero Section
Edit the `.hero` styles in `assets/css/style.css` to customize the home page hero section.

### Add Team Photos
In team pages, you can add photos by including an image reference:

```yaml
---
layout: team
title: Team Name
image: /assets/images/team-photo.jpg
---
```

Then update `_layouts/team.html` to display the image.

### Custom Fonts
To use custom fonts, add Google Fonts or other font links to `_layouts/default.html` in the `<head>` section.

## Support

For issues or questions:
- Check the Jekyll documentation: https://jekyllrb.com/docs/
- GitHub Pages documentation: https://docs.github.com/en/pages

## License

This theme is free to use and modify for your volleyball club.

---

**Happy Volleyball! 🏐**
