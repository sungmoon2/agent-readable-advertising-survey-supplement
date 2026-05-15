# S8 AARS Synthetic Example

This example is synthetic. It is not a reported experiment and should not be cited as empirical evidence.

## Scenario

An AI commerce agent observes a legacy display advertisement for a discounted consumer product on a web page. The ad includes a visible price, a discount claim, a sponsor label, and a call-to-action button.

## Example Representation Sketch

| AARS field family | Synthetic example value |
|---|---|
| Ad identity | `creative_id: synthetic-demo-001`; `placement_context: right-rail display ad` |
| Sponsor/seller identity | `advertiser_name: Example Retailer`; `sponsor_disclosure: Sponsored` |
| Creative evidence | OCR span for discount text; bounding box for product image; DOM node for call-to-action button |
| Product/offer facts | `product_name: Example Headphones`; `price: USD 49.99`; `discount: 30 percent` |
| Claims | `claim_text: 30 percent off today`; `claim_type: price/discount`; `evidence_pointer: OCR span` |
| Disclosure/provenance | sponsored label observed; seller chain not available in this synthetic example |
| Policy/risk signals | no restricted category in the synthetic example; risk status unreviewed |
| Agent action constraints | require user confirmation before purchase or subscription |
| Audit metadata | extractor model/version and timestamp fields reserved |

## Use

The purpose of this example is to show the intended structure of the AARS reference schema. It does not establish that any existing C7/C8 standard already provides all fields.
