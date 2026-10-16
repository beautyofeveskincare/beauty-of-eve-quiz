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
- `treatment` must be one of: `hifu`, `thread`, `filler`, `lip`, `body`, `rf`, `laser`, `hydra`, `exo`, `lhr`.
- A deal shows when the quiz suggests that treatment, either as the main pick or as the second option.
