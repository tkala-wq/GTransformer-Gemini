# 06 · Label-Reading Guide

**Topic:** How to read product photos (front and back), ingredient order, serving sizes and nutrition or supplement panels, how to check that the ingredient pull is correct, and what to do when a label can't be read.
**Last reviewed:** 2026-11-14

> **Golden rule:** if a label can't be read, **say so; never guess.** Write `[UNREADABLE: <what and where>]`, or `[NOT AVAILABLE: <what>]` when a web source doesn't publish it.
> The product **is still scored** from what is known, with the ⚠️ "Full ingredient list not available" warning (`01` §4, Missing data).
>
> **Common case:** brand and retailer websites often publish only "key ingredients" (e.g. three herbs), not the full list. Record them as known ingredients, mark the rest `[NOT AVAILABLE: full ingredient list not published online]`, and ask for a back-label photo to complete the score.

---

## 1. Input scenarios

| Scenario | What the user gives | What we do |
|---|---|---|
| **A. Photos** | Front and back photos of both products | Extract all 10 fields below from the images |
| **B. Typed details** | A web link or barcode for each product | Identify the product, fetch its label text **from a US sale website**, and mark the source as "web label" |
| **C. Hybrid** | Photos plus links or barcodes | Read the photos first, then fill gaps from the web label (**US sale websites only**). **If they conflict, the photo wins**, and the difference is noted |

### Guardrails (demo)
- 🇺🇸 **US sale websites only.** Every online lookup (label, ingredients, claims, price, link or barcode) uses only websites that sell the product **in the United States**. See the allowed list in `02-approved-sources.md` §7.
  - ✅ For example: the brand's US site (e.g. headandshoulders.com/en-us, srisritattvausa.com), wholefoodsmarket.com, amazon.com, walmart.com, target.com, cvs.com, walgreens.com.
  - ❌ Not allowed: sites selling outside the US, such as a brand's India site (srisritattva.com), bigbasket.com, 1mg.com, apollopharmacy.in, flipkart.com, nykaa.com, or amazon.in.
  - If a user sends a non-US link, identify the product, then look it up on a US sale website. If no US site carries it, say: *"This product isn't listed on a US sale website, so I can only use the label photos you send."*
