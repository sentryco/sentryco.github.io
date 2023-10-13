# sentry.co
Website for sentry.co

### General information
- Uses custom domain from [namecheap.com](namecheap.com) etc
- Uses anonymised Google analytics (GDPR friendly)
- CNAME file must match the used domain

### Todo:
- Investigate new GDPR rules regarding anonymised Google analytics
- Update the crisp account with correct name / logo etc
- Fix favicon not showing in safari

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

### Todo:
- Quickly try the list blog grid with images. 🚫
- Add FAQ item that has link to video of macApp "Where can I can see a video of macApp?" Here is a link to our launch video which includes footage of the macApp

```html
<video autoplay loop muted playsinline controls preload="auto" poster="{{ '/assets/images/video-poster.jpg' | prepend: site.baseurl }}">
	<source src="{{ '/assets/video/' | prepend: site.baseurl }}{{ item.url }}">
	Sorry, your browser doesn't support embedded videos.
</video>
```

### Finalizing: (Thursday)
- Add html best practice checkup as a github action or use external service, do research (after launch)
- Add the TOA, PA, NA, etc. copy from excisiting website (use gpt if one is missing). 
- Upload site to github (announce on friday)

### Videos:

Maybe make an importable json file for demo accounts?

1. Store locally
  - Authenticate with bio-auth (Add master-pass as option)
  - Show Apple, Evernote, Dribble, Slack, Trello, Amazon, Messenger, Facebook, Soundcloud, MailChimp 
  - Scroll the tabbar, press favorites, press search, search for trello
  - Go into detail on trello and change a password. Save. Go back. To main.

2. Sync offline ✅
  - From MainScreen. With 3 accounts press prefs
  - From preferences. Tap Add device. Tap add device. And confirm adding macbook
  - Go back to main and see 3 new accounts load (shoppify, LastFM, Trello)

3. AutoFill anywhere
  - In Safari. In Evernote.com
  - Tap textField. Tap The AutoFill button that prompts the AF ext
  - Press login

### Alternate colors:
- Alternatice posetive color: (greenish) #62C8A9 and negative: (redish) #ED6D6E
- Alternate filters: `--posetive-filter: brightness(0) saturate(100%) invert(72%) sepia(43%) saturate(393%) hue-rotate(111deg) brightness(90%) contrast(89%); /* posetive */
	--negative-filter: brightness(0) saturate(100%) invert(66%) sepia(58%) saturate(6413%) hue-rotate(323deg) brightness(107%) contrast(85%); /* negative */`


### Launch blurb

New website out! https://sentry.co/

[Gif of iPad IRL video at deichman]
[Gif of mobile IRL video at deichman]

Here is how we made the website 👇

- 💰 Pure CSS based price-toggle component (Zero JS)
- 🙋‍♀️ Pure CSS based FAQ / Support component (linked w/ UUID) (Zero JS)
- 🐙 Hosted on github pages with Jekyll backend
- ⬇️ Data-model stored in .yml and .markdown
- 📚 Fonts: Header: Monteserrat, Text: OpenSans
- 🎨 Icon-set https://www.feather-icons.com/
- 🖥️ 2 breakpoint reposive layout: Mobile and Desktop 
- 💧 Front end: HTML via liquid expands
- 🍦 Pure vanilla CSS3 variables (Zero CSS frameworks etc)
- 🌙 Darkmode only w/ duo color highlights: 🔵 accent-blue and ⚪️ primary-white

Tools used:
- 🦾 Prompt-coded with Cursor.so  (prompt-coding is so much faster than webflow / framer / no-code etc)
- 🤖 ChatGPT / Grammarly AI to clean up some of the text
- 🖌️ iPad notes + apple pencil for initial mockup / concept
- 💎 Sketch app for finalizing the design
- 🌍 All code is open-source: https://github.com/sentryco/sentryco

Next website goals:
- 🆕 Move to github action based jekyll hosting to get paginator v2 which has tagging 😋
- 🛸 ...or move to github action based astro.space hosting 
- 📽️ Incorporate video of macOS / iPadOS app
- 💻 Add more responsive breakpoints (laptop and tablet size)
