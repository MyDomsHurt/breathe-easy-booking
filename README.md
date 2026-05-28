# Breathe Easy HK — Booking Page

A sophisticated, minimalist booking experience that mirrors the premium branding of breathe-easyhk.com.

## Design direction
- Deep royal blue (#1F4088) + fresh cyan accent (#68C8F0) from your logo
- Generous whitespace, refined typography, and calm luxury feel
- Custom hero photography tailored to the "fresh, clean, peaceful home" aesthetic
- Live price calculator + elegant WhatsApp-first flow

## How to customize pricing (very easy)
Open `index.html` and find this block near the top of the `<script>`:

```js
const UNIT_PRICES = {
  split: 900,        // Split / Wall-mounted units
  window: 600,       // Window units
  cassette: 1400,    // Cassette units
  builtin: 1100,     // Built-in / Ducted units
  underceiling: 1100 // Under-ceiling units
}
```

Change any of the per-unit prices. The live summary and WhatsApp message will update automatically with the correct breakdown.

## Volume Discount Rule
The page automatically applies your volume discount:
- Every full $2,000 → 5% off
- Maximum discount = 15%

Example:
- $2,700 subtotal → 5% discount → $2,565
- $4,500 subtotal → 10% discount → $4,050
- $7,200+ subtotal → capped at 15% discount

The discount is clearly shown in the summary, confirmation modal, and pre-filled WhatsApp message.

## How the booking flow works
1. User fills the beautiful form
2. On submit → elegant success modal appears with reference number
3. Big green "Message us on WhatsApp" button constructs a perfectly formatted message with all details
4. One tap opens WhatsApp with everything pre-filled

This converts extremely well for service businesses.

## Future upgrades you can ask for
- Add a "Deep Clean" upsell toggle (+$380)
- Real backend submission (Formspree, Make.com, email, etc.)
- Multiple service types
- Calendar integration
- Move this exact design into Next.js + Tailwind + shadcn

## Files
- `index.html` — The complete standalone page
- `assets/logo.svg` — Official Breathe Easy logo (directly from their site)
- `assets/team-photo.jpg` — Main hero image from breathe-easyhk.com
- `assets/family-1.png`, `family-2.png`, `family-3.png` — Authentic family lifestyle photos from their guarantees section

All visuals now come from the original website for brand accuracy.

Built to feel expensive, trustworthy, and calm — exactly like your brand.
