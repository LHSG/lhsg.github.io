# LHSG Startup Homepage - Implementation Plan

## Project Overview

Transform the existing Jekyll blog (`lhsg_blog`) into a modern startup homepage for **LHSG Inc.** (주)엘에치이에스지.

---

## Company Information

### About LHSG
- **Company Name**: LHSG Inc. (주)엘에치이에스지
- **Tagline**: "Everything about Metaverse & BlockChain"
- **Mission**: "Extend Your Dream with BlockChain At Metaverse!"
- **Vision**: Technology- and human-centered enterprise providing services that can change the world

### Business Areas
1. **AR/VR/MR/Metaverse** - First runner in converging physical and virtual worlds
2. **Cloud Storage** - Secure file sharing, synchronization, and backup
3. **Big Data** - "Big Data as a Service" platform for data analysis
4. **Android STB** - Android UI solutions for mobile/embedded systems
5. **Blockchain** - Next-generation decentralized technology solutions

### Products/Services
| Product | Description |
|---------|-------------|
| WHOOPEE | Photo/video transfer via local Wi-Fi network |
| POP Photo Album | Photo organizer grouping by time & places |
| POP TV | Social TV ratings from SNS via Big Data analysis |
| POP Cloud | Cross-device cloud file access |
| Dead Wave | AR Zombie Shooter game |
| Car Battle AR | AR Drive & Shoot game |

### Contact Information
- **Email**: contact.lhsg@gmail.com
- **Address**: #310, 105 Dong, Seoul National University (SNU), 1 Gwanak-ro, Gwanak-gu, Seoul, Korea
- **Social**: GitHub (lhsg), Facebook (lhsgfb), Twitter (LHSG_)

---

## Current State Analysis

### lhsg_blog (Current Project)
- **Framework**: Jekyll (Ruby-based static site generator)
- **Styling**: Bootstrap 3.x + Custom CSS (hux-blog theme)
- **Structure**: Blog-focused with posts, tags, about page
- **Assets**: Contains LHSG logo, favicon already

### lhsg_hompepage (Reference Project)
Available HTML templates for reference:
- Arena HTML - Modern corporate template with slider
- Statum HTML - Clean business template
- Clumb HTML - Creative agency template
- Creon HTML - Multi-purpose template
- Lewis Landing - Landing page variations

---

## Proposed Architecture

### Option A: Keep Jekyll (Recommended)
**Pros**:
- Free GitHub Pages hosting
- Existing infrastructure in place
- Easy content management via Markdown
- Fast static site delivery

**Cons**:
- Limited dynamic features
- Requires Ruby environment for local dev

### Option B: Convert to Static HTML
**Pros**:
- Simpler deployment
- No build step needed

**Cons**:
- Harder content management
- More code duplication

### Decision: **Option A - Keep Jekyll** with modern Bootstrap 5 theme

---

## Site Structure

```
/
├── index.html          # Homepage with hero, services, about preview
├── about.html          # Full company story & team
├── services.html       # Detailed business areas
├── products.html       # Product showcase
├── portfolio.html      # Project portfolio/case studies
├── blog/               # Keep existing blog functionality
│   └── index.html      # Blog listing
├── contact.html        # Contact form & map
└── _posts/             # Blog posts (existing)
```

---

## Page Specifications

### 1. Homepage (`index.html`)
**Sections**:
1. **Hero Section** - Full-width banner with tagline
   - Background: Tech/Metaverse themed image
   - Text: "Everything about Metaverse & BlockChain"
   - CTA: "Explore Our Services" / "Contact Us"

2. **About Preview** - Brief company intro
   - 2-3 sentences about LHSG
   - Link to full About page

3. **Services Grid** - 4 business areas
   - AR/VR/MR/Metaverse
   - Cloud Storage
   - Big Data
   - Android STB

4. **Products Showcase** - Featured products carousel
   - WHOOPEE, POP Photo Album, POP TV, POP Cloud

5. **Partners Section** - Partner logos

6. **CTA Section** - Contact prompt

7. **Footer** - Links, social, copyright

### 2. About Page (`about.html`)
- Company history & story
- Mission & Vision statements
- Team section (if applicable)
- Press/Media mentions
- Company values

### 3. Services Page (`services.html`)
- Detailed description of each business area
- Technology stack highlights
- Use cases / benefits

### 4. Products Page (`products.html`)
- Individual product cards
- Screenshots / demos
- App store links
- Feature lists

### 5. Portfolio Page (`portfolio.html`)
- Project case studies
- AR/VR demos
- Client work samples

### 6. Contact Page (`contact.html`)
- Contact form
- Google Maps embed (SNU location)
- Address & email info
- Social media links

### 7. Blog (Existing, Update Design)
- Keep existing blog functionality
- Update styling to match new theme

---

## Design Guidelines

