# 01 · Scoring Methodology

**Topic:** How the Wellbeing Index (0–100), its five sub-scores, the risk tiers and the Quality ROI are calculated.
**Applies to:** Personal care (soaps, shampoos, oils) and supplements.
**Last reviewed:** 2026-11-14

> This tool informs product choice. It does not give medical advice.

---

## 1. What "wellbeing" means here

A product scores well when it **does its job (efficacy) without side effects**, judged on two things:

- **Body impact:** what the ingredients, additives and contaminants do to the person using it.
- **Environment impact:** packaging and ingredients that persist or pollute, such as microplastics and plastic-related chemicals.

Every score is built only from the label and from the approved sources in `02-approved-sources.md`.

---

## 2. Risk tiers for individual ingredients

Every ingredient of concern gets exactly one tier, and **each tier must name the authority behind it**.

| Tier | Meaning | Typical evidence |
|---|---|---|
| **High** | Banned, restricted or prohibited for this use by a regulator in the market of sale, **or** a known human carcinogen (e.g. IARC Group 1) at a realistic exposure, **or** linked to a Class I recall or active import alert | FDA prohibited-ingredient rule, FDA recall, IARC Group 1, EPA hazard finding |
| **Moderate** | Restricted or banned in at least one major jurisdiction, a possible or probable carcinogen (IARC 2A/2B), a known endocrine-disruption concern, or a recognised skin sensitiser | EU/EFSA restriction, IARC 2A/2B, NIH/NIEHS finding |
| **Low** | Permitted, but with a known irritation, allergy or contamination watch-point | FDA guidance, NIH ODS fact sheet |
| **No authoritative data found** | None of the approved sources covers the ingredient | Write exactly: *"No authoritative data found."* |

Rules:

1. **Use the stricter rating when approved sources disagree**, but report the legal status in the market where the product is sold (see the conflict rule in `02-approved-sources.md`).
2. **IARC classifies hazard, not risk.** When a rating rests only on an IARC class, say so, and note the exposure route (e.g. "rinse-off, low exposure").
3. **Allergens are flagged separately** (see section 7) and are not toxicity ratings.
4. Contaminants (e.g. benzene, 1,4-dioxane, heavy metals) are only scored when a recall, import alert or published test result names **this product or batch**. Otherwise they are listed as a *watch-point* with no deduction.

---

## 3. The five sub-scores

Each sub-score runs from 0 to 100. All of them start at 100 and lose points by deduction. None can go below 0.

### 3.1 Ingredient Safety
Covers actives, base ingredients and named contaminants. **Additives are scored in 3.3, never here.** Each flagged ingredient is deducted in exactly one sub-score.

| Finding | Deduction |
|---|---|
| High-risk ingredient | −30 |
| Moderate-risk ingredient | −12 |
| Low-risk ingredient | −4 |
| No authoritative data found | 0 (listed; lowers confidence) |

**Position multiplier:** ×1.25 if the ingredient is among the **first five** on the list or is a declared **active ingredient** (round to the nearest whole point; e.g. −4 becomes −5, −12 becomes −15).

### 3.2 Processing Level
This is the tool's own rubric. It describes how far the product is from its raw materials and is not a risk rating, so it needs no authority.

| Level | Supplements (adapted from the NOVA classification as described by FAO, 2019) | Personal care | Score |
|---|---|---|---|
| P1 | Minimally processed (e.g. single whole-food powder) | Simple: plain oils, saponified-oil soap, ≤10 ingredients, no ethoxylated ingredients | 100 |
| P2 | Processed culinary ingredients or a simple blend | Plant-derived, non-ethoxylated surfactants, ≤20 ingredients | 75 |
| P3 | Processed: protein isolates or extracts, few additives | Conventional system with ethoxylated surfactants (names containing "-eth", "PEG-") | 50 |
| P4 | Ultra-processed: isolates plus flavours, sweeteners and other cosmetic additives | >25 ingredients, several ethoxylated ingredients plus synthetic polymers | 25 |

### 3.3 Additives
Additives are preservatives, colours, fragrance or flavour, sweeteners, fillers, emulsifiers, thickeners, opacifiers, pH adjusters, hydrotropes and chelators added for function rather than for the product's purpose. Ingredients that serve the product's purpose (surfactants, oils, conditioners, humectants such as glycerin or panthenol, protein sources) are not counted as additives.

| Finding | Deduction |
|---|---|
| Each additive (load) | −3 |
| Plus: High-risk additive | −30 |
| Plus: Moderate-risk additive | −12 |
| Plus: Low-risk additive | −4 |

