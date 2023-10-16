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

### Design system
- Headline font: Monteserrat
- Text font: Open sans
- Accent color: Blue
- Primary and secondary color: White / black

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

### CSS colors
- Use this to get svg filter colors: [https://angel-rs.github.io/css-color-filter-generator/](https://angel-rs.github.io/css-color-filter-generator/) 
- or this: [https://codepen.io/sosuke/pen/Pjoqqp](https://codepen.io/sosuke/pen/Pjoqqp) 
- google "color picker" to find hex color etc
- use this to convert hex to rgba: [https://rgbacolorpicker.com/hex-to-rgba](https://rgbacolorpicker.com/hex-to-rgba) 
- webcolors: [https://en.wikipedia.org/wiki/Web_colors](https://en.wikipedia.org/wiki/Web_colors).

### Media queries:
- Using **600px** as a breakpoint for a responsive media query is a common practice. However, it ultimately depends on the design and layout of your website. If you have a lot of content or a complex layout, you may want to consider using a larger breakpoint. Conversely, if your website is simple and has less content, you may be able to use a smaller breakpoint. It's important to test your website on different devices and screen sizes to ensure that it looks good and functions properly.

### Random UUID for FAQ / Support perma links:
Run this in terminal (Change 4 to some arbitrary number to get different lengths)
```bash
cat /dev/urandom | LC_CTYPE=C tr -dc 'a-zA-Z0-9' | head -c 4; echo
```

### The feature grid:
- 8 features total
- Desktop: 3x2
- Mobile: 2x4

### The compare grid:
- Desktop: 6 Columns (2 hidden)
- Mobile: 3 Columns (we hide 5)

### Theme colors
Theme colors are stored in as variables in th css/common/theme.css and can be customized to change globally

### Resources:
- Media querries to the fonts: https://codyhouse.co/blog/post/css-custom-properties-vs-sass-variables
- Clamp in fluid layouts (very comprehensive tut): https://blog.logrocket.com/flexible-layouts-without-media-queries/
- Has nice blog design: https://astroship.web3templates.com/blog and coloring in darkmode

### Videos:
- Record video without red circle w/ Quicktime via lightning cable. Record video. Then choose iPhone
- Export to 720p in Quicktime -> Export (to get the file size down. 1-3mb for 15-30 sec vid is fine)
- Use adobe express online video converter https://www.adobe.com/express/ to conver mov to mp4
- There is bezel for iPhone 11 Pro Max and iPhone 15 Pro Max. Make sure pixel ratio is correct b4 use.

### Todo:
- Quickly try the list blog grid with images. 
- Add FAQ item that has link to video of macApp "Where can I can see a video of macApp?" Here is a link to our launch video which includes footage of the macApp
- Align the download btns like the price btns (the dl boxes are also not equal in width)

### Future milestones:
- Move to github action based jekyll hosting to get paginator v2 which has tagging :yum:
- ...or move to github action based astro.space hosting
- Incorporate video of macOS / iPadOS app
- Add more responsive breakpoints (laptop and tablet size)


```html
<video autoplay loop muted playsinline controls preload="auto" poster="{{ '/assets/images/video-poster.jpg' | prepend: site.baseurl }}">
	<source src="{{ '/assets/video/' | prepend: site.baseurl }}{{ item.url }}">
	Sorry, your browser doesn't support embedded videos.
</video>
```

### Alternate colors:
- Alternatice posetive color: (greenish) #62C8A9 and negative: (redish) #ED6D6E
- Alternate filters: `--posetive-filter: brightness(0) saturate(100%) invert(72%) sepia(43%) saturate(393%) hue-rotate(111deg) brightness(90%) contrast(89%); /* posetive */
	--negative-filter: brightness(0) saturate(100%) invert(66%) sepia(58%) saturate(6413%) hue-rotate(323deg) brightness(107%) contrast(85%); /* negative */`

