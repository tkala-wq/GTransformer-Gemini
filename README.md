# GTransformer: Know Your Product, Wellbeing Comparison

Helps households, especially married couples, choose the healthier of two products, either **personal care** (soaps, shampoos, oils) or **supplements**. Each product gets a 0–100 **Wellbeing Index**, and the report explains the health risks of each choice, in plain language that can be acted on in the store.

> **Wellbeing** = the product does its job (efficacy) without side effects, for the body and the environment.
> This tool informs choices. It does not give medical advice.

## How a comparison works

1. **Input:** front and back photos, a web link or barcode, or both (hybrid). Demo product universe: **Whole Foods** and **Sri Sri Tattva**, as sold in the US.
   🇺🇸 **Online lookups use US sale websites only** (e.g. the brand's US site, Amazon.com, Walmart.com). See [PROBLEM_STATEMENT.md](PROBLEM_STATEMENT.md) and `reference/02-approved-sources.md` §7.
2. **Read the label** → `reference/06-label-reading-guide.md`
3. **Check the ingredient pull** → `reference/06-label-reading-guide.md` §6. Is it the right product, the full list (not just "key ingredients"), and a plausible formula? FAIL → re-pull or ask for a back-label photo
4. **Check ingredients** → `reference/04-additives-and-ingredients-of-concern.md`
5. **Verify claims** → `reference/03-key-terms-registry.md` + `reference/05-regulatory-registries.md`
6. **Score** → `reference/01-scoring-methodology.md`
7. **Cite only approved sources** → `reference/02-approved-sources.md`
8. **Write the report** → `reference/07-output-template.md` (see the examples in `reference/08-sample-comparisons.md`)

## Topic files (one topic per file)

| File | Topic |
|---|---|
| [01-scoring-methodology.md](reference/01-scoring-methodology.md) | Wellbeing Index weights, risk tiers, scoring rules, Quality ROI |
| [02-approved-sources.md](reference/02-approved-sources.md) | Allowed sources and URLs, trust tiers, conflict rules |
| [03-key-terms-registry.md](reference/03-key-terms-registry.md) | Label-term glossary: legal definition, certifier, red flags |
| [04-additives-and-ingredients-of-concern.md](reference/04-additives-and-ingredients-of-concern.md) | Flagged ingredients, regulatory status, limits, allergens |
| [05-regulatory-registries.md](reference/05-regulatory-registries.md) | Reading FDA recalls, import alerts, GRAS, the USDA OID, FSSAI |
| [06-label-reading-guide.md](reference/06-label-reading-guide.md) | Reading ingredient order, panels and photos |
| [07-output-template.md](reference/07-output-template.md) | The fixed comparison report format |
| [08-sample-comparisons.md](reference/08-sample-comparisons.md) | Three worked examples (fictional products) |

## Open decisions for the project owner

- **Approve or reject the proposed extra sources** in `02` §5 (EU Commission/SCCS, CDSCO, AYUSH, FTC, OEHHA). The core list leaves personal care in India thin. Ratings marked † depend on them.
- **Confirm the Quality ROI formula reading** in `01` §6 (WI ÷ price per 100 mL or g × 100).
- **Process Flow diagram:** not yet in the shared Drive folder. Once added, map its steps to these files.

## Source document
Derived from *1. Problem Statement* (project brief). A tracked copy, including later changes, is in [PROBLEM_STATEMENT.md](PROBLEM_STATEMENT.md).
