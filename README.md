# Anthony Marquez: personal website

This folder is the complete website. It is plain HTML, CSS and JavaScript, so there is nothing to install and nothing to build. To preview it, open `index.html` in any browser.

## How it is built

The site is hand-coded with no framework and no build step, so it loads fast and runs anywhere.

| Part | What is used |
|---|---|
| Structure | HTML5, one page (`index.html`) |
| Styling | Plain CSS: custom properties for the color palette, CSS Grid and Flexbox for layout, responsive breakpoints for phone, tablet and desktop, keyframe animations |
| Interactivity | Plain JavaScript (no libraries): live time zone clocks, mobile menu, active section highlighting, scroll reveal and bounce-in effects, counting numbers, portrait tilt, auto-sizing contact form |
| Fonts | Google Fonts: Bricolage Grotesque (headings), Hanken Grotesk (body), JetBrains Mono (labels) |
| Images | WebP and JPEG photos, SVG and PNG logos |
| App install | Web app manifest and a service worker (Progressive Web App), so it can be added to a home screen and opens like an app |
| Link previews | Open Graph and Twitter Card tags with a 1200 x 630 preview image |
| Contact form | Embedded Gallagher's Resource form that reports its height to the page, so it always fits without scrolling or cutting off |
| Hosting | Any static host (Vercel, Netlify, GitHub Pages). No server or database needed |

## What is in this folder

| File or folder | What it is |
|---|---|
| `index.html` | The whole page: text, layout, colors and animations |
| `img/` | Profile photo, project images, client logos and tool logos |
| `og.jpg` | The preview image shown when the link is shared on Instagram, Facebook, Messenger, WhatsApp, iMessage and LinkedIn |
| `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png` | App icons, used when someone adds the site to their home screen |
| `manifest.webmanifest`, `sw.js` | Let the site install like an app on phones and computers |
| `img/form-banner.png` | The 1800 x 600 banner used at the top of the contact form |

## Step 1: Put the code on GitHub

1. Create a free account at github.com and sign in.
2. Click the **+** button at the top right, then **New repository**.
3. Name it (for example `anthony-marquez-website`), leave everything else as is, and click **Create repository**.
4. On the next screen, click **uploading an existing file**.
5. Open this folder on your computer, select everything inside it (all files and the `img` folder), and drag it into the browser window.
6. Click **Commit changes**.

Your code is now saved on GitHub.

## Step 2: Put the website online

The easiest free option is Vercel.

1. Go to vercel.com and click **Sign Up**, then **Continue with GitHub**.
2. Click **Add New**, then **Project**.
3. Find the repository you just created and click **Import**.
4. Leave every setting as it is. There is no build command and no framework to choose.
5. Click **Deploy**.

After about a minute, Vercel gives you a working link (something like `anthony-marquez-website.vercel.app`). The site is live.

From now on, any change you save on GitHub updates the live site automatically.

## Step 3: Connect your own domain

1. Buy a domain from any registrar (for example Namecheap, GoDaddy, Squarespace or Cloudflare), such as `anthonymarquez.com`.
2. In Vercel, open your project, then **Settings**, then **Domains**.
3. Type your domain and click **Add**.
4. Vercel shows one or two DNS records. Log in to your registrar, open the DNS settings for your domain, and add those records exactly as shown.
5. Wait a few minutes (sometimes up to a few hours). Vercel shows a green check when the domain is connected, and it turns on HTTPS for you.

## Step 4: Tell the page its new address

This makes link previews on social media and messaging apps show the right image and title.

1. On GitHub, open your repository and click `index.html`.
2. Click the pencil icon to edit.
3. Press Ctrl+F (Cmd+F on a Mac) and search for `YOUR-DOMAIN.com`.
4. Replace every match with your real address, for example `https://anthonymarquez.com`. There are a few matches near the top of the file.
5. Click **Commit changes**. Vercel updates the live site within a minute.

To check the preview, paste your link into the Facebook Sharing Debugger (developers.facebook.com/tools/debug) and click **Scrape Again**.

## The contact form

The contact form already works. You do not need to set anything up.

The form is hosted by Gallagher's Resource and loads from this link inside the page:

`https://reports.gallaghersresource.com/f/gallaghers-resource/anthony-marquez`

As long as `index.html` keeps that same link, the form shows on your site, sizes itself to fit, and every message is delivered to you, on any domain you use. Do not change or remove that link.

## Editing the content

Everything is in `index.html`. On GitHub, open the file, click the pencil icon, find the text you want to change, edit it, and click **Commit changes**. The live site updates on its own.

The sections, from top to bottom, are: intro, skills band, results, About, Work, Tools, Testimonials and Contact.

To change a photo, upload a new image to the `img` folder with the same file name as the one you are replacing. Keep photos under about 300 KB so the page stays fast.

## Other places you can host it

Any static hosting works with these same files, for example Netlify (drag the folder onto app.netlify.com) or GitHub Pages (in your repository, **Settings**, then **Pages**, then choose the main branch).
