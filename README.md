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

### Font research:
- Alternative font for header: inter, "Syne Bold"
- Alternative font for paragraph: lato or "Istok Web" or Manrope, "open sans" , inter, Barlow, IBM Plex Sans, dm sans
- https://www.leadpages.com/blog/best-google-fonts
- https://www.typewolf.com/google-fonts
- https://www.pagecloud.com/blog/best-google-fonts-pairings
- https://fonts.google.com/
- https://www.figma.com/google-fonts/

## Todo:

- Do SEO testing o the site. Do research into which online service can help with this.
- Move to github action based jekyll hosting to get paginator v2 which has tagging :yum:
- Add more responsive breakpoints (laptop and tablet size)

### Now 
- Make branded vimeo account etc 👈 
- Add logo to linkedin, post video, remove some old posts, change bio 👈  
- Add logo, video, Ipad and iphone images to IG (remove old posts), change bio 👈 
- Add logo to twitter, pin video, remove old posts, change bio 👈
- Change bio in PH to be more focused 👈 
- Announcement on the slack, change slack avatar and description. 

### Next
- clean up the todo list in this readme
- add a bit of padding above blog grid, check with debug colors

### Later
- add the part about novel tech stack and patents to the introduction video 🚫 nope
- add hover styles to faq items see legacy 🚫
- add mouseover effects to faq-items 🚫
- store the device frame bezel html somewhere, we should use it for adding bezels to demo videos in SoMe etc 🚫
- we could also draw technical bezels. ala the olo app website uses 🚫
- add competitor element (An underdog picking a fight with the behemoths / A challanger among behemoths) 🚫
- add pricing element 🚫
- try adding dropshadow to the devices.  🚫
- add mask to videos.  🚫
- make the video switcher work 🚫
- Record app videos 🚫
- begin to add mouse hover on elements. faq items for instance. subtle brightness change 🚫
- add nav menu tag selected state 🚫
- Make outline device bezels in svg in sketch.app 🚫 (later)
- Tweak text with gpt 🚫 (later)
- add article 🚫 
- add more width to the website 🚫
- tweak porportions more 🚫
- change offline sync to local sync. Local sounds less tinfoil hat. 🚫
- design all the different shadings and tones for the fonts etc (seperate preview) 🚫
- Make the device bezels that are perfect for iphone11 max, and ipad pro (isolated) 🚫
- top_view/ own preview own style work in isolation (do it with jekyl?) 🚫
- feature_view/ own preview own style (do it with jekyl?) 🚫
- faq_view/ own preview own style (do it with jekyl?) 🚫
- download_view/ preview style (do it with jekyl?) 🚫
- header_view/ own preview style (do it with jekyl?) 🚫
- footer_view own preview style (do it with jekyl?) 🚫
- use the database icon for database 🚫
- tweak the design of the feature icons 🚫
- tweak the design of the feature icons 🚫
- add macbook air bezel 🚫
- create the pricing module 🚫
- create an alternate feature list module 🚫 
- Maybe make the pricing chart just to have med it in this style 🚫
- add link to more faq. in the description of the faq. 🚫
- Change top titles: 1. Offline (sync via Bluetooth), 2. Secure (Secure-enclave, E2EE, Biometric), 3. Local (Local device database)  🚫
- try to make the orange ascent color more peach 🚫
- try to tweak colors with filters. use the dark chrome extension and use iphone photo filters 🚫
- add colors to tag cloud in blog and support 🚫
- move email to footer, just use @ icon or? 🚫
- make a pricing module. see apple notes, and v0 printscreens (after experimenting with poart dots) 🚫
- try different bezel designs for the devices. gradients, shades, shaddows etc 🚫
- add green tone to a gradient. experiment with different looks. 🚫
- experiment with grany gradient shapes 🚫 (drop grainy look, we want simple design)
- add correct text from current website 🚫 (do later, we dont want to get tunnel vision on end result)
- try a half circle with grainy mask 🚫
- add an eye icon with grainy mask. representing the orewellian vibe. maybe 🚫
- use text buttons for next and previous in blog 🚫
- smaller font size for about page (🧠 no brainer, easy) 🚫
- add nicer grid to features for mobile. either center icon. or use 3x3 grid ❤️ 🚫
- also use grid for blog (legacy) 🚫
- test jekyll site on github pages 🚫
- try to add play and download icons to the see-how-it-works module (easy) 🚫
- try to add a color to the center of the website 🚫
- add a description for the blog page about freequent updates etc. also link to newsletter signup 🚫
- add hover effevt for faq items 🚫
- add newsletter link in the blog description, or add it to the blog page with a input field 🚫
- add intercom instead of crisp 🚫 (maybe not, stay scrappy and lean)
- enable the background color for the FAQ tag cloud, remove the debug color 🚫 (remove tag cloud, instead reduce amount of faq items)
- add a description for the faq page with contact info and info about chat function 🚫 (keep it simple)
- make the email button hover fo white 🚫 (there is no email atm)
- move blog indicator to bottom and add 9 posts per page (still relevant?) 🚫
- add contact email in the faq description 🚫 (people can just use SoMe)
- test only showing 6 features in the feature secion. 🚫 (nah 9 is fine, 6 looks too empty)
- try full width of page? super wide website etc🚫 (very hard to manage all the formats that way, hard to make it look good)
- try white icons for the feature icons 🚫 nah. ascent color of icons makes them meatier
- make front slogan text non all caps maybe (maybe) 🚫 keep as is. its how headlines are these days
- maybe make feature icon color mint on hover and white otherwise 🚫 its fine as is. add hover effect to bg instead maybe
- add read more link to blog post bottom, and move date up, with hover effect 🚫 or maybe keep as is?
- add transitions to hover state. see legacy for ready to use animation code 🚫 Not important at the moment
- add an overlay to the entire website. check the grid. ask copilot (do it later, use debug colors for now to spot issues) 🚫
- use flex gap and top bottom padding to align groups of elements etc (connected to debug grid) 🚫 maybe later
- change nav items text to: About, Updates, FAQ 🚫 or keep as is? 
- maybe add a subtle gray bg on buttons? (try it quickly) 🚫
- use em for consts instead of px sizes. ask copilot for best practices (maybe later after feedback etc) 🚫

### Future milestones:
- Move to github action based jekyll hosting to get paginator v2 which has tagging :yum:
- ...or move to github action based astro.space hosting
- Add more responsive breakpoints (laptop and tablet size)
 