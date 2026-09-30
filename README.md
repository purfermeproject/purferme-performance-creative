# Puŕ Ferme Project — Performance Creative Framework

> **Consciously Sourced. Passionately Crafted.**
> An internal operating system for making ads that sell familiar food made with better ingredients, without preaching, scaring people or overclaiming.

This repo is the playbook our team (marketers, designers, editors, UGC creators and AI tools) uses to plan, write, shoot, test and iterate every paid ad.

Every ad has to answer one question:

> **Why would this exact customer stop scrolling, care, believe us, and take the next step?**

If a brief can't answer all four parts of that question (**stop**, **care**, **believe**, **act**), it doesn't go into production.

---

## How to use this repo

| If you are… | Start here |
|---|---|
| New to the brand | [`final-output/01-framework-one-page.md`](final-output/01-framework-one-page.md), then [`12-claims-guardrails.md`](12-claims-guardrails.md) |
| Writing a brief | [`10-creative-brief-template.md`](10-creative-brief-template.md) |
| Writing hooks | [`06-hook-engine.md`](06-hook-engine.md) |
| Scripting UGC | [`04-ugc-script-system.md`](04-ugc-script-system.md) |
| Designing statics | [`05-static-ad-system.md`](05-static-ad-system.md) |
| Using an AI tool | [`11-ai-prompt-template.md`](11-ai-prompt-template.md) |
| Running Meta tests | [`08-creative-testing.md`](08-creative-testing.md) and [`09-winner-iteration.md`](09-winner-iteration.md) |
| Approving an ad | [`final-output/09-approval-checklist.md`](final-output/09-approval-checklist.md) |

## Structure

| # | File | What it answers |
|---|---|---|
| 1 | [`00-master-framework.md`](00-master-framework.md) | The 15-step persuasion sequence every ad draws from |
| 2 | [`01-consumer-tensions.md`](01-consumer-tensions.md) | The 38 real-life tensions we start ads from |
| 3 | [`02-angle-library.md`](02-angle-library.md) | 35 creative angles, fully built out |
| 4 | [`products/`](products/) | One framework per product (they are **not** the same campaign) |
| 5 | [`04-ugc-script-system.md`](04-ugc-script-system.md) | Timed script templates for 15/30/45/60s, plus product-reveal rules |
| 6 | [`05-static-ad-system.md`](05-static-ad-system.md) | 17 static formats with layouts and copy rules |
| 7 | [`06-hook-engine.md`](06-hook-engine.md) | 15 hook categories, 10+ hooks each |
| 8 | [`07-creative-multiplication.md`](07-creative-multiplication.md) | Turning one piece of footage into many *meaningful* ads |
| 9 | [`08-creative-testing.md`](08-creative-testing.md) | Meta testing on a growing-brand budget, and diagnosing failures |
| 10 | [`09-winner-iteration.md`](09-winner-iteration.md) | Keep / kill / modify / expand / reshoot decision tree |
| 11 | [`10-creative-brief-template.md`](10-creative-brief-template.md) | Fill-in-the-blank brief |
| 12 | [`11-ai-prompt-template.md`](11-ai-prompt-template.md) | Reusable prompt for Claude / ChatGPT / Gemini |
| 13 | [`12-claims-guardrails.md`](12-claims-guardrails.md) | Red / yellow / green claims system |
| — | [`13-verification-register.md`](13-verification-register.md) | Every fact we have **not** yet verified. Check it before using a claim. |
| 14 | [`final-output/`](final-output/) | One-pager, product matrix, territories, top 50 hooks, first 10 ads, 30-day roadmap, checklist |

## Products covered

| Product | Framework |
|---|---|
| Millet & Oats Breakfast Cookies | [`products/01-millet-oats-breakfast-cookies.md`](products/01-millet-oats-breakfast-cookies.md) |
| Millets & Oats Chocolate Cookies | [`products/02-millets-oats-chocolate-cookies.md`](products/02-millets-oats-chocolate-cookies.md) |
| Unsweetened Peanut Butter | [`products/03-unsweetened-peanut-butter.md`](products/03-unsweetened-peanut-butter.md) |
| Ragi & Cocoa Spread with Jaggery | [`products/04-ragi-cocoa-spread.md`](products/04-ragi-cocoa-spread.md) |
| Sunrise Bowl Sprouted Ragi & Sweet Potato Porridge | [`products/05-sunrise-bowl-porridge.md`](products/05-sunrise-bowl-porridge.md) |
| PurGro bars and future products | [`products/06-purgro-and-future-products.md`](products/06-purgro-and-future-products.md) |

## The non-negotiables

1. **Taste first, then ingredients.** We sell food people want to eat. Ingredients are the reason to trust it, not the reason to buy it.
2. **Show the back of the pack.** Transparency is our proof. If we can't show it, we don't claim it.
3. **No fear, no preaching, no medicine.** We don't scare people about other brands' foods, lecture anyone, or promise health outcomes.
4. **Never invent facts.** Anything in [`13-verification-register.md`](13-verification-register.md) stays out of ads until it has been verified.
5. **Warm, modern, Indian, slightly playful.** We're the friend who reads labels, not the one who judges your plate.

## Contributing

- Put new winning hooks, angles and learnings in the relevant file, with the date and test result.
- Record every test in `learnings/` (create it at your first test) using the log format in [`08-creative-testing.md`](08-creative-testing.md#9-the-learning-log).
- When a fact is verified, move it from the verification register into the product file and note the source (pack photo, lab report, etc.).
