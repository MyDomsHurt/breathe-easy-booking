# Breathe Easy HK — Booking Page Context

## Project Overview
This is a **sophisticated, minimalist booking/quote page** for **Breathe Easy HK**, a premium air conditioning cleaning service in Hong Kong.

The goal is to create a high-quality, trustworthy-feeling web page that allows customers to request a quote for AC cleaning by selecting specific unit types, preferred time windows, and district. It is **not** a same-day booking system.

**Important Philosophy:**
- Honest and realistic communication (no fake urgency)
- Premium, calm, professional design
- Clear that this is a **quote request**, not an instant booking
- Responses happen during office hours only

## Current Technical Setup
- **Single file website**: `index.html` + `assets/` folder
- Uses **Tailwind CSS via CDN** (no build process)
- All images are in the `assets/` folder (real assets pulled from the client's original site)
- No backend — form data is collected client-side and sent via WhatsApp (pre-filled message)

## Key Features Currently Implemented

### Unit Selection
- Users can select quantities for 5 different unit types:
  - Split Units ($900)
  - Window Units ($600)
  - Cassette Units ($1,400)
  - Built-in / Ducted ($1,100)
  - Under-Ceiling ($1,100)

### Pricing & Discounts
- Live pricing calculation
- Volume discount system:
  - 5% off for every full $2,000 in subtotal
  - Capped at 15% maximum discount
- Invoice-style breakdown in the sidebar summary

### Location & Scheduling
- Detailed district selector covering all of Hong Kong (with optgroups)
- No full address field (kept simple — exact address collected later via WhatsApp)
- Time windows (no evenings):
  - Morning: 9:00 – 12:00
  - Afternoon: 12:00 – 15:00
  - Late afternoon: 3:00pm – 5:30pm

### Messaging & Tone
- "This is a quote" positioning (not instant booking)
- Office hours clearly stated: Monday–Friday, 8am – 5:30pm
- Realistic lead times: "Current waiting period: 2–3 weeks"
- "Trusted by thousands of families in Hong Kong"
- Removed all fake urgency ("same day", "responds in minutes", etc.)

### Design & Branding
- Colors: Deep royal blue (#1F4088) + Cyan accent (#68C8F0)
- Clean, premium, minimalist aesthetic
- Uses real photography and logo from the client's existing website

## What Was Intentionally Removed / Changed
- Preferred date field (now "Flexible date")
- Full address textarea
- Same-day / next-day claims
- Fake fast response times
- Low urgency numbers (e.g. "only 12 families booked this week")
- "Instant confirmation" language

## Best Prompts for Future Work

### Master Context Prompt (Use this when starting a new Grok session)

```
You are helping me develop a premium booking/quote page for Breathe Easy HK, an aircon cleaning company in Hong Kong.

Project context:
- Single-file HTML site using Tailwind via CDN
- Design must stay sophisticated, calm, minimalist, and trustworthy
- Branding uses deep blue (#1F4088) and cyan (#68C8F0)
- We use real assets from their existing website
- This is a quote request flow, not instant booking
- Responses only during office hours (Mon–Fri 8am–5:30pm)
- Current lead time is 2–3 weeks
- We have removed all fake urgency and unrealistic promises

Current state:
- Detailed unit type selector with per-unit pricing and volume discounts
- District selector covering all of Hong Kong
- No preferred date field (flexible)
- No full address field
- Strong emphasis on honest communication

Please read the current index.html and CONTEXT.md first. Once you understand the project, confirm you have the context and ask what I want to work on.
```

### Good Follow-up Prompts

**For design/UX improvements:**
```
Review the current Breathe Easy HK booking page from a conversion and user experience perspective. Suggest the highest-impact improvements while staying true to the premium, honest tone we've established.
```

**For adding new features:**
```
I want to add [feature idea]. Given the current structure (single HTML file + Tailwind CDN), how would you recommend implementing it while keeping the code clean and maintainable?
```

**For copywriting / messaging:**
```
Review the current messaging on the Breathe Easy HK booking page. Suggest more polished, trustworthy alternatives, especially around the quote nature of the form and lead times.
```

**For writing customer emails:**
```
You are an expert email writer for Breathe Easy HK, a premium air conditioning cleaning company in Hong Kong.

Core principles for every email:
- Tone: Calm, professional, honest, and premium (never pushy, hype-filled, or overly salesy)
- Be realistic about timing — we respond during office hours only (Monday to Friday, 8:00am – 5:30pm) and current lead times are typically 2–3 weeks
- This is a quote-based service. We do not offer same-day or instant bookings
- Always sound trustworthy and low-pressure
- Reference the new online quote tool (https://mydomshurt.github.io/breathe-easy-booking/) when it makes sense
- Include the WhatsApp number clearly: +852 9887 7273

When writing emails:
- Keep them relatively concise and well-structured
- Use a warm but professional greeting
- Clearly state next steps
- Offer to answer questions via WhatsApp
- Provide 2–3 variations when asked (e.g. shorter vs more detailed, or different levels of warmth)

Current situation / customer context:
[Insert details here — e.g. what units they selected, any notes from their quote request, whether they’ve already been contacted, etc.]

Write a [follow-up / confirmation / marketing / re-engagement] email for the above situation.
```

## Recommended Next Steps on a New Computer

1. Unzip the project folder.
2. Open `index.html` in a browser to view it.
3. Start a new chat with Grok.
4. Paste the **Master Context Prompt** above.
5. Then describe what you want to work on.

## Notes for Future Development

- Keep the single-file + Tailwind CDN approach unless there's a strong reason to move to a framework.
- Any new features should respect the honest, premium tone.
- When in doubt, prioritize clarity and professionalism over conversion tricks.

---
Last updated: May 2025 (added strong email writing prompt)
