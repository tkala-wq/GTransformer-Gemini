# 07 · Output Template

**Topic:** The fixed format for every product comparison report. Use every section in this order. Do not add or drop sections.
**Last reviewed:** 2026-11-14

**Style rules**
- Plain language a couple can act on **in the store**. Short sentences. No jargon without a one-line explanation.
- **Inform, don't alarm.** Say how big a concern is and how it reaches the body (e.g. "rinse-off, short contact").
- Cite every risk claim as `[Body, document]`. If nothing covers it: *"No authoritative data found."*
- Never guess unreadable text. Show `[UNREADABLE: …]`.
- End with the disclaimer, unchanged.

---

## Template (copy from here)

```markdown
# Product Comparison: <Product A> vs <Product B>

**Date:** YYYY-MM-DD · **Market:** US / India · **Category:** Personal care / Supplement
**Input:** Photos / Web link or barcode / Hybrid · **Confidence:** High / Medium / Low

<!-- Include this warning (one line per affected product) whenever a full ingredient list was not available. Delete it otherwise. -->
> ⚠️ **Full ingredient list not available for <Product>.** This score is based on <N> known ingredients (<source>). Ingredients we could not see may raise or lower it. To complete it: <e.g. a photo of the back label>.

## ⚡ Quick answer
<One or two sentences: which one to pick and the single main reason. Mention any fit-for-purpose caveat. If a product has the warning above, say "pending the full label".>

| | Product A | Product B |
|---|---|---|
| **Wellbeing Index** | NN / 100 (🟢/🟡/🟠/🔴) <⚠️ Provisional: incomplete ingredient list> | NN / 100 (🟢/🟡/🟠/🔴) |
| **Data coverage** | Full list / <N> known ingredients (<source>) | Full list / … |
| **Ingredient pull check** (`06` §6) | ✅ PASS / ⚠️ PARTIAL / ❌ FAIL (checks failed: …) | ✅ / ⚠️ / ❌ |
| **Quality ROI** | NN.N | NN.N |
| **Does the job it's bought for?** | Yes / No / Unclear | Yes / No / Unclear |
| **Biggest concern** | <ingredient or claim> | <ingredient or claim> |

---

## 1. Product snapshot

### Product A: <Brand Name Variant>
- **Net quantity / price:** <qty> · <price, currency> (price per 100 mL or g: <x>)
- **Claims made:** "<claim 1>", "<claim 2>", …
- **Active ingredient(s):** <name, strength> or "None declared"
- **Full ingredient list (label order):** <1. …, 2. …, …> or <known ingredients> + `[NOT AVAILABLE: …]`
- **Panel (supplements):** serving <x>; <key nutrients with %DV>
- **Allergens:** <list or "None of the major allergens found">
- **Identifiers:** <FSSAI / licence / NDC / certifier / lot / expiry>
- **Unreadable parts:** <list or "None">
- **Ingredient pull check:** <PASS / PARTIAL / FAIL> · source <url> · checks failed <list> · next step <re-pull / photo / none>

### Product B: <…>
<same fields>

---

## 2. Ingredient risk check

| Product | Ingredient | Position | Risk tier | Why (plain language) | Authority |
|---|---|---|---|---|---|
| A | <name> | #<n> / active | High / Moderate / Low / No authoritative data found | <one line> | [<Body>, <doc>] |

**Watch-points (not scored):** <contaminant watch-points, e.g. "1,4-dioxane possible with SLES; no product test found">

---

## 3. Claim verification

| Product | Claim | Status | What we found | Source |
|---|---|---|---|---|
| A | "<claim>" | Verified / Consistent / Unverifiable / Misleading / False / Missing required statement | <one line> | [<registry or 03 entry>] |

New label terms found: <term → added to 03-key-terms-registry.md / "none">

---

## 4. Wellbeing Index

| Sub-score | Weight | Product A | Product B |
|---|---|---|---|
| Ingredient Safety | 35% | NN | NN |
| Processing Level | 15% | NN (P_) | NN (P_) |
| Additives | 15% | NN | NN |
| Nutrition Balance (dietary / skin and hair) | 20% | NN | NN |
| Claim Integrity | 15% | NN | NN |
| **Wellbeing Index** | | **NN** | **NN** |
| Caps applied | | <none / reason> | <none / reason> |
| Provisional? | | Yes / No | Yes / No |
| Full ingredient list available? | | Yes / ⚠️ No: <N> known | Yes / ⚠️ No: <N> known |

**Quality ROI** = WI ÷ (price per 100 mL or g) × 100

| | Product A | Product B |
|---|---|---|
| Price per 100 | <x> | <x> |
| Quality ROI | NN.N | NN.N |

<Show the deductions behind each sub-score in one line each, e.g. "A Additives: 11 additives (−33), fragrance (−12), MCI/MI (−12), Blue 1 (−4) = 39".>

---

## 5. Verdict

**Better choice for the household:** <Product> (<Clear winner / Leans toward / Comparable>, gap NN points) <, pending the full label (if the winner's list is incomplete; drop the wording one level per `01` §4)>

**Trade-offs**
- <e.g. "B scores higher but has no anti-dandruff active. If dandruff is the reason for buying, A does that job.">
- <value vs quality>

**Who should be careful**
- 👶 **Children:** <specific note with source, or "No specific concern found in approved sources">
- 🤰 **Pregnancy / breastfeeding:** <…>
- 🤧 **Allergies:** <…>

**In-store tip:** <one practical action, e.g. "Look for 'fragrance-free' if anyone in the family has sensitive skin.">

---

## 6. Sources and registry checks

| # | Registry | Query | Date | Result | Effect |
|---|---|---|---|---|---|
| 0 | Ingredient pull check (`06` §6) | <source URL> | … | PASS / PARTIAL / FAIL | Warning / confidence |
| 1 | FDA Recalls | … | … | … | … |

**References**
1. <Body> — <document> — <URL>

---

> *This comparison is for general information to help you choose between products. It is not medical advice. If you have a health condition, are pregnant, or are buying for a young child, check with a doctor or pharmacist. Ratings are based on the product label and the public sources listed above as of the date shown.*
```

---

## Quality checklist before sending

- [ ] Every ingredient of concern has a tier **and** a named authority
- [ ] Every claim has a status
- [ ] **Ingredient pull check run for each product**, with the result shown; a FAIL was re-pulled or a photo requested
- [ ] Unreadable text is marked, not guessed
- [ ] Every product is scored; any product without a full ingredient list carries the ⚠️ warning, a data-coverage note, and "pending the full label" in the verdict
- [ ] Sub-score arithmetic adds up; caps checked
- [ ] Quality ROI uses the same currency and unit for both products
- [ ] The fit-for-purpose check is stated
- [ ] No Tier 3 (news) source is used as the basis of a rating
- [ ] Tone is calm and practical; the disclaimer is present
