# Pokémon Card Sold-Price Reference by Grade — Raw, PSA 9, PSA 10 (508 Cards, 2026)

Median sold-price reference for 508 Pokémon cards across raw (ungraded), PSA 9, and PSA 10 eBay sales, compiled from real graded and ungraded sold comps (PokemonPriceTracker sold-listing data). 508 of 508 cards have a PSA 9 comp; the median PSA-10-over-PSA-9 grading premium across cards with both is 4.9×. Reference pricing only — sample sizes and confidence flags are included so nobody treats a thin-sample median as a firm price.

Data: [`gemsnipe-card-sold-price-reference.csv`](./gemsnipe-card-sold-price-reference.csv) — one row per card, 508 rows.

## Column notes — please read before citing

| column | meaning |
| --- | --- |
| `raw_price_usd` | median sold price for the ungraded (raw) card. |
| `raw_sample_count` | number of raw sold comps behind that median (all rows have ≥5). |
| `raw_confidence` | `high`/`medium`/`low` — a sample-size-based confidence flag, not a data-quality claim. |
| `psa9_price_usd` | median sold price for a PSA 9 grade of the same card. Blank if no PSA 9 comp exists. |
| `psa10_price_usd` | median sold price for a PSA 10 (Gem Mint) grade of the same card. |
| `psa10_over_psa9_multiple` | PSA 10 median ÷ PSA 9 median — the grading premium, where both exist. |
| `graded_sales_total` | total graded (PSA 9 + PSA 10) sold comps counted for this card. |

**This is reference pricing, not investment advice or a ranked opportunity list.** Rows are sorted by
total graded sales volume (most-traded first), not by price spread or expected value. Thin-sample rows
(low `raw_confidence`/`psa10_confidence`) should be treated as directional, not exact.

## Source and license

Compiled and maintained by **[GemSnipe](https://gemsnipe.com)** (gemsnipe.com) — a free centering + zoom tool for
grading Pokémon card listing photos by eye, plus real sold-comp pricing by grade, so a buyer can judge
a raw listing against what a PSA 10 of that card actually sells for. Licensed CC-BY-4.0.
