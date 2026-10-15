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

## Contact form (delivers straight to your inbox)
The form sends each message to yurii.klovak@gmail.com through FormSubmit (formsubmit.co), a free relay, and
shows the visitor a "message sent" confirmation. If the automatic send ever fails, the visitor gets a button that
opens their email app with the message prefilled, so nothing is lost.

**One-time activation (required):**
1. Put the site online (it won't send from a file opened on your computer or from the design editor).
2. Fill in and submit the form once yourself.
3. FormSubmit emails yurii.klovak@gmail.com a confirmation link (check Spam/Promotions). Click it.
4. From then on every message arrives in your inbox. Reply goes straight to the sender.
5. Recommended: FormSubmit also emails you a random alias. In `index.html`, change the line
   `var FORM_ENDPOINT = 'https://formsubmit.co/ajax/' + EMAIL;` to
   `var FORM_ENDPOINT = 'https://formsubmit.co/ajax/<your-random-alias>';` so your address isn't visible to spam bots.

Note: messages pass through FormSubmit's servers before reaching you.

## Still placeholders
About-me paragraphs, testimonials ("[Client name]" etc.) and project names are placeholders — search for the
square brackets in `index.html` and replace them.
