# Part 9 — Creative Testing System (Meta)

Written for a **growing D2C brand with a finite budget**. The aim is to learn the most per rupee, not to run a perfect experiment.

> **On benchmarks:** This document deliberately avoids universal "good CTR = X%" numbers. Food D2C in India varies too much by product price, audience, placement and season. Every judgement is **relative**: this creative vs our own account baseline, vs the current best ad (the "control"), and vs its siblings in the same test. Section 4 explains how to build that baseline.

---

## 1. Definitions

| Term | Definition |
|---|---|
| **Concept** | A distinct **message** = one tension + one angle + one core argument. "Keep the chai" and "Four things we left out" are two concepts, even for the same product. |
| **Execution** | One way of making a concept: a UGC video, a static, a carousel, a founder video. The same concept can have several executions. |
| **Variant** | A change to the entry point of an execution (hook, first frame, length, CTA, caption). See [Part 8](07-creative-multiplication.md). |
| **Control** | The current best-performing ad for that product/audience. Every new test is compared against it. |
| **Winner** | A new ad that beats the control on the primary metric at an acceptable CPA, with enough data to trust it. |

**Rule:** Test *concepts* first, *executions* second, *variants* third. Most learning comes from testing concepts.

---

## 2. Account structure (lean)

| Campaign | Purpose | Budget share (guideline) |
|---|---|---|
| **Testing** | New concepts and variants | ~20–30% of spend |
| **Scaling** | Proven winners only (graduated from testing) | ~60–70% |
| **Retargeting** *(optional, if audience size allows)* | Site visitors, video viewers, ATC | ~10% |

**Testing campaign set-up:**
- One ad set per **concept** (or per product, if budget is very tight), so each concept gets its own budget and results can't be hidden by one ad taking all the spend.
- 2–4 ads per ad set (the hook/frame variants of that concept).
- Broad targeting (India, relevant age range, relevant geos/cities), because modern Meta delivery finds the audience through the creative. Keep the audience **the same across concepts in a test** so that creative is the only variable.
- One optimisation event for the whole test: **Purchase** if the pixel has enough purchase volume, otherwise **Add to Cart** as a proxy until volume grows. *(What counts as "enough" depends on your weekly purchase volume; review with your media buyer.)*
- Winners graduate to scaling campaigns **as new ads using the existing post ID**, which preserves the social proof (likes, comments).

---

## 3. How much to launch, and how long to wait

### Batch size
| Monthly Meta budget (guideline) | Concepts per batch | Variants per concept | Ads per batch |
|---|---|---|---|
| Small | 2–3 | 2 | 4–6 |
| Medium | 3–5 | 2–3 | 6–15 |
| Larger | 5–8 | 3 | 15–24 |

**The binding constraint is spend per ad, not the number of ideas.** Each ad needs enough spend to produce a readable signal. A working rule:

> **Minimum test spend per concept ≈ 2–3× your target CPA** (split across its variants).
> Early attention signals (hook rate, hold rate, CTR) become readable much sooner, typically after a few thousand impressions per ad.

If budget can't give every concept 2–3× target CPA in a week, **launch fewer concepts**. Five half-tested concepts teach you less than two fully tested ones.

### How long to wait
| Signal | When it becomes readable | Decision it supports |
|---|---|---|
| Hook rate, hold rate | ~2–3 days / a few thousand impressions per ad | Kill or keep a **hook** |
| CTR (link) | ~3–4 days | Is the **message** motivating action? |
| LPV rate, ATC rate | ~4–7 days | Are the **landing page** and **offer** working? |
| Purchases, CPA, ROAS | ~7 days minimum, and only once spend ≥ 2–3× target CPA | Keep, scale or kill the **concept** |

**Don't judge in the first 24–48 hours** unless an ad is catastrophically bad (e.g. hook rate far below every sibling with meaningful impressions). Meta's early delivery is noisy.

**Don't touch a test while it runs.** Editing an ad resets its learning. Pause and relaunch instead.

---

## 4. The metrics, and how to judge them relatively

### Build a baseline first
Before judging anything, calculate for **your own account, per product**, using the last 30–60 days:
- the **median** of each metric across all ads with meaningful spend
- the **control ad's** value for each metric