### Color Palette
```css
--primary:     #1a1a2e;   /* Dark navy - tech feel */
--secondary:   #16213e;   /* Deep blue */
--accent:      #0f3460;   /* Blue accent */
--highlight:   #e94560;   /* Red highlight for CTAs */
--light:       #f5f5f5;   /* Light background */
--white:       #ffffff;
```

### Typography
- **Headings**: Poppins or Montserrat (modern, clean)
- **Body**: Open Sans or Lato (readable)
- **Code**: Fira Code (for any tech displays)

### Design Principles
- Modern, clean, professional
- Mobile-first responsive
- Emphasize tech/innovation theme
- Subtle animations on scroll
- Clear CTAs and navigation

---

## Technical Implementation

### Phase 1: Setup & Foundation
1. Update `_config.yml` with new site settings
2. Install/configure Bootstrap 5
3. Create new layout templates
4. Set up SCSS structure

### Phase 2: Core Pages
1. Build homepage with all sections
2. Create About page
3. Create Services page
4. Create Products page
5. Create Contact page

### Phase 3: Enhancement
1. Add animations (AOS or similar)
2. Implement contact form (Formspree/Netlify Forms)
3. Add Google Maps integration
4. SEO optimization

### Phase 4: Blog Integration
1. Update blog layout to match new theme
2. Style post pages
3. Update tag/archive pages

### Phase 5: Testing & Deployment
1. Cross-browser testing
2. Mobile responsiveness check
3. Performance optimization
4. Deploy to GitHub Pages

---

## File Structure Changes

### New Files to Create
```
_layouts/
├── homepage.html       # Homepage layout
├── page.html           # General page layout
├── services.html       # Services layout

_includes/
├── header.html         # Updated navigation
├── footer.html         # New footer
├── hero.html           # Hero section
├── services-grid.html  # Services component
├── products-carousel.html
├── partners.html
├── contact-form.html

_sass/
├── _variables.scss     # Design tokens
├── _base.scss          # Base styles
├── _layout.scss        # Layout styles
├── _components.scss    # Component styles
├── _responsive.scss    # Media queries

pages/
├── about.md
├── services.md
├── products.md
├── portfolio.md
├── contact.md
```

### Files to Update
```
_config.yml             # Site configuration
index.html              # Complete rewrite
_includes/head.html     # New assets
_includes/nav.html      # New navigation
css/                    # New styles
```

---

## Content Requirements

### Images Needed
- [ ] Hero background (Metaverse/tech themed)
- [ ] Service icons (4 business areas)
- [ ] Product screenshots (each app)
- [ ] Team photos (if available)
- [ ] Partner logos
- [ ] About page imagery

### Copy Needed
- [ ] Updated company description
- [ ] Service descriptions (detailed)
- [ ] Product feature lists
- [ ] Team bios (if applicable)
- [ ] Contact page copy

---

## Timeline Estimate

| Phase | Tasks | Estimated Effort |
|-------|-------|------------------|
| Phase 1 | Setup & Foundation | 2-3 hours |
| Phase 2 | Core Pages | 6-8 hours |
| Phase 3 | Enhancement | 3-4 hours |
| Phase 4 | Blog Integration | 2-3 hours |
| Phase 5 | Testing & Deploy | 2 hours |
| **Total** | | **15-20 hours** |

---

## Questions for Stakeholder

1. **Team Information**: Should we include a team section? If yes, who should be featured?
2. **Portfolio/Case Studies**: Are there specific projects to showcase?
3. **Blog Strategy**: Keep existing posts or start fresh?
4. **Contact Form**: Preferred backend (Formspree, Netlify Forms, custom)?
5. **Analytics**: Google Analytics tracking required?
6. **Domain**: Will this be hosted on lhsg.co.kr or lhsg.github.io?
7. **Language**: Korean, English, or both?
8. **Additional Pages**: Careers page? Investor relations?

---

## References

### External Resources
- [LHSG Official Website](http://www.lhsg.co.kr/) - Existing content reference
- [Bootstrap 5 Documentation](https://getbootstrap.com/docs/5.3/)
- [Jekyll Documentation](https://jekyllrb.com/docs/)

### Internal Reference Templates
- `/Users/artilla/Dev/workspace/homepage/lhsg_hompepage/Refs/arenahtml-10/` - Modern corporate
- `/Users/artilla/Dev/workspace/homepage/lhsg_hompepage/lhsg/` - LHSG-specific pages
- `/Users/artilla/Dev/workspace/homepage/lhsg_hompepage/WebContent/` - Existing homepage content

---

## Approval

- [ ] Plan reviewed
- [ ] Architecture approved
- [ ] Design direction confirmed
- [ ] Content requirements confirmed
- [ ] Ready to proceed with implementation

---

*Plan created: 2026-01-04*
*Last updated: 2026-01-04*
