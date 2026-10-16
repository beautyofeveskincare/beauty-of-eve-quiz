# Beauty of Eve Skin Quiz

A 4-question skin quiz for Beauty of Eve Skincare (20 Eglinton Ave E, Unit 403, Toronto).
Visitors answer questions about their skin goals, get a suggested treatment, and book a free consultation.

- `index.html` — the quiz page
- `deals.json` — this month's deals, shown on the result screen

## Updating the monthly deals

At the start of each month, change `deals.json`:

```json
{
  "month": "2026-11",
  "headline": "November Glow-Up",
  "deals": [
    { "treatment": "filler", "text": "Juvéderm $549 per syringe (reg. $699)" },
    { "treatment": "hydra",  "text": "Hydra Facial + Contouring $149" }
  ]
}
```

- `month` must be the current month (YYYY-MM). Deals from any other month are hidden automatically.
- `treatment` links the deal to a treatment so it also shows on the quiz result. Leave it out for a general offer (it then shows only on the start screen).
- All deals are listed on the quiz's start screen. A deal with a `treatment` also shows on the result screen when the quiz suggests that treatment, as the main pick or the second option.

| Key | Treatment |
|---|---|
| `botox` | Anti-Wrinkle Injections (Botox) |
| `filler` | Dermal Fillers |
| `lip` | Lip Filler |
| `hifu` | HIFU Face Lift |
| `thread` | Thread Lift |
| `endolift` | Endolift |
| `rf` | RF Microneedling |
| `micro` | Microneedling |
| `laser` | Fractional Laser |
| `subcision` | Subcision |
| `pigment` | Hyperpigmentation Treatment |
| `vascular` | Vascular Lesion Treatment |
| `booster` | Skin Booster |
| `salmon` | Salmon DNA (Polynucleotides) |
| `hydra` | Hydra Facial + Contouring |
| `fatdis` | Fat Dissolving Injections |
| `skintag` | Skin Tag Removal |
| `body` | Body & Butt Filler |
| `contour` | Body Contouring |
| `cellulite` | Cellulite Reduction |
| `stretch` | Stretch Mark Reduction |
| `bodyfirm` | Body Skin Firming |
| `vaginal` | Vaginal Tightening |
| `lhr` | Laser Hair Removal |
| `exo` | Exosome Therapy |
| `prp` | PRP Hair Treatment |
| `iv` | IV Therapy |
