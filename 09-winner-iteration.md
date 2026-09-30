# Part 10 — Winner Iteration System

Once a test has enough data ([Part 9, section 3](08-creative-testing.md#3-how-much-to-launch-and-how-long-to-wait)), every ad gets **one of five decisions**:

| Decision | Meaning |
|---|---|
| 🟢 **KEEP** | Working. Leave it alone, and graduate it to scaling if it's beating the control. |
| 🔴 **KILL** | Not working and not fixable cheaply. Pause it and log the learning. |
| 🟡 **MODIFY** | One part of the chain is broken. Fix that part using existing footage. |
| 🔵 **EXPAND** | The message is proven. Take it to new hooks, formats, products or audiences. |
| 🟣 **RESHOOT** | The message is proven, but the footage limits it (quality, creator, missing shots). |

---

## The decision tree

Start at the top. Compare each metric with **this ad's siblings, the account baseline and the control** (never an absolute benchmark).

```
                        ┌─────────────────────────────┐
                        │ Enough data? (spend ≥ 2–3×  │
                        │ target CPA, ≥ 5–7 days)     │
                        └──────────────┬──────────────┘
                              no ──────┴────── yes
                               │                │
                        WAIT (don't touch)      ▼
                                   ┌──────────────────────────┐
                                   │ CPA at or better than    │
                                   │ target?                  │
                                   └────────────┬─────────────┘
                                 yes ───────────┴─────────── no
                                  │                          │
                                  ▼                          ▼
                    ┌─────────────────────────┐   ┌──────────────────────────┐
                    │ Is hook rate / CTR also │   │ Where does the chain     │
                    │ strong?                 │   │ break first?             │
                    └───────────┬─────────────┘   └────────────┬─────────────┘
                  yes ──────────┴────── no                     │
                   │                    │                      ▼
                   ▼                    ▼            (see Scenarios 1–6 below)
           KEEP + EXPAND        KEEP + MODIFY hook
                                (Scenario 3)
```

---

## Scenarios

### Scenario 1: Strong hook, weak purchases
**Pattern:** Hook rate above baseline, CTR at or above baseline, purchases/CPA poor.

**What it means:** The ad earns attention and clicks, but the promise doesn't convert. Either the hook attracts the wrong people, or the page/offer lets them down.

**Investigate in this order:**
1. **Message–page match.** Does the landing page continue the ad's story? (A tiffin hook landing on a generic product page loses people.)
2. **Hook–product match.** Is the hook broad curiosity (a meme, "why is there an accent on the R") that draws non-buyers? Check the age/gender/geo breakdowns.
3. **ATC rate vs other ads to the same page.** If other ads convert on the same page, the problem is this ad's *audience quality*, not the page.

**Change:**
- If the hook is too broad: **MODIFY** by keeping the hook's energy but adding a qualifier ("Parents: …", "If you drink chai…").
- If it's a page mismatch: **MODIFY** the destination (a relevant page or section).
- If both look fine: **KILL** and log it as "attention without intent".

### Scenario 2: Strong CTR, weak add-to-cart
**Pattern:** CTR at or above baseline, LPV rate fine, ATC rate poor.

**What to investigate:**
- **Is it just this ad, or all ads for this product?**
  - *Just this ad:* message mismatch, or the ad over-promised (e.g. implied a price, offer or format that isn't there). **MODIFY** the ad.
  - *All ads for this product:* a **landing page, price or offer** issue. Not a creative problem. Escalate: page above-the-fold, price clarity (per pack, per cookie, per serving), pack size, delivery cost, reviews, and the back of the pack visible on the page.
- **Is the LPV rate low too?** Then it's page speed or accidental clicks. Fix the page first.

### Scenario 3: Good purchases, low thumb-stop
**Pattern:** CPA good, but hook rate below baseline, so the ad reaches few people and will be hard to scale.

**What it means:** The body and message convert well. The entry point is the bottleneck, and the few who get past it are high-intent.

**Change:** **KEEP** the original running, and **MODIFY** by producing 3–5 new hook/first-frame variants on the **same body** (Part 8, stage 1). Prioritise:
- an appetite close-up first frame
- a face-plus-strong-statement first frame
- on-screen text readable in under 1 second

Don't change the body. It's the valuable part.

### Scenario 4: Good hook, low hold rate
**Pattern:** Hook rate strong, hold rate weak, CTR weak.

**What it means:** The body doesn't pay off the hook, or it's too slow.

**Change:** **MODIFY** the edit:
- Check the retention curve for the drop point.
- Move taste proof or the product reveal earlier.
- Cut the tension/old-solution blocks down.
- Make sure the second 3–6 continues the hook's promise directly.
- Try the shorter length.

### Scenario 5: Everything average, nothing broken
**Pattern:** All metrics near median, and CPA slightly above target.

**What it means:** A competent ad with no edge. The concept may be too familiar.

**Change:** Don't spend time polishing. **KILL** it, or try a single **bold** hook variant (contrarian or humour) as a last shot. Average concepts rarely become winners through tweaks.

### Scenario 6: Poor on every metric
**Pattern:** Hook rate, CTR and conversion all below baseline.

**Change:** **KILL.** Log what the concept was and one hypothesis for why it failed (wrong tension? wrong audience? wrong product?). Don't reshoot a concept that failed at the hook *and* the conversion.

### Scenario 7: One message keeps winning
**Pattern:** The same angle (e.g. "read the back", "dad approval", "keep the chai") wins across multiple executions.

**What it means:** You've found a **campaign territory**, not just an ad. This is the most valuable outcome of testing.

**Expand it systematically:**

| Expansion axis | Example (winning message: "Dad-approved label") |
|---|---|
| **New hooks** in the same territory | "My dad read the whole back of this pack" → "My dad has one question for every snack" → "Things my dad says reading labels" |
| **New products** | Breakfast Cookies → Ragi & Cocoa Spread → PB |
| **New formats** | UGC → meme static → carousel → founder reaction video |
| **New characters** | Dad → Nani → a gym-bro friend → a colleague |
| **New audiences/languages** | Hindi, Tamil and Kannada versions; regional tests |
| **New funnel stages** | Prospecting → retargeting ("Dad's still approving") → post-purchase email and social |
| **Off-Meta** | Pack messaging, website hero, marketplace A+ content, organic series |

**Rule:** Expand one axis at a time so you know what caused any change.

### Scenario 8: A winner starts declining
See [creative fatigue](08-creative-testing.md#creative-fatigue). Refresh the entry point first, then the execution, then retire it.

---

## Decision rules summary

### 🟢 KEEP when
- CPA ≤ target with enough data, **and**
- performance is stable or improving over the last 3–5 days, **and**
- no compliance issue has been raised (comments, platform, legal).

### 🔴 KILL when
- It has had enough spend (≥ 2–3× target CPA) with CPA clearly above target **and** no single metric suggests a cheap fix, **or**
- the hook rate is far below siblings after meaningful impressions (an early kill is fine for hooks), **or**
- a compliance issue arises (a claim problem, misleading comments you can't correct), which means pause immediately, whatever the performance.

### 🟡 MODIFY when
- **one** link in the metric chain is clearly weak and the rest are healthy (Scenarios 1, 3, 4), **and**
- the fix can be made from existing footage (a new hook, trim, CTA or caption).

### 🔵 EXPAND when
- the ad has beaten the control, **or**
- the same message has won in 2+ executions (Scenario 7).

### 🟣 RESHOOT when
- the message is proven, **but** the footage is limiting it: poor lighting on the food, a creator mismatch with the audience, missing shots (no back-of-pack, no taste shot), an outdated pack, low production quality in a format that needs polish, **or**
- the proven concept needs a new creator or setting to reach a new segment (e.g. a regional language, a gym setting), **or**
- AI UGC proved the concept and it's time to reshoot with real creators.

---

## Iteration cadence
- **Weekly:** decisions on every ad in testing (Monday review).
- **Bi-weekly:** refresh entry points for scaling winners before fatigue.
- **Monthly:** review territories. Which messages are winning across products? Update [the top territories](final-output/03-campaign-territories.md) and the [top hooks](final-output/04-top-50-hooks.md).
- **Quarterly:** strategic review. Is the product mix right? Which tensions haven't been tested yet?
