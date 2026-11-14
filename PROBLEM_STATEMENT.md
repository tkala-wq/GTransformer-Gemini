# Problem Statement: Know Your Product, Wellbeing Comparison

*Source: "1. Problem Statement" (project brief). Markdown copy kept in the repo so changes are tracked.*

## Purpose
Help households, especially married couples, choose the healthier of two products. Score each product (**personal care**: soaps, shampoos, oils; **supplements**) on wellbeing, and explain the health risks of each choice.

- **What do we mean by wellbeing?** The product does its job (efficacy) without any side effects.
- **Packaging/claims:** the healthiest and best available, considering impact on the environment and the body. Packaging terms such as "Organic", "No GMO", "no micronutrients": are they really true, or fake news?
- **Health risks / side effects:** phthalates, BPA, and keywords on side effects that measure plastic issues.

## Use case
Head & Shoulders versus a protein shampoo. How do we compare the two products?

- **Inputs:** two product photos (front and back) plus their ingredient lists. Read the photos to get the brand, the claims (for example "organic" or "non-GMO"), the ingredients in order, the additives and the nutrition panel. If a label can't be read, say so instead of guessing.
- **Ingredient pull check:** before scoring, check that the app actually pulled the product's **full ingredient list**: the right product and variant, the label list rather than a "key ingredients" marketing list, and a plausible formula (e.g. a shampoo lists water and a cleansing agent). If the check fails, re-pull or ask for a back-label photo (`reference/06-label-reading-guide.md` §6).
- **Scenarios:**
  - Post two pictures of two products
  - Type product details for two products (web link or barcode)
  - Hybrid
- **Guardrails:**
  - Demo product universe: Whole Foods, Sri Sri Tattva.
  - 🇺🇸 **US sale websites only.** When looking up a product online (label, ingredients, claims, price, web link or barcode), use **only websites that sell the product in the United States**: for example the brand's US site, Whole Foods Market, Amazon.com, Walmart.com, Target, CVS or Walgreens. Do not use websites that sell outside the US (for example Indian retailers or a brand's India site). If no US sale website carries the product or its label details, say so.
  - **Designated product page:** Sri Sri Tattva Protein Shampoo → https://srisritattvausa.com/products/protein-shampoo?_pos=1&_psq=protein+sham&_psid=ff0d59a8f&_ss=e Product pages identify the product and its label only; risk ratings still come only from the approved sources.

## What to produce for each comparison
1. **Product snapshot:** name, claims made, and the full ingredient list.
2. **Ingredient risk check:** mark each ingredient of concern as Low, Moderate or High risk, and name the authority behind each rating.
3. **Claim verification:** check claims like "organic" against the key-terms registry. Flag claims that can't be verified or that mislead.
4. **Wellbeing Index (0–100) for each product:** show the sub-scores (ingredient safety, processing level, additives, nutrition balance and claim integrity). Add a "Quality ROI = Wellbeing Index / price / qty × 100".
5. **Verdict:** which product is the better choice for the household, the trade-offs, and who should be careful (children, pregnancy, allergies).

## Allowed sources (strict)
- **Government and accredited bodies:** FDA, USDA (including the National Organic Program), EPA, CDC, NIH, EFSA, WHO/IARC, Codex Alimentarius, FSSAI.
- **Official registries:** FDA import alerts, FDA recall data, GRAS notices, the Food Additive Status List, the USDA Organic Integrity Database, and import/export registries.
- **Reputable journalism** such as the New York Times, used only as context and never as the basis for a risk rating.
- (Double-check whether an extended list needs to be used.)
- Cite every risk claim. If none of these sources covers something, say "No authoritative data found."

## Key-terms registry
Keep a running glossary of label terms (organic, natural, non-GMO, clean label and so on). For each term, record the legal definition, the certifying body, and red flags that the term is being misused. Add new terms as you meet them.

## Tone
Plain language that a couple can act on in the store. Inform without alarming. This tool doesn't give medical advice.

## Topic files
| # | File | Topic |
|---|---|---|
| 1 | `reference/01-scoring-methodology.md` | Wellbeing Index weights, risk tiers and the scoring rules |
| 2 | `reference/02-approved-sources.md` | The allowed sources and URLs, plus which source wins when they conflict |
| 3 | `reference/03-key-terms-registry.md` | The label-term glossary (term, legal definition, certifier, red flags) |
| 4 | `reference/04-additives-and-ingredients-of-concern.md` | Flagged additives, their regulatory status and limits |
| 5 | `reference/05-regulatory-registries.md` | How to read FDA import alerts, recalls and GRAS notices, and the organic certification database |
| 6 | `reference/06-label-reading-guide.md` | How to read ingredient order, serving sizes and nutrition panels from photos |
| 7 | `reference/07-output-template.md` | The fixed comparison report format |
| 8 | `reference/08-sample-comparisons.md` | Worked examples that set the standard |

Keep each file to one topic so that search within the project finds the right one.

## Change log
| Date | Change |
|---|---|
| 2026-11-14 | Added guardrail: US sale websites only for online product lookups |
| 2026-11-14 | Designated the Sri Sri Tattva USA product page for Protein Shampoo |
| 2026-11-14 | Added the ingredient pull check step |