Then judge every new ad as:
- **Above control** → a potential winner
- **Between median and control** → promising; iterate
- **Below median** → a weak signal on that metric

Recalculate baselines monthly. They move with seasonality (festive periods, school terms) and rising CPMs.

### The metric chain
Each metric measures one link in the chain from scroll to purchase. **The first weak link is where the problem is.**

| # | Metric | Formula | What it tells us | Mainly driven by |
|---|---|---|---|---|
| 1 | **Hook rate (thumb-stop)** | 3-second video plays ÷ impressions | Did the first frame + hook stop the scroll? | First frame, hook, sound-off legibility |
| 2 | **Hold rate** | ThruPlays (or 15s views) ÷ 3-second plays | Did the body keep them after the hook? | Pacing, story, relevance of body to hook |
| 3 | **CTR (link)** | Link clicks ÷ impressions | Did the ad make them want to act? | Message, proof, CTA, desire |
| 4 | **LPV rate** | Landing page views ÷ link clicks | Did the page actually load for them? | Page speed, accidental clicks |
| 5 | **ATC rate** | Add-to-carts ÷ landing page views | Did the page and offer convert interest? | Page, price, pack size, offer, message match |
| 6 | **Checkout / purchase rate** | Purchases ÷ ATC | Did the checkout close the sale? | Shipping cost, COD availability, checkout friction, trust |
| 7 | **CPA** | Spend ÷ purchases | Cost to acquire a customer | Everything above plus CPM |
| 8 | **ROAS** | Revenue ÷ spend | First-order efficiency | CPA plus AOV |

**For statics:** skip hook and hold rates. Use **CTR** as the attention-and-intent signal, and **CPM** as a rough read of how Meta rates the ad's quality and relevance.

### Judging principles for a food brand
- **First-order ROAS understates food.** Our products are consumables with repeat potential. Judge winners on CPA against a **target CPA derived from contribution margin and expected repeat rate** *(requires internal data: AOV, margin, 60/90-day repeat rate)*. Don't use a blanket ROAS target.
- **Different products, different baselines.** A ₹X jar of PB and a ₹Y pack of cookies have different price points, AOVs and funnels *(pricing: verify)*. Never compare a PB ad's CPA to a cookie ad's CPA.
- **A high CTR on a meme is not the same as a high CTR on a label ad.** Memes attract curious clicks; label ads attract intent. Compare within the format first.
- **Watch the ratio, not just the number.** A hook rate 1.5× the account median with a hold rate at median is a clear "hook works, body is fine" signal, whatever the absolute values are.

### Creative fatigue
Fatigue is when a **previously winning** ad declines because the audience has seen it enough.

**Signals (look for 2+ together, over 5–7 days):**
- Frequency rising (in prospecting, especially past ~3–4 over 7 days for a mid-size audience; *calibrate to your account*)
- Hook rate and CTR declining vs the ad's own first two weeks
- CPM rising while CTR falls
- CPA rising steadily, not just a noisy day

**Response:**
1. **Refresh the entry point** first: a new hook and first frame on the same body (Part 8, stage 1). This is the cheapest fix.
2. **New execution** of the same concept (a new creator, a new setting).
3. Only then **retire the concept**, and keep it in the learning log for a later revival.

**Reduce fatigue by design:** keep 3–5 winning concepts live at once, not one hero ad.

---

## 5. Diagnosis: what's actually broken?

Read the metric chain left to right. The first link that falls clearly below baseline is the likely problem.

