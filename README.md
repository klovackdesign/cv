# klovackdesign — standalone site

Plain HTML/CSS/JS. No build step, no framework. Fonts load from Google Fonts.

## Files
- `index.html`  – the whole site (styles + script inside)
- `portrait.jpg` – your hero photo
- `images/`     – put your portfolio images here

## Publish it (free options)
**Cloudflare Pages** or **Netlify**: create an account, choose "upload / drag & drop", drop this whole folder
(or the .zip). You get a live `*.pages.dev` / `*.netlify.app` address in about a minute.

## Attach your domain
1. Buy a domain (Namecheap, Porkbun, Cloudflare Registrar…).
2. In your host's dashboard open **Custom domains → Add domain** and type it in.
3. The host shows the DNS records to create (usually an A/ALIAS record for the bare domain and a CNAME for `www`).
   Add them at your registrar (or switch the domain's nameservers to Cloudflare if you use Cloudflare Pages).
4. Wait a few minutes to a few hours. HTTPS is enabled automatically.

## Add your real portfolio work
Open `index.html`, find `imgs:` in the three categories (ui / email / ads) and list your files in the same order
as the `works` list above each one, e.g. `imgs: ['images/ui-1.jpg', 'images/ui-2.jpg', ...]`.
The same images fill the category previews, the popups and the collage behind "Discuss Project".
Use JPG/WebP, about 1200px wide.

## Contact form
By default, after the visitor passes the anti-spam question, a button opens their email app with the
message prefilled for yurii.klovak@gmail.com.
To get messages delivered automatically: create a free form at formspree.io (or a similar service) and paste its
URL into `FORM_ENDPOINT` near the top of the script in `index.html`.

## Still placeholders
About-me paragraphs, testimonials ("[Client name]" etc.) and project names are placeholders — search for the
square brackets in `index.html` and replace them.
