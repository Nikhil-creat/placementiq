# PlacementIQ

AI-powered mock interview trainer for Indian tech placements. Generates resume-aware
interview questions and scores answers instantly using Claude.

## Designed and Developed by 
# **NIKHIL CHARY SRIRAMOJU**
BTech CSE (Final Year)

- GitHub: [Nikhil-creat](https://github.com/Nikhil-creat)
- LinkedIn: [nikhil-chary-sriramoju](https://in.linkedin.com/in/nikhil-chary-sriramoju-95041b38a)
- Email: sriramojunikhil66@gmail.com
- Instagram: [@nikhil__sriramoju](https://www.instagram.com/nikhil__sriramoju)
- Facebook: [Profile](https://www.facebook.com/profile.php?id=100079201124141)

## Structure
- `index.html` — landing / marketing page (this is what people see first)
- `app.html` — the actual tool (resume upload → mock interview → scoring)

## How it works (Phase 1 — no backend)
The app calls the Claude API **directly from the user's browser** using their own
API key, which is stored only in their browser session. This is why it works on
GitHub Pages with **zero hosting cost** — there is no server.

## Deploy to GitHub Pages

1. Create a new repo on GitHub, e.g. `placementiq`.
2. Unzip this project and push it:
   ```bash
   cd placementiq
   git init
   git add .
   git commit -m "PlacementIQ Phase 1"
   git branch -M main
   git remote add origin https://github.com/<your-username>/placementiq.git
   git push -u origin main
   ```
3. On GitHub: go to the repo → **Settings → Pages** → under "Build and deployment",
   set Source = `main` branch, folder = `/ (root)` → Save.
4. Wait ~1 minute. Your site is live at:
   `https://<your-username>.github.io/placementiq/`

## Monetization path

### Stage 1 (now): Bring-your-own-key, free
- Launch as-is. Zero cost to you. Goal: get 50-100 users, testimonials, feedback.
- Share on LinkedIn (build-in-public posts), r/developersIndia, college placement
  WhatsApp/Telegram groups, your college's T&P cell.

### Stage 2: Paid "Placement Pass" (manual, no code needed yet)
- Advertise ₹399 for 3-month unlimited access + weak-topic tracking.
- Collect payment via a simple Razorpay Payment Link (no coding — create one free
  at razorpay.com/payment-links) or UPI, then manually email/WhatsApp the buyer
  your shared API key or an invite.
- This validates people will actually pay BEFORE you build a full backend.

### Stage 3: Real SaaS (Phase 2 build)
- Add Supabase auth + a credits table so YOU hold one Claude API key server-side
  and users no longer need their own.
- Add Razorpay Checkout integration for self-serve payment (no manual work).
- Deploy the backend as a Supabase Edge Function (free tier) — GitHub Pages still
  hosts the frontend, Supabase handles auth/payments/API calls.
- This is what turns it from "cool project" into a real recurring-revenue product.

### Distribution checklist (do this in parallel with building)
- [ ] Post progress on LinkedIn 2-3x/week (screenshots, metrics, learnings)
- [ ] Post on r/developersIndia, r/Btechtards
- [ ] Get 5 friends to test it and give testimonials
- [ ] Approach your college T&P cell — offer free batch access for feedback
- [ ] Launch on Product Hunt once Stage 2 is stable
- [ ] Target October–December (placement season) — speed beats polish right now

## Next step
Once Stage 1 has real users and Stage 2 has at least one paying customer, come back
and we build Phase 2 (Supabase auth + Razorpay + credits system).