| Problem | Symptom pattern | How to confirm | Fix |
|---|---|---|---|
| **Bad hook** | Low hook rate vs siblings and baseline; the rest of the chain may be fine for the few who stayed | The same body with a different hook performs better | New hook/first frame (Part 8, stage 1) |
| **Bad body** | Good hook rate, **low hold rate**; CTR low | Retention graph drops sharply right after the hook, or at one specific moment | Tighten pacing, bring taste proof earlier, remove the slow segment, check the body delivers what the hook promised |
| **Bad offer / price** | Good CTR, good LPV, **low ATC** across **multiple different creatives** for the same product | Session recordings show price-checking and exits; low ATC for this product even with the best ad | Test a trial size, bundle or introductory offer *(business decision)*, clarify price per unit/serving on the page |
| **Bad landing page** | Good CTR, **low LPV rate** (load issue) or low ATC (content issue); problem occurs for **all ads** to that page | Page speed test; compare the same ad to a different landing page | Speed, above-the-fold product and price, match headline to ad message, show the back of the pack on the page, reviews, clear CTA |
| **Message–page mismatch** | Good CTR, low ATC **for one ad only**; other ads to the same page convert | This ad promises something the page doesn't show (e.g. the ad is about tiffin, the page is about protein) | Point the ad at a matching page/section, or adjust the page hero |
| **Checkout friction** | Good ATC, **low purchase rate** | Drop-off at shipping, payment or COD step | Shipping threshold, COD, payment options, trust badges *(business decision)* |
| **Bad audience** | Good metrics in one age/geo/gender breakdown, poor in others; or everything is poor despite strong creative | Check the breakdowns; compare with the same creative in broad targeting | Broaden, or build a specific concept for the segment that's responding |
| **Weak product-market fit** (for this product, now) | Multiple **distinct concepts** get good hook and CTR, the landing page converts for other products, but this product's ATC and repeat rate stay low | Reviews and feedback mention taste, price or usage issues; low repeat among buyers | This isn't an ad problem. Feed back to product/pricing. Shift budget to products that convert. |

**Key rule:** Don't blame the creative for a funnel problem, and don't blame the funnel for a creative problem. **One ad failing is a creative issue. All ads failing at the same step is a funnel issue.**

---

## 6. Test hygiene

- Change **one class of variable** per test (hook OR length OR CTA), and at most one concept per ad set.
- Keep the landing page, offer and audience **fixed** during a creative test.
- Record the hypothesis *before* launching ("We think the dad-humour hook will beat the ritual hook on hook rate because…").
- Log results even when they fail. Failed tests prevent repeated mistakes.
- Use the naming convention from [Part 8](07-creative-multiplication.md#naming-convention).
- Check comments daily: they're free qualitative research (objections, confusion, praise), and misleading comments may need a reply.

---

## 7. Weekly rhythm

| Day | Activity |
|---|---|
| **Monday** | Review the previous week's tests against baseline. Decide keep / kill / modify / expand / reshoot ([Part 10](09-winner-iteration.md)). Update the learning log. |
| **Tuesday** | Brief the next batch (using the [brief template](10-creative-brief-template.md)). Graduate winners to scaling. |
| **Wednesday–Thursday** | Production: edit variants from existing footage; make statics. |
| **Thursday/Friday** | Launch the new test batch (launching before the weekend gives a full week of data by the next review). |
| **Daily (10 min)** | Check spend pacing, catastrophic underperformers and comments. **No optimisation edits.** |

---

## 8. What to test first (priority order)

1. **Product**: which product acquires customers most efficiently? (It may not be the one you expect.)
2. **Concept/angle**: which tension and argument wins for that product?
3. **Format**: UGC vs static vs carousel for the winning concept.
4. **Hook and first frame**: multiply the winner.
5. **Length**: optimise depth.
6. **CTA and caption**: polish.

---

## 9. The learning log

Keep one row per test in `learnings/test-log.md` (or a shared sheet):

| Field | Example |
|---|---|
| Test ID | T-2026-10-01 |
| Dates | 3 Oct – 10 Oct |
| Product | Breakfast Cookies |
| Concept (Tension / Angle) | T-22 / A-34 Chai Needs a Biscuit |
| Variable tested | Hook category |
| Hypothesis | Humour (dad) hook will beat cultural ritual hook on hook rate |
| Ads | BC_A34_HHU01_DAD_30_RITUAL_v1 vs BC_A34_HCT07_DUNK_30_RITUAL_v1 |
| Spend per ad | — |
| Hook rate / hold / CTR / ATC rate / CPA vs baseline | — |
| Result | Winner / loser / inconclusive |
| **Learning (one sentence)** | "Dad-approval humour beats ritual on attention and matches it on CPA." |
| Next action | Expand: dad-humour hook for Chocolate Cookies |