The position multiplier from 3.1 applies to the **risk** deductions here, not to the −3 load.

### 3.4 Nutrition Balance
Both categories are scored with the same 20% weight. The checks differ because a supplement nourishes the body from inside and a personal-care product nourishes the skin or hair from outside.

#### 3.4a Supplements: dietary nutrition
This is based on one serving, with % Daily Value (%DV) taken from the label.

| Finding | Deduction |
|---|---|
| Added sugars >10% DV | −15 (>20% DV: −30) |
| Sodium >20% DV | −15 |
| Saturated fat >20% DV | −10 |
| Any nutrient above the NIH ODS Tolerable Upper Intake Level at the suggested daily use | −30 |
| Proprietary blend that hides individual amounts | −15 |
| Fibre ≥10% DV | +5 (cap 100) |

#### 3.4b Personal care: skin and hair nourishment
This sub-score asks whether the formula **balances cleansing with nourishment**, or whether it strips and dries the skin or hair. It is the tool's own label-based rubric, like Processing Level, and is not a risk rating. Toxicity is handled in Ingredient Safety, and this sub-score never rates a harm.

**Nourishing ingredients** are plant oils and butters, humectants (glycerin, panthenol, aloe), proteins and amino acids, ceramides, and conditioning agents (silicones, guar hydroxypropyltrimonium chloride, polyquaterniums).

| Finding | Deduction |
|---|---|
| Harsh anionic surfactant (a sulfate or sulfonate, e.g. SLS, SLES, ammonium lauryl sulfate, olefin sulfonate) among the first 3 ingredients | −20 for the first, −10 for each additional one |
| Drying alcohol (alcohol denat., SD alcohol, isopropyl alcohol) among the first 5 ingredients | −15 |
| Nourishing ingredients appear only **after the first preservative**, so likely ≤1% (a "label-dressing" amount) | −10 |
| **No** nourishing ingredient anywhere on the list | −20 |
| Leave-on product (oil, lotion, cream) whose first ingredient is a nourishing oil, butter or humectant | +5 (cap 100) |

If a section of the ingredient list can't be read or isn't published, score from the known part and add the incomplete-list warning (section 4, "Missing data").

### 3.5 Claim Integrity
Every front and back claim is checked against `03-key-terms-registry.md` and the registries in `05-regulatory-registries.md`.

| Status | Meaning | Deduction |
|---|---|---|
| **Verified** | Confirmed in an official registry (e.g. USDA Organic Integrity Database) | 0 |
| **Consistent** | Not registry-checked, but matches the ingredient list and its legal definition | 0 |
| **Unverifiable** | No legal definition, or no certificate or test found in approved sources | −10 |
| **Misleading** | Technically arguable but likely to create a false impression (e.g. "chemical-free") | −25 |
| **False** | Contradicted by the label, ingredients or a registry | −40 |
| **Missing required statement** | A statement the law requires is absent (e.g. the FDA disclaimer on a supplement structure/function claim) | −15 |

---

## 4. Weights and the Wellbeing Index

**Wellbeing Index (WI) = Σ (sub-score × weight)**, rounded to a whole number (halves round up, e.g. 81.5 → 82).

The same weights apply to **both** supplements and personal care, so every product is scored on all five sub-scores.

| Sub-score | Weight (supplements and personal care) |
|---|---|
| Ingredient Safety | 35% |
| Processing Level | 15% |
| Additives | 15% |
| Nutrition Balance | 20% (dietary nutrition §3.4a / skin and hair nourishment §3.4b) |
| Claim Integrity | 15% |
| **Total** | **100%** |

### Hard caps (these override the computed score)

| Condition | WI capped at |
|---|---|
| Active Class I recall covering this product or lot | 20 |
| Recall for an undeclared major allergen covering this product | 20 |
| Contains an ingredient prohibited for this product type in the market of sale | 30 |
| Product or firm on an active FDA import alert (Red List) for a safety reason | 30 |

### Missing data: always rate, always warn

Every product gets a Wellbeing Index, even when data is missing. When data is missing, the score comes with a clear warning.

