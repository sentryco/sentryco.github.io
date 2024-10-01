# sentry.co

Website for sentry.co

### General information
- Uses custom domain from [namecheap.com](namecheap.com) etc
- Uses anonymised Google analytics (GDPR friendly)
- CNAME file must match the used domain

### Testing
- Use Google chrome developer mode to test responsive layouts at smaller sizes
- Test on actual Devices iPad / iPhone
- Test online. Sometimes serverside is different from local host

### Features
- Jekyll  (pagination v1, hosted via github actions / github pages)
- Pure HTML, CSS (no JS other than GA)
- Hosted on github-pages
- Front, about, blog, support
- Dark mode only
- Google analytics (Annonymous)
- Google fonts (OpenSource)

### Jekyll architecture gotchas:
`_data` has the data model (text, links etc)
`_includes` has html elements (sub-elements etc)
`_layouts` has page html structures (html pages)
`_posts` has markdown blog posts (blog posts)
`_site` has the jekyll output (Render of static website)
`pages` has the core pages (These show up in nav)
`blog` has the blogpost template (blog post structure)
`css` has styles (styling)
`assets` has svgs etc (images, svg etc)
`legal` add doc for this

### Media queries:
- Using **600px** as a breakpoint for a responsive media query is a common practice. However, it ultimately depends on the design and layout of your website. If you have a lot of content or a complex layout, you may want to consider using a larger breakpoint. Conversely, if your website is simple and has less content, you may be able to use a smaller breakpoint. It's important to test your website on different devices and screen sizes to ensure that it looks good and functions properly.

### Random UUID for FAQ / Support perma links:
Run this in terminal (Change 4 to some arbitrary number to get different lengths)
```bash
cat /dev/urandom | LC_CTYPE=C tr -dc 'a-zA-Z0-9' | head -c 4; echo
```

### Google fonts used: 
- IBM Plex Sans
- Montserrat
- Source Sans Pro

### The feature grid:
- 9 features total
- Desktop: 3x3
- Mobile: 1x9

### The blog grid:
- Desktop: 3 x 2
- Mobile: 1 x 9

### Theme colors
Theme colors are stored in as variables in th css/common/theme.css and can be customized to change globally

### Resources:
- Media querries to the fonts: https://codyhouse.co/blog/post/css-custom-properties-vs-sass-variables
- Clamp in fluid layouts (very comprehensive tut): https://blog.logrocket.com/flexible-layouts-without-media-queries/
- Has nice blog design: https://astroship.web3templates.com/blog and coloring in darkmode
- Lots of inspo: https://www.relume.io/page-templates

### Font research:
- Alternative font for header: inter, "Syne Bold"
- Alternative font for paragraph: lato or "Istok Web" or Manrope, "open sans" , inter, Barlow, IBM Plex Sans, dm sans
- https://www.leadpages.com/blog/best-google-fonts
- https://www.typewolf.com/google-fonts
- https://www.pagecloud.com/blog/best-google-fonts-pairings
- https://fonts.google.com/
- https://www.figma.com/google-fonts/

## Todo:

- Do SEO testing to the site. Do research into which online service can help with this.
- Move to github action based jekyll hosting to get paginator v2 which has tagging :yum:
- Add more responsive breakpoints (laptop and tablet size)
- add a bit of padding above blog grid, check with debug colors

### Future milestones:
- Move to github action based jekyll hosting to get paginator v2 which has tagging :yum:
- ...or move to github action based astro.space hosting
- Add more responsive breakpoints (laptop and tablet size)
 