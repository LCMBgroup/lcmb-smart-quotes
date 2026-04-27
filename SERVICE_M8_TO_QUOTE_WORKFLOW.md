# LCMB daily quote workflow

## Goal

Keep ServiceM8/GHL as the official source of truth and use GitHub only as the customer-facing proposal page.

## Daily workflow

1. Create the quote in ServiceM8 or GHL as normal.
2. Confirm:
   - Customer name
   - Job address or suburb
   - ServiceM8 job number
   - Quote date
   - Valid-until date
   - Line items
   - Subtotal
   - GST
   - Total inc GST
   - Payment terms
   - Inclusions
   - Exclusions
3. Copy the quote details into ChatGPT using `prompt.md`.
4. Review ChatGPT's wording.
5. Open `quote-generator.html`.
6. Paste the final wording and pricing into the generator.
7. Paste the ServiceM8 or GHL acceptance link into the acceptance link field if available.
8. Preview the quote.
9. Download the HTML file.
10. Upload the file into the `/quotes` folder in GitHub.
11. Open the live GitHub quote URL and check it on your phone.
12. Send the quote link to the customer through ServiceM8 or GHL.
13. The customer accepts through ServiceM8/GHL or emails acceptance.
14. Convert/continue the job inside ServiceM8/GHL as normal.

## Fallback rule

If anything goes wrong, send the normal ServiceM8/GHL quote.

Do not delay urgent quotes while troubleshooting the GitHub page.

## File naming rule

Use this format:

```text
SM8JOBNUMBER-customerfirst-suburb.html
```

Examples:

```text
sm8-1042-sarah-burleigh-heads.html
sm8-1188-robert-palm-beach.html
sm8-1201-tt-brisbane.html
```

Avoid surnames where possible.

## What must never go on GitHub

- Internal notes
- Cost prices
- Margins
- Supplier costs
- Customer private details unless approved
- Customer phone numbers
- Customer email addresses
- Photos containing sensitive/private information
- Unsafe claims
- Promises of guaranteed savings or guaranteed same-day availability
