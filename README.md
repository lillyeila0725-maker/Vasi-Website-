# Vasi's Cursive Writing & Grammar Learning: website

A single-file, scroll-animated website (`index.html`) with no build step and no backend.

## What's inside
- **Scroll story hero** (modelled on the reference video): one sheet of four-line copybook paper changes over 5 stages as you scroll: basic strokes → letters → a joined cursive word → a grammar correction in red pen → the "Vasi's" signature. The headline changes per stage, the backdrop goes dark for the middle stages (like the "Baked to rise" part of the reference), and there are dot indicators.
- Stats band (5.0 rating · 23 reviews · open 24 hrs)
- Two course cards (Cursive Handwriting, English Grammar)
- 5-step method with self-drawing line icons
- Before/after drag slider (labelled as an illustration)
- "See your name in cursive": visitors type a name and watch it written out
- Photo gallery (stand-in photos, each tagged "Sample photo")
- The 3 real Google reviews, quoted as written, with a link to all 23
- Address, phone, hours, Google Map embed, WhatsApp enquiry form
- Floating call button, mobile menu, reduced-motion support

## Deploy (pick one, about 2 minutes each)
**Netlify Drop (easiest):** go to https://app.netlify.com/drop and drag the whole `vasis-website` folder onto the page. You get a live URL right away.

**Vercel:** `npm i -g vercel` → run `vercel` inside this folder → accept the defaults → `vercel --prod`.

**GitHub Pages:** push this folder to a repo (e.g. `nikitha2525/vasis-website`), then Settings → Pages → Branch `main` / root. The site will be at `https://nikitha2525.github.io/vasis-website/`.

**Custom domain:** buy e.g. `vasiscursive.in`, then add it under Netlify/Vercel → Domains and follow the DNS steps they show.

## Before going live: replace and confirm with the client
1. **Photos:** all 7 images are free Unsplash stock photos used as stand-ins. Put real photos in `images/` (class in progress, students writing, notebooks, before/after pages, the teacher, the centre's entrance), then change each `src="https://images.unsplash.com/..."` to `src="images/your-photo.jpg"`. After that, delete the `<span class="sample">Sample photo</span>` tags. Each slot is marked with a `PHOTO SLOT` comment.
2. **Before/after:** this is currently an illustration made with two fonts. Swap in scans of a real student's pages (with the parents' permission).
3. **WhatsApp:** the enquiry form opens WhatsApp chat with **+91 93445 57559**. Confirm that this number uses WhatsApp, or change `PHONE` in the script.
4. **Content to confirm:** course module lists, age groups, batch timings, fees (not included on purpose), the teacher's full name and qualifications, and whether there's an online option (one review mentions "this website… tutorials").
5. **Reviews:** these are quoted from the public Google listing. Get the owner's OK before launch, and update the count as more reviews come in.

## Fonts
Playfair Display (headlines), Manrope (body), Playwrite IN (cursive; it was designed for teaching handwriting in India), with Dancing Script as a fallback. All are loaded from Google Fonts.
