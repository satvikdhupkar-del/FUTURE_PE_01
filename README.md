# AI Website Copy Generator — Sawariya Mobile Shopee

**Task:** Prompt Engineering Task 1 (2026) — Future Interns
**Submitted by:** [Your Name]

## 🏪 Business Chosen

**Sawariya Mobile Shopee** — a local mobile phone shop in Bibwewadi, Pune, offering phone sales, repairs, diagnostics, SIM activation, and mobile accessories.

- 📍 Shop No. 4, 658/8/6, Opp Vinayak Sweets, Upper Kondhawa Rd, Bibwewadi, Pune, Maharashtra 411037
- 📞 +91 77448 83919
- 🕒 Open all 7 days, 10:00 AM – 10:00 PM

This business was chosen because it's a common but underserved local business type — a neighborhood mobile shop with a real, slightly unusual constraint: **services are in-store only, while physical products can be delivered across the city.** That constraint made it a good test case for writing copy that's specific and non-generic rather than a template that could apply to any shop.

## 🧠 Prompt Logic

The prompt system is split into a **master context prompt** (business facts, tone, and the critical in-store-vs-delivery distinction) followed by **task-specific prompts** for each content block:

1. Homepage copy (headline, sub-headline, intro, CTAs)
2. Services page (per-service breakdown, in-store-only banner)
3. Products/shop page (delivery-across-Pune framing)
4. CTA sections (repair booking, product ordering, contact/location)
5. Testimonials intro

Reusing the same master context across every prompt kept the tone and facts consistent, while each task-specific prompt narrowed the ask to one content block at a time — making the system easy to adapt to a different local business by just swapping the context block.

The core design decision throughout: **never let repair-service language and delivery language blur together**, since that's the single detail most likely to create a bad customer experience if the copy were wrong (someone expecting doorstep repair pickup).

## 🤖 Tool Used

**Claude** (claude.ai) — used to generate all homepage, services, product, and CTA copy from the structured prompts in [`prompts.md`](./prompts.md).

## 📁 Repo Contents

| File | Description |
|---|---|
| `prompts.md` | The structured, reusable prompts used to generate the copy |
| `generated-website-copy.md` | The final AI-generated homepage, services, products, and CTA copy |
| `README.md` | This file |

## 🌐 Next Step

This copy is structured to be dropped directly into a website builder such as [Lovable](https://lovable.dev) to scaffold a live site for the business.