- **Product universe:** products sold in the US at **Whole Foods Market**, or **Sri Sri Tattva** products sold in the US (e.g. srisritattvausa.com, Amazon.com).
- **Designated product pages:** when the project owner names a product page, use it as the primary web label for that product (see `02` §7). Sri Sri Tattva Protein Shampoo → [srisritattvausa.com/products/protein-shampoo](https://srisritattvausa.com/products/protein-shampoo?_pos=1&_psq=protein+sham&_psid=ff0d59a8f&_ss=e).
- **Market:** US. Prices are in **USD**, and US rules (FDA, USDA) give the legal status.
- **In scope:** personal care (soaps, shampoos, oils) and supplements.
- Out-of-scope product → reply: *"This demo covers personal care and supplements from Whole Foods and Sri Sri Tattva. I can still read the label, but the scoring hasn't been validated for this product."*
- **Compare like with like** (shampoo with shampoo, protein powder with protein powder). If the categories differ, say so and compare only the sub-scores that apply.

---

## 2. The 10 fields to extract

| # | Field | Where it is | Notes |
|---|---|---|---|
| 1 | **Brand and product name** | Front | Include the variant (e.g. "Chocolate", "Anti-Hairfall") |
| 2 | **Net quantity** | Front, bottom | mL, g, fl oz, oz, count. Needed for Quality ROI |
| 3 | **Price** | Typed by the user, or from a shelf photo or web listing | Note the currency and date |
| 4 | **Claims** | Front and back: badges, seals, slogans | Every claim goes to `03` |
| 5 | **Ingredients, in order** | Back | Exact spelling; keep brackets and percentages |
| 6 | **Active ingredients** | "Drug Facts" box (US OTC) or "Composition" (Ayurvedic) | Name and strength |
| 7 | **Nutrition or Supplement Facts panel** | Back or side | Serving size, servings per container, nutrients, %DV |
| 8 | **Allergens and warnings** | Back | "Contains:", "May contain", caution statements |
| 9 | **Regulatory identifiers** | Back or bottom | FSSAI licence (14 digits), AYUSH/drug licence no., NDC (US OTC), certifier name, veg/non-veg mark, organic seals |
| 10 | **Batch / lot, manufacturing and expiry dates, manufacturer and country** | Bottom, crimp or neck | Lot is needed to check recalls |

Record each field with a **confidence** mark: ✅ read clearly · ⚠️ partly read (state which part) · ❌ unreadable.

---

## 3. Reading the ingredient list

### Order means amount
- **Food and supplements (US):** listed in descending order of weight (21 CFR 101.4).
- **Cosmetics (US):** descending order of predominance, **except** that ingredients at **1% or less** may be listed in any order after those above 1%, and **colour additives may be listed last** in any order (21 CFR 701.3).
- **India (food):** descending order of weight or volume at the time of manufacture (FSSAI Labelling & Display Regulations 2020).
- **Practical rule:** the first 3–5 ingredients make up most of the product. A "hero" plant extract listed after the preservative (e.g. after phenoxyethanol, usually ≤1%) is present only in a **tiny amount**.

### Names to recognise
- **Cosmetics** use **INCI** names: *Aqua* = water, *Parfum* = fragrance, *Butyrospermum Parkii* = shea, *Cocos Nucifera* = coconut, *Sesamum Indicum* = sesame, *CI 42090* = FD&C Blue 1.
- **Ayurvedic** labels may use Sanskrit names with a botanical name: *Bhringraj* (Eclipta alba), *Amla* (Emblica officinalis), *Brahmi* (Bacopa monnieri), *Tila taila* (sesame oil).
- "-eth" or "PEG-" means **ethoxylated** (a 1,4-dioxane watch-point; Processing Level P3).
- "-paraben", "-isothiazolinone", "DMDM", "quaternium-15", "urea" (imidazolidinyl/diazolidinyl) → check `04`.
- "Fragrance", "parfum" or "aroma" is **one word that can hide many chemicals**.

### Compound ingredients
`Chocolate chips (sugar, cocoa butter, soy lecithin)`: list the sub-ingredients separately for scoring.

---

## 4. Reading the panels

### US Nutrition Facts (food)
1. **Serving size** first. All numbers are per serving.
2. **Servings per container.** Multiply if a person uses more.
3. **%DV:** 5% or less is low; 20% or more is high (FDA rule of thumb).
4. **Added sugars** has its own line and %DV.

### US Supplement Facts (21 CFR 101.36)
- Shows the **serving size** (e.g. "1 scoop (33 g)") and the amount and %DV of each dietary ingredient.
- **Proprietary blend:** only the total blend weight is required, not the amount of each ingredient → deduct under Nutrition Balance (`01` §3.4).
- `†` means "Daily Value not established".
- Compare the dose with **NIH ODS Upper Limits** at the **suggested daily use** (e.g. 2 scoops a day = 2 × panel).

### India nutrition information (FSSAI 2020)
- Given **per 100 g or 100 mL** and usually **per serve**, with %RDA per serve.
- **Green dot in a square = vegetarian; brown triangle in a square = non-vegetarian.**
- Health supplements must carry **"NOT FOR MEDICINAL USE"**.

### US Drug Facts (OTC anti-dandruff shampoo)
- **Active ingredient** and strength (e.g. "Pyrithione zinc 1%"), **purpose**, uses, warnings, directions, then **inactive ingredients**.
- The active and its strength must match 21 CFR 358.710 (see `03` §E).

---

## 5. Photo-reading tips

| Problem | What to do |
|---|---|
| **Glare or reflection** | Read the clear parts; mark the glare zone `[UNREADABLE: glare, lines 3–4 of ingredients]` |
| **Curved bottle; text wraps out of view** | Mark it as cut off: `[UNREADABLE: list continues beyond image edge]`. Ask for a side photo |
| **Very small font** | Read only what is certain; do not complete partial words from memory |
| **Several languages** | Use the English (or Hindi, if clear) panel; note the language |
| **Sticker over the original label** (imports) | Read both; the importer's sticker is the legal label for that market |
| **Blurry digits** (licence, lot, %) | Mark as ⚠️. Never round or infer a number |
| **Front and back from different variants** | Flag it and ask the user to confirm |

**Never:** guess an ingredient from the brand's other products, fill in a "typical" formula, or take the list from memory.

---

## 6. Ingredient pull check (required before scoring)

> **Why this step exists:** an app or web lookup can "succeed" but return the wrong thing: only the advertised key ingredients, a different variant, or the marketing text instead of the label. **Never score until the pull has passed this check.** If it fails, re-pull or ask for a photo. If that isn't possible, score with the ⚠️ warning (`01` §4, Missing data).

Run all 8 checks on **every product**, every time.

| # | Check | How to check | Fails when… |
|---|---|---|---|
| 1 | **Right source** | The page is the designated product page (`02` §7) or another US sale website, and the URL is recorded | No URL, a non-US site, or a different product page |
| 2 | **Right product** | The brand, product name, **variant** and **size** match the user's request or photo | E.g. the 2-in-1 or the 7 mL sachet instead of the 200 mL shampoo |
| 3 | **Full list, not "key ingredients"** | The text pulled is the label's ingredient list ("Ingredients:" / INCI list), not a "Key ingredients" or "Benefits" section | Only hero ingredients are listed (e.g. "Green gram, Fenugreek, Chickpea extract") |
| 4 | **Has a base** | Water-based products (shampoo, conditioner, lotion) list **water/aqua**, usually first | No water in a shampoo or lotion |
| 5 | **Has a functional ingredient for the job** | A shampoo or soap lists at least one **cleansing agent** (surfactant, e.g. "…sulfate", "…sulfonate", "…betaine", "…glucoside", "…isethionate", saponified oils). A supplement has a **Supplement Facts** panel | A shampoo with no cleanser |
| 6 | **Has a preservative** (water-based products) | E.g. phenoxyethanol, sodium benzoate, potassium sorbate, parabens, isothiazolinones | No preservative in a water-based product. Flag it, don't fail on it alone; some formulas use other preservation systems |
| 7 | **Plausible length** | Shampoos and lotions usually list **10–30** ingredients; supplements list every dietary ingredient in the panel | A shampoo with fewer than 6 ingredients |
| 8 | **Consistent with claims** | Claims such as "sulfate-free" or "paraben-free" can be checked against the list | A claim can't be checked because the list is missing |

**Result**

| Status | Rule | What happens next |
|---|---|---|
| ✅ **PASS** | Checks 1–5 and 7 pass | Score normally |
| ⚠️ **PARTIAL** | The list is real but some items are unconfirmed, or check 6 or 8 fails | Score, with the incomplete-list warning |
| ❌ **FAIL** | Any of checks 1–5 or 7 fails | **Re-pull** from the designated page, or ask for a back-label photo. If neither works, score from what is known with the warning, show "Ingredient pull: FAILED" in the report, and set confidence to Low |

**Record the result** in the hand-off record (section 7) and in the report's sources table (`07` §6):

```yaml
pull_check:
  status: PASS | PARTIAL | FAIL
  source_url: "<url>"
  pulled_at: 2026-11-14
  checks_failed: [3, 4, 5, 7]
  note: "Only 'key ingredients' returned; no water, cleanser or preservative"
  next_step: "Re-pull ingredient list from designated page, or request back-label photo"
```

---

## 7. Hand-off to scoring

After extraction **and the ingredient pull check (section 6)**, build this record per product, then follow `01` → `03`/`04`/`05` → `07`.

```yaml
product: "<brand> <name> <variant>"
category: personal_care | supplement
market: US
net_qty: { value: 13.5, unit: fl oz }
price: { value: 8.99, currency: USD, date: 2026-11-14 }
claims: ["...", "..."]
actives: [{ name: "Pyrithione zinc", strength: "1%" }]
ingredients: ["Water", "Sodium Laureth Sulfate", "..."]
panel: { serving: "33 g", per_serving: { protein_g: 24, added_sugars_g: 2, sodium_mg: 130 } }
allergens: ["milk", "soy"]
identifiers: { ndc: "", certifier: "", lot: "", expiry: "" }
unreadable: ["ingredients after 'Fragrance' (glare)"]
source: photo | web | hybrid
pull_check: { status: PASS | PARTIAL | FAIL, source_url: "", checks_failed: [] }
```
