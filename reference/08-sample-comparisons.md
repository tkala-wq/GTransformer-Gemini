# 08 · Sample Comparisons

**Topic:** Worked examples that set the standard for finished reports.
**Last reviewed:** 2026-11-14

> **Sample 1 uses real products** (the problem statement's use case), built from **public web labels only** (Scenario B in `06`). It shows how the tool handles a label that isn't fully published: it **never guesses** the missing ingredients, **still scores** the product from what is known, and shows the ⚠️ incomplete-list warning.
> **Samples 2 and 3 use made-up products** (Brands C–F) to show the full method; their registry results are illustrative.
> Ratings marked † assume the proposed EU source in `02` §5 is approved.

| # | Products | Market | Shows |
|---|---|---|---|
| 1 | **Head & Shoulders Classic Clean vs Sri Sri Tattva Protein Shampoo** (real) | US | A real web-label evaluation; a **failed ingredient pull check** (key ingredients only); scoring with an **incomplete ingredient list** (⚠️ warning, softened verdict); a fit-for-purpose check |
| 2 | Protein powder: whey vs plant (fictional) | US ($) | A false claim, a missing DSHEA disclaimer, an organic seal verified in the OID |
| 3 | Hair oil: Ayurvedic blend vs pure coconut (fictional) | US ($) | A partly unreadable label → ⚠️ Provisional score; a "chemical-free" claim |

---

# Sample 1: Head & Shoulders Classic Clean vs Sri Sri Tattva Protein Shampoo

**Date:** 2026-11-14 · **Market:** US · **Category:** Personal care · **Input:** Web label from US sale websites (no photos) · **Confidence:** Low
**Status:** Both products scored; both scores are **Provisional**.

> ⚠️ **Full ingredient list not available for Sri Sri Tattva Protein Shampoo.** This score is based on **3 known ingredients** (the "key ingredients" on the brand's US store and Amazon.com). Ingredients we could not see may raise or lower it. To complete it: a photo of the back label.
>
> ⚠️ **Full ingredient list not confirmed for Head & Shoulders Classic Clean.** This score is based on the **active ingredient plus 18 known inactive ingredients** (brand page and DailyMed). The official list could not be opened in full, so a few items, such as preservatives, may be missing.

> **Read this first**
> - 🇺🇸 **US sale websites only** (Problem Statement guardrail). Product facts come only from websites that sell these products in the US: the brands' US sites, Amazon.com and H-E-B, plus DailyMed (the official US register of OTC drug labels, run by NIH). Non-US sites, such as Indian retailers, were not used.
> - The pages could not be opened directly from this session, so the facts below come from search results that quote these pages. Every fact is cited.
> - **Head & Shoulders formulas differ by variant.** The label used here is the **US "Classic Clean" shampoo** (DailyMed set ID `f28a55cf-eb42-4a0d-a4a3-2bae72b58ac8`).
> - This is not a judgement of either brand's safety. It is not medical advice.

## ⚡ Quick answer
- **For dandruff:** choose **Head & Shoulders**. It is the only one with an FDA-recognised anti-dandruff active (pyrithione zinc 1%).
- **For dry hair without dandruff:** the evidence **leans toward Sri Sri Tattva** (80 vs 68), *pending the full label*. Its score rests on only 3 known ingredients, so it could drop once the full list is seen.

| | Head & Shoulders Classic Clean | Sri Sri Tattva Protein Shampoo |
|---|---|---|
| **Wellbeing Index** | 68 / 100 🟡 ⚠️ **Provisional**: list not fully confirmed | 80 / 100 🟢 ⚠️ **Provisional**: incomplete ingredient list |
| **Data coverage** | Active + 18 known inactive ingredients (brand page, DailyMed) | 3 known ingredients (key ingredients only: srisritattvausa.com, Amazon.com) |
| **Ingredient pull check** (`06` §6) | ⚠️ PARTIAL (check 6 flagged) | ❌ **FAIL** (checks 3, 4, 5, 7) |
| **Quality ROI** | Needs price | Needs price |
| **Does the job it's bought for?** | Dandruff: **Yes** (pyrithione zinc 1%) | Dandruff: No active declared · Dry hair: unclear |
| **Biggest concern** | Zinc pyrithione (banned in EU cosmetics†), fragrance, two harsh surfactants first on the list | A hair-loss claim (drug-like for a US cosmetic); most of the formula is unknown |

## 0. Ingredient pull check

> ❌ **The Sri Sri Tattva ingredient pull failed.** What was pulled is the brand's **"key ingredients"** marketing list, not the label's ingredient list. A real shampoo must contain water and at least one cleansing agent, and none appear. The score below is therefore based on incomplete data.

| # | Check | Head & Shoulders Classic Clean | Sri Sri Tattva Protein Shampoo |
|---|---|---|---|
| 1 | Right source | ✅ Brand US page + DailyMed | ✅ Designated page (https://srisritattvausa.com/products/protein-shampoo?_pos=1&_psq=protein+sham&_psid=ff0d59a8f&_ss=e) + Amazon.com |
| 2 | Right product (variant, size) | ✅ Classic Clean shampoo (not 2-in-1) | ✅ Protein Shampoo, 200 mL |
| 3 | Full list, not "key ingredients" | ✅ Ingredient list (some items unconfirmed) | ❌ Only "key ingredients": Green gram, Fenugreek, Chickpea extract |
| 4 | Has a base (water) | ✅ Water #1 | ❌ No water |
| 5 | Has a cleansing agent | ✅ SLS, SLES, cocamidopropyl betaine | ❌ No cleanser |
| 6 | Has a preservative | ⚠️ Not confirmed (piroctone olamine is an antifungal) | ❌ None listed |
| 7 | Plausible length | ✅ 19 items | ❌ 3 items |
| 8 | Consistent with claims | ✅ "Paraben free" can be checked | ❌ "Sulfate-free", "paraben-free" and "vegan" can't be checked |
| | **Result** | ⚠️ **PARTIAL** | ❌ **FAIL** |
| | **Next step** | Confirm the full DailyMed list | **Re-pull the ingredient list from the designated page**, or a photo of the US pack's back label |

Because the re-pull wasn't possible in this session, both products are scored from what is known (`01` §4), and Sri Sri Tattva's confidence is **Low**.

## 1. Product snapshot

### Head & Shoulders Classic Clean Anti-Dandruff Shampoo (US label)
- **Maker:** Procter & Gamble · **Type:** OTC drug (US) · NDC prefix 37000-071 [DailyMed]
- **Net quantity / price:** sold in sizes including 13.5 fl oz and 28.2 fl oz [US retailer listings]. **Price (USD): not supplied.**
- **Claims on the brand page:** "Paraben Free", "24/7 Dandruff Protection", "for daily use" [headandshoulders.com]
- **Active ingredient:** **Pyrithione zinc 1%** (anti-dandruff) [DailyMed; H-E-B listing]
- **Inactive ingredients, in the order on the brand page:** 1. Water, 2. Sodium Lauryl Sulfate, 3. Sodium Laureth Sulfate, 4. Cocamidopropyl Betaine, 5. Sodium Xylenesulfonate, 6. Zinc Carbonate, 7. Fragrance, 8. Sodium Chloride, 9. Dimethicone, 10. Guar Hydroxypropyltrimonium Chloride, 11. Piroctone Olamine, 12. Glycerin, 13. Trihydroxystearin [headandshoulders.com, quoted in search results]
- **Also on the DailyMed label (position not confirmed):** Niacinamide, Polyquaternium-76, Neosetophoma Cerealis Extract, Blue 1, Red 33 [DailyMed]
- **Unreadable / unconfirmed:** `[NOT CONFIRMED: the full DailyMed inactive list could not be opened; the published list may contain further items such as preservatives]`
- **Allergens:** none of the major allergens in the confirmed list

### Sri Sri Tattva Protein Shampoo, for normal to dry hair (200 mL)
- **Sold in the US by:** Sri Sri Tattva USA and Amazon.com
- **Designated product page (provided by the project owner):** [Sri Sri Tattva USA: Protein Shampoo](https://srisritattvausa.com/products/protein-shampoo?_pos=1&_psq=protein+sham&_psid=ff0d59a8f&_ss=e)
- **Net quantity / price:** 200 mL. **Price (USD): not supplied.**
- **Claims:**
  - "Plant-based proteins and minerals from chickpeas, green gram, and fenugreek"; "Paraben-free"; "Vegan" [srisritattvausa.com]
  - Fenugreek "helps reduce premature graying and hair loss" [srisritattvausa.com, ingredient description]
  - "Natural Ayurvedic Haircare for Normal to Dry, Damaged Hair"; "Sulfate-Free Formula"; "for Healthy, Shiny and Strong Locks" [Amazon.com listing title]
- **Key ingredients (as published):** Green gram, Fenugreek, Chickpea extract [srisritattvausa.com; Amazon.com]
- **Full ingredient list:** `[NOT AVAILABLE: no US sale website returned the complete INCI list]`
- **Ingredient pull check:** ❌ FAIL (checks 3, 4, 5, 7). Only the key ingredients were returned. Next step: re-pull from the designated page or photograph the back label
- **Allergens:** none of the US major allergens among the known ingredients (chickpea and green gram are legumes)

## 2. Ingredient risk check

| Product | Ingredient | Position | Tier | Why (plain language) | Authority |
|---|---|---|---|---|---|
| H&S | **Pyrithione zinc** | **active** | Moderate† | Approved by the FDA for dandruff at 1–2% in rinse-off shampoos. Banned in EU cosmetics since 2022 as a reproductive-toxicity hazard. In a shampoo it's rinsed off, so contact is short | [FDA, 21 CFR 358.710]; [EU Reg. 2021/1902]† |
| H&S | Sodium lauryl sulfate | #2 | Low | Can irritate skin and eyes with long contact | [PubChem] |
| H&S | Sodium laureth sulfate | #3 | Low | Mild irritant; possible 1,4-dioxane traces (no product test found → watch-point only) | [PubChem]; [EPA] |
| H&S | Cocamidopropyl betaine | #4 | Low | Occasional contact allergy | [FDA, allergens in cosmetics] |
| H&S | Fragrance | #7 (additive) | Moderate | Undisclosed mixture; a common cause of cosmetic allergy | [FDA, MoCRA / allergens in cosmetics] |
| H&S | Blue 1, Red 33 | end (additive) | Low | FDA-listed colour additives; rare allergy | [FDA, 21 CFR 74] |
| H&S | Piroctone olamine | #11 | No authoritative data found | Antifungal; no rating from a core approved source (EU limits it in cosmetics†) | — |
| H&S | Neosetophoma cerealis extract | unconfirmed | No authoritative data found | — | — |
| H&S | Zinc carbonate, niacinamide, glycerin, dimethicone, guar HPTC, polyquaternium-76 | — | Not flagged | — | — |
| SST | Green gram, fenugreek, chickpea extract | unknown | Not flagged | Plant extracts; no concern found. Chickpea is a legume, so people with legume allergies may want to check | — |
| SST | **Everything else** | — | Not seen ⚠️ | The full list isn't published, so cleansers, preservatives and fragrance (if any) could not be rated | — |

**Watch-points (not scored):** 1,4-dioxane (H&S, from SLES): no product test or recall found.

## 3. Claim verification

| Product | Claim | Status | What we found |
|---|---|---|---|
| H&S | Anti-dandruff (Drug Facts use) | Consistent | Pyrithione zinc 1% is within the FDA monograph range for rinse-off products (21 CFR 358.710) |
| H&S | "Paraben Free" | Consistent* | No parabens in the confirmed list (*the list may be incomplete) |
| H&S | "24/7 Dandruff Protection" | Unverifiable (−10) | No legal definition; no study cited |
| SST | "Plant-based proteins … chickpeas, green gram, fenugreek" | Consistent | Matches the published key ingredients; amounts unknown |
| SST | "Natural" | Unverifiable (−10) | "Natural" has no legal definition for cosmetics |
| SST | "Ayurvedic" | Unverifiable (−10) | No US legal definition (see `03`) |
| SST | "Sulfate-Free Formula" | Unverifiable (−10) | The full list isn't published, so this can't be checked. It becomes Consistent if the label shows no sulfates |
| SST | "Paraben-free" | Unverifiable (−10) | Same reason |
| SST | "Vegan" | Unverifiable (−10) | Same reason |
| SST | "Healthy, Shiny and Strong Locks" | Unverifiable (−10) | No evidence cited |
| SST | Fenugreek "helps reduce … hair loss" | **Misleading** (−25) | A hair-loss claim implies a drug effect, which a US cosmetic can't claim (FDA, cosmetic vs drug), and no evidence is cited |

## 4. Wellbeing Index

| Sub-score | Weight | Head & Shoulders | Sri Sri Tattva |
|---|---|---|---|
| Ingredient Safety | 35% | 70 | 100 ⚠️ |
| Processing Level | 15% | 50 (P3: ethoxylated SLES) | 50 (P3 default: formula not known) |
| Additives | 15% | 59 ⚠️ | 100 ⚠️ |
| Nutrition Balance (skin and hair) | 20% | 70 | 100 ⚠️ |
| Claim Integrity | 15% | 90 | 15 |
| **Wellbeing Index** | | **68** (68.35) ⚠️ Provisional | **80** (79.75) ⚠️ Provisional |
| Full ingredient list available? | | ⚠️ Not fully confirmed: active + 18 known | ⚠️ No: 3 known |
| Caps | | None found | None found |

- **H&S Ingredient Safety:** SLS −5, SLES −5, CAPB −5 (Low ×1.25, top five), pyrithione zinc −15 (Moderate ×1.25, active) = **70**
- **H&S Additives:** 7 confirmed additives (sodium xylenesulfonate, zinc carbonate, fragrance, sodium chloride, trihydroxystearin, Blue 1, Red 33) −21; fragrance −12; Blue 1 −4; Red 33 −4 = **59**. Provisional, because unconfirmed items could lower it
- **H&S Nutrition Balance:** SLS (#2) −20, SLES (#3) −10; conditioning agents (dimethicone, guar) come before the first preservative-type ingredient (piroctone olamine) = **70**
- **H&S Claim Integrity:** "24/7" −10 = **90**
- **SST Ingredient Safety:** green gram, fenugreek and chickpea extract are not flagged = **100** ⚠️ (only 3 ingredients known)
- **SST Processing Level:** can't be judged from 3 plant extracts, so the P3 default applies = **50**
- **SST Additives:** no additives among the known ingredients = **100** ⚠️. Any preservative, fragrance or thickener on the real label would lower this
- **SST Nutrition Balance:** no harsh cleanser among the known ingredients; nourishing protein sources present = **100** ⚠️. The real cleanser is unknown, and a sulfate there would cost −20
- **SST Claim Integrity:** 6 Unverifiable claims (−60) and 1 Misleading hair-loss claim (−25) = **15**. Three of these ("sulfate-free", "paraben-free", "vegan") are Unverifiable only because the full list is missing
- **Why the warning matters:** Sri Sri Tattva's 100s reflect *missing information*, not proven cleanliness. Every shampoo needs a cleansing agent and usually a preservative, and neither is shown. If its cleanser were a sulfate and it contained fragrance, the "sulfate-free" claim would become False and its score would drop to about 69, level with Head & Shoulders. If the full label confirms it is sulfate- and paraben-free, its score would rise

**Quality ROI:** not calculated. Prices weren't supplied, and the two products would need the same currency.

## 5. Verdict

**Better choice for the household:** **Leans toward Sri Sri Tattva Protein Shampoo** (gap 12 points), *pending the full label*.
The gap would normally make it a "Clear winner", but the higher-scoring product has an incomplete ingredient list, so the wording drops one level (`01` §4, Missing data).

**Trade-offs**
- **If someone has dandruff:** choose **Head & Shoulders**. It contains an FDA-recognised anti-dandruff active (pyrithione zinc 1%); Sri Sri Tattva declares none.
- **Head & Shoulders:** it starts with two strong cleansers (SLS, SLES), and it contains fragrance and an active that the EU no longer allows in cosmetics†. Rinse it off well.
- **Sri Sri Tattva:** its herbal "protein" ingredients raise no concern, but its US listing makes a hair-loss claim it can't support as a cosmetic, and most of its formula is unseen. ⚠️ Its score may fall once the full label is checked.

**Who should be careful**
- 🤧 **Allergies / sensitive skin:** Head & Shoulders has fragrance and cocamidopropyl betaine. Sri Sri Tattva's full formula is unknown; chickpea and green gram are legumes.
- 👶 **Children:** keep both out of the eyes. No child-specific concern found in approved sources.
- 🤰 **Pregnancy:** No authoritative data found from US regulators on rinse-off pyrithione zinc in pregnancy. The EU classification is a hazard classification†.

### What would complete these scores
1. The **full ingredient list** for Sri Sri Tattva Protein Shampoo, from the [designated product page](https://srisritattvausa.com/products/protein-shampoo?_pos=1&_psq=protein+sham&_psid=ff0d59a8f&_ss=e) (if it lists one) or a **photo of the US pack's back label**.
2. The **Head & Shoulders variant you would actually buy**: a front and back photo.
3. **US prices (USD) and pack sizes** for both, from a US sale website or the shelf, to work out Quality ROI.

**In-store tip:** In the US, a shampoo that promises to "reduce hair loss" is making a drug claim. Look for a "Drug Facts" box; if there isn't one, treat the claim as marketing.

### Sources and checks

| # | Source | What it gave | Date |
|---|---|---|---|
| 1 | DailyMed (NLM/NIH): *Head and Shoulders Classic Clean, pyrithione zinc shampoo*, set ID f28a55cf-eb42-4a0d-a4a3-2bae72b58ac8. https://dailymed.nlm.nih.gov/dailymed/drugInfo.cfm?setid=f28a55cf-eb42-4a0d-a4a3-2bae72b58ac8 | Active ingredient, NDC, partial inactive list | 2026-11-14 (via search) |
| 2 | Head & Shoulders US product page: https://www.headandshoulders.com/en-us/products/classic-clean-shampoo | Inactive list order, "Paraben Free", "24/7" claims | 2026-11-14 (via search) |
| 3 | H-E-B listing: https://www.heb.com/product-detail/head-shoulders-classic-clean-dandruff-shampoo/10662535 | "Pyrithione Zinc (1 %)" | 2026-11-14 (via search) |
| 0 | Ingredient pull check (`06` §6) | H&S: ⚠️ PARTIAL · SST: ❌ FAIL (key ingredients only) | 2026-11-14 |
| 4 | Sri Sri Tattva USA, **designated product page** (provided by the project owner): https://srisritattvausa.com/products/protein-shampoo?_pos=1&_psq=protein+sham&_psid=ff0d59a8f&_ss=e | Key ingredients, "paraben-free", "vegan", fenugreek hair-loss claim | 2026-11-14 (via search) |
| 5 | Amazon.com: https://www.amazon.com/dp/B07GJZQ4HC | "Natural Ayurvedic", "Sulfate-Free Formula", "Healthy, Shiny and Strong Locks" | 2026-11-14 (via search) |
| 6 | FDA: *Is it a cosmetic, a drug, or both?* https://www.fda.gov/cosmetics/cosmetics-laws-regulations/it-cosmetic-drug-or-both-or-it-soap | Hair-loss claims are drug claims | — |
| 7 | FDA, 21 CFR 358.710 (anti-dandruff actives): https://www.ecfr.gov/current/title-21/section-358.710 | Pyrithione zinc 1–2% rinse-off | — |
| 8 | FDA recalls / openFDA drug enforcement | Not yet searched for this product | To do |

Retailer pages (3, 5) are used **only to identify the product and its label text**. They are never the basis of a risk rating.

---

# Sample 2: Brand C Whey Protein (Chocolate) vs Brand D Organic Plant Protein

**Date:** 2026-11-14 · **Market:** US (Whole Foods) · **Category:** Supplement · **Input:** Hybrid · **Confidence:** High

> **Ingredient pull check (`06` §6):** Brand C ✅ PASS · Brand D ✅ PASS. Full labels with Supplement Facts panels.

## ⚡ Quick answer
**Brand D** is the clear winner (87 vs 75): no additives, and its organic seal checks out. Brand C is better value per dollar, but one of its claims is false.

| | Brand C Whey | Brand D Plant |
|---|---|---|
| **Wellbeing Index** | 75 / 100 🟡 | 87 / 100 🟢 |
| **Quality ROI** | 1237.0 | 1109.5 |
| **Does the job?** | Yes (24 g protein) | Yes (21 g protein) |
| **Biggest concern** | "Natural flavor" claim is false; 3 sweeteners/flavours | Sodium 21% DV per scoop |

## 1. Product snapshot

### Brand C Whey Protein, Chocolate
- **Net quantity / price:** 2 lb (907 g) · $54.99 ($6.06 per 100 g)
- **Claims:** "24 g protein per serving", "Builds lean muscle", "Natural chocolate flavor", "Gluten-free"
- **Ingredients:** 1. Whey Protein Concentrate (Milk), 2. Whey Protein Isolate (Milk), 3. Cocoa Powder (processed with alkali), 4. Maltodextrin, 5. Natural and Artificial Flavors, 6. Xanthan Gum, 7. Soy Lecithin, 8. Sucralose, 9. Acesulfame Potassium
- **Supplement Facts (1 scoop, 33 g):** 130 kcal · protein 24 g · added sugars 1 g (2% DV) · sodium 130 mg (6% DV) · saturated fat 1 g (5% DV)
- **Allergens:** **Milk, soy**
- **DSHEA disclaimer:** ❌ not on the label

### Brand D Organic Plant Protein, Unflavored
- **Net quantity / price:** 18 oz (510 g) · $39.99 ($7.84 per 100 g)
- **Claims:** "USDA Organic", "Non-GMO Project Verified", "Vegan", "Heavy-metal tested"
- **Ingredients:** 1. Organic Pea Protein, 2. Organic Brown Rice Protein, 3. Organic Pumpkin Seed Protein
- **Supplement Facts (1 scoop, 30 g):** 120 kcal · protein 21 g · added sugars 0 g · sodium 480 mg (21% DV) · saturated fat 0.5 g (3% DV)
- **Allergens:** None of the major allergens
- **Certifier:** "Certified organic by [Certifier X]"

## 2. Ingredient risk check

| Product | Ingredient | Position | Tier | Why | Authority |
|---|---|---|---|---|---|
| C | Maltodextrin | #4 (additive) | Low | High-glycaemic filler | [FDA, GRAS] |
| C | Natural and artificial flavors | #5 (additive) | Low | Composition not disclosed | [FDA, 21 CFR 101.22] |
| C | Sucralose | #8 (additive) | Low | WHO advises against non-sugar sweeteners for weight control | [WHO 2023]; [FDA] |
| C | Acesulfame potassium | #9 (additive) | Low | As above | [WHO 2023]; [FDA] |
| D | Brown rice protein | #2 | Watch-point | Rice can carry inorganic arsenic; no product test result published | [FDA, arsenic in rice] |

## 3. Claim verification

| Product | Claim | Status | What we found |
|---|---|---|---|
| C | "24 g protein" | Consistent | Matches the panel |
| C | "Builds lean muscle" | **Missing required statement** (−15) | Structure/function claim without the FDA disclaimer (21 CFR 101.93) |
| C | "Natural chocolate flavor" | **False** (−40) | The ingredient list says "Natural **and Artificial** Flavors" |
| C | "Gluten-free" | Consistent | No gluten grains listed; no test certificate |
| D | "USDA Organic" | **Verified** | *Illustrative:* operation found in the USDA OID, status Certified, Handling scope, certifier matches the label |
| D | "Non-GMO Project Verified" | Unverifiable (−10) | Private certifier, not an approved source. Organic certification already excludes GMOs |
| D | "Vegan" | Consistent | All ingredients are plant-derived |
| D | "Heavy-metal tested" | Unverifiable (−10) | No results, lab or limits published |

## 4. Wellbeing Index

| Sub-score | Weight | Brand C | Brand D |
|---|---|---|---|
| Ingredient Safety | 35% | 100 | 100 |
| Processing Level | 15% | 25 (P4) | 50 (P3) |
| Additives | 15% | 65 | 100 |
| Nutrition Balance | 20% | 100 | 85 |
| Claim Integrity | 15% | 45 | 80 |
| **Wellbeing Index** | | **75** (75.25) | **87** (86.5) |

- **C Additives:** 6 additives −18; maltodextrin −5 (Low ×1.25, top five); flavours −4; sucralose −4; ace-K −4 = **65**
- **D Nutrition Balance:** sodium 21% DV −15 = **85**

| | Brand C | Brand D |
|---|---|---|
| Price per 100 g | $6.06 | $7.84 |
| **Quality ROI** | **1237.0** | **1109.5** |

## 5. Verdict
**Better choice:** Brand D (**clear winner**, a 12-point gap).
**Trade-offs**
- Brand C costs less per gram and has a bit more protein per scoop, but uses sweeteners and flavours and makes a false "natural flavor" claim.
- Brand D has more sodium. Two scoops a day gives about 42% of the daily sodium value.

**Who should be careful**
- 🤧 **Allergies:** Brand C contains **milk and soy**.
- 👶 **Children:** protein powders are made for adults; follow the label. No child-specific data in approved sources.
- 🤰 **Pregnancy:** No authoritative data found for these products. Ask a doctor before starting supplements.
- 🧂 **Watching salt:** Brand D, 480 mg sodium per scoop.

**In-store tip:** Read the flavour line on the back, not the front. "Natural and artificial flavors" means the front claim isn't the whole story.

---

# Sample 3: Brand E Herbal Hair Oil vs Brand F Pure Coconut Oil

**Date:** 2026-11-14 · **Market:** US · **Category:** Personal care · **Input:** Photos · **Confidence:** Low (part of Brand E's label is unreadable)

> **Ingredient pull check (`06` §6):** Brand E ⚠️ PARTIAL (a real label list from the photo, but the last ~2 lines are unreadable) · Brand F ✅ PASS (oils are anhydrous, so checks 4–6 don't apply).
>
> ⚠️ **Full ingredient list not available for Brand E Herbal Hair Oil.** This score is based on **6 known ingredients** (read from the photo). About 2 lines after "Parfum" are hidden by glare. Ingredients we could not see may raise or lower the score. To complete it: a clearer photo of the back label.

## ⚡ Quick answer
**Brand F** is the clear winner (99 vs 82, provisional): one ingredient and no misleading claims. Brand E's "reduces hair fall" is a drug claim that a US cosmetic can't make.

| | Brand E Herbal | Brand F Coconut |
|---|---|---|
| **Wellbeing Index** | 82 / 100 🟢 ⚠️ **Provisional**: incomplete ingredient list | 99 / 100 🟢 |
| **Data coverage** | 6 known ingredients (about 2 lines unreadable) | Full list (1 ingredient) |
| **Quality ROI** | 1824.2 | 4955.0 |
| **Does the job?** | Oiling: yes · Hair fall: unclear | Oiling: yes |
| **Biggest concern** | "Chemical-free" and hair-fall claims; unreadable ingredients | None found |

## 1. Product snapshot

### Brand E Herbal Hair Oil
- **Net quantity / price:** 200 mL · $8.99 ($4.50 per 100 mL)
- **Claims:** "Ayurvedic", "Reduces hair fall", "Chemical-free"
- **Ingredients:** 1. Sesamum Indicum (Sesame) Oil, 2. Paraffinum Liquidum (Light Liquid Paraffin), 3. Eclipta Alba (Bhringraj) Extract, 4. Emblica Officinalis (Amla) Extract, 5. Bacopa Monnieri (Brahmi) Extract, 6. Parfum, **[UNREADABLE: glare covers about 2 lines after "Parfum"]**
- **Identifiers:** "Distributed by" US address printed (✅ read)
- **Allergens:** **Sesame**

### Brand F Pure Coconut Oil
- **Net quantity / price:** 500 mL · $9.99 ($2.00 per 100 mL)
- **Claims:** "100% pure", "Edible grade"
- **Ingredients:** 1. Cocos Nucifera (Coconut) Oil
- **Identifiers:** "Distributed by" US address printed (✅ read)

## 2. Ingredient risk check

| Product | Ingredient | Position | Tier | Why | Authority |
|---|---|---|---|---|---|
| E | Sesame oil | #1 | Low (allergen) | Sesame is a major food allergen; caution on skin for people allergic to it | [FDA, FASTER Act] |
| E | Light liquid paraffin | #2 | Low | Highly refined cosmetic-grade mineral oil is IARC Group 3 (not classifiable) | [IARC] |
| E | Parfum | #6 (additive) | Moderate | Undisclosed mixture; allergy trigger | [FDA] |
| E | [Unreadable lines] | — | — | Not rated. **We did not guess** | — |
| F | Coconut oil | #1 | — | No concern found | — |

## 3. Claim verification

| Product | Claim | Status | What we found |
|---|---|---|---|
| E | "Ayurvedic" | Unverifiable (−10) | No US legal definition (see `03`) |
| E | "Reduces hair fall" | **Misleading** (−25) | A hair-loss claim implies a drug effect, which a US cosmetic can't claim (FDA, cosmetic vs drug); no evidence cited |
| E | "Chemical-free" | **Misleading** (−25) | Every ingredient is a chemical, and this product includes mineral oil and fragrance |
| F | "100% pure" | Consistent | Single ingredient |
| F | "Edible grade" | Unverifiable (−10) | No US legal definition for "edible grade" |

## 4. Wellbeing Index

| Sub-score | Weight | Brand E | Brand F |
|---|---|---|---|
| Ingredient Safety | 35% | 90 | 100 |
| Processing Level | 15% | 75 (P2) | 100 (P1) |
| Additives | 15% | 85 *(provisional)* | 100 |
| Nutrition Balance (skin and hair) | 20% | 100 | 100 |
| Claim Integrity | 15% | 40 | 90 |
| **Wellbeing Index** | | **82** (81.5) ⚠️ Provisional | **99** (98.5) |
| Full ingredient list available? | | ⚠️ No: 6 known | Yes |

- **E Ingredient Safety:** sesame −5, paraffin −5 (Low ×1.25, top five) = **90**
- **E Additives:** 1 readable additive −3; parfum −12 = **85**. The unreadable lines may hold more additives, so the score could fall
- **E and F Nutrition Balance:** leave-on oils whose first ingredient is a nourishing oil (+5, capped at **100**); no harsh surfactants or drying alcohols
- **E Claim Integrity:** "Ayurvedic" −10, "reduces hair fall" −25, "chemical-free" −25 = **40**. **F Claim Integrity:** "edible grade" −10 = **90**
- A sub-score of 100 means **no deductions were found by this method**. It doesn't mean "perfect" or "medically proven"

| | Brand E | Brand F |
|---|---|---|
| Price per 100 mL | $4.50 | $2.00 |
| **Quality ROI** | **1824.2** | **4955.0** |

## 5. Verdict
**Better choice:** Brand F (**clear winner**, a 17-point gap, and more than twice the value per dollar). The winner has a complete list, so the verdict wording is not softened.
**Trade-offs**
- Brand E adds herbal extracts that some people prefer, but its hair-fall claim is a drug claim with no evidence, and "chemical-free" is misleading.
- **Ask for a clearer photo** of Brand E's back label to finish the score.

**Who should be careful**
- 🤧 **Allergies:** Brand E contains **sesame** and fragrance. Anyone sensitive to coconut should patch-test Brand F.
- 👶 **Children:** No authoritative data found for these products.
- 🤰 **Pregnancy:** No authoritative data found for these products.

**In-store tip:** A "chemical-free" label is a marketing line. Turn the bottle over and count the ingredients.

---

> *These samples are for training and illustration. They are not medical advice. Sample 1 reflects public labels on US sale websites as of the date shown; formulas change, so check the pack in hand. Samples 2 and 3 use fictional products.*