0. **Check the ingredient pull first.** Before any scoring, run the ingredient pull check in `06-label-reading-guide.md` §6. It confirms the right product, the full list (not just "key ingredients"), and a plausible formula (water and a cleanser in a shampoo, for example). **FAIL** → re-pull from the designated page or ask for a back-label photo. Score with the warning only if neither works.
1. **Never guess.** If part of the label can't be read or isn't published, say so (`[UNREADABLE: …]` / `[NOT AVAILABLE: …]`). Never fill the gap from memory or from a "typical" formula.
2. **Score from what is known.** Apply sections 3.1–3.5 to the ingredients and claims that *are* known:
   - **Ingredient Safety, Additives, Nutrition Balance:** deduct only for known ingredients.
   - **Processing Level:** if the level can't be judged from the known ingredients, use **P3 (50)**, the typical level for shampoos, soaps and protein powders, and note *"default level: formula not known"*.
   - **Nutrition Balance (supplements):** if the nutrition or supplement panel is missing, mark it *Insufficient data* and rescale the other weights to 100%. This is the only case where a sub-score is left out.
3. **Add the incomplete-list warning** to the score wherever it appears (quick answer, score table, verdict):

   > ⚠️ **Full ingredient list not available.** This score is based on <N> known ingredients (<source, e.g. "key ingredients from the brand website">). Ingredients we could not see may raise or lower it.

   Label the WI **Provisional** and show **data coverage**, e.g. *"3 known ingredients (key ingredients only)"* or *"13 of an estimated 18+ ingredients"*.
4. **The warning affects the verdict wording.** If the higher-scoring product has an incomplete list, drop the verdict one level ("Clear winner" → "Leans toward"; "Leans toward" → "Comparable") and add *"pending the full label"*.
5. **Say what would complete the score**, e.g. a photo of the back label.

**Confidence:**
- **High:** full label read, and all ingredients covered by sources.
- **Medium:** 1–3 ingredients with no authoritative data, or a minor unreadable section.
- **Low:** the ingredient pull check failed, the full ingredient list is not available, a sub-score was left out, or more than 3 ingredients are not covered by sources.

---

## 5. Bands

| WI | Band | Plain-language label |
|---|---|---|
| 80–100 | 🟢 Green | Strong choice |
| 60–79 | 🟡 Yellow | Good, with caveats |
| 40–59 | 🟠 Amber | Fair; use with care |
| 0–39 | 🔴 Red | Weak; prefer an alternative |

---

## 6. Quality ROI

> Problem statement: *"Quality ROI = Wellbeing Index / price / qty × 100."*

Read literally (WI ÷ price ÷ qty), a bigger pack would score worse, so the tool uses **WI per unit price**:

```
Price per 100   = Price ÷ (Net quantity in mL or g) × 100
Quality ROI     = WI ÷ Price per 100 × 100
```

- Compare ROI **only between products in the same currency and unit** (mL with mL, g with g).
- Higher ROI means more wellbeing per rupee or dollar.
- ROI is a **tie-breaker and value signal only**. It never overrides a safety cap.
- *Assumption to confirm with the project owner:* "qty" means net quantity in 100 mL or 100 g units.

**Example:** WI 64, ₹390 for 340 mL → price per 100 mL = ₹114.71 → ROI = 64 ÷ 114.71 × 100 = **55.8**.

---

## 7. Efficacy, allergens and care groups (shown, not scored)

- **Fit-for-purpose check:** does the product contain an ingredient recognised by a regulator for the job it is bought for? Example: anti-dandruff actives in the FDA OTC monograph (21 CFR 358.710). If not, the verdict must say so even when the WI is higher.
- **Allergens:** flag the 9 US major food allergens (milk, egg, fish, crustacean shellfish, tree nuts, peanuts, wheat, soy, sesame) and the FSSAI-declared allergens wherever they appear, including in topical products.
- **Care groups:** children, pregnancy and breastfeeding, known allergies. Name a group only when an approved source supports it.

---

## 8. Comparing two products

| WI gap | Verdict wording |
|---|---|
| ≥10 points | "**Clear winner:** Product X" |
| 5–9 points | "**Leans toward** Product X" |
| <5 points | "**Comparable.**" Break the tie by Ingredient Safety, then Claim Integrity, then Quality ROI |

A capped product can never win against an uncapped one.

---

## 9. Worked arithmetic (personal care, illustrative product)

| Sub-score | Score | Weight | Points |
|---|---|---|---|
| Ingredient Safety | 70 | 0.35 | 24.5 |
| Processing Level | 50 | 0.15 | 7.5 |
| Additives | 39 | 0.15 | 5.85 |
| Nutrition Balance (skin and hair nourishment) | 70 | 0.20 | 14.0 |
| Claim Integrity | 80 | 0.15 | 12.0 |
| **WI** | | | **63.85 → 64 (Yellow)** |

Nutrition Balance here: SLES and SLS are both among the first 3 ingredients (−20, −10); the conditioning agents come before the first preservative (no deduction) → 70.

See `08-sample-comparisons.md` for full examples.
