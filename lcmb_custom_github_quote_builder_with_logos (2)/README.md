# LCMB Smart Quotes - GitHub Pages Build

This folder contains the first no-developer version of the LCMB Group quote lander system.

## What this system does

1. You create your official quote in ServiceM8 or GHL.
2. You use ChatGPT to polish the wording.
3. You open `quote-generator.html`.
4. You paste the quote details into the form.
5. You preview the quote page.
6. You download the generated HTML file.
7. You upload that file into the `/quotes` folder on GitHub.
8. You send the customer the GitHub quote URL through ServiceM8 or GHL.

## Important privacy rule

GitHub Pages is public. Do not upload private notes, cost prices, margin, customer phone numbers, customer emails, internal notes or anything you would not be comfortable being public.

Recommended first version:
- Customer first name only
- Suburb instead of full street address
- ServiceM8 job number
- Scope
- Pricing that matches ServiceM8
- Payment terms
- Inclusions and exclusions

## Files

- `index.html` - simple homepage for the LCMB Smart Quote system.
- `quote-generator.html` - form used to create new customer quote pages.
- `quotes/example-quote.html` - demo customer quote page.
- `assets/site.css` - shared styling.
- `assets/lcmb-logo-main.png` - main LCMB logo used in quote headers.
- `assets/lcmb-logo-transparent.png` - transparent LCMB logo for darker sections if needed.
- `assets/lcmb-icon-square.png` - square LCMB icon option.
- `prompt.md` - ChatGPT prompt for quote copywriting.
- `GITHUB_SETUP_STEPS.md` - exact GitHub setup instructions.
- `SERVICE_M8_TO_QUOTE_WORKFLOW.md` - daily workflow.
- `EMAIL_SMS_TEMPLATES.md` - ServiceM8/GHL message templates.
- `QUOTE_CHECKLIST.md` - checklist before sending each quote.
- `robots.txt` - asks search engines not to index the site.
- `.nojekyll` - keeps GitHub Pages simple/static.
- `CNAME.example` - rename to `CNAME` later when setting up `quotes.lcmbgroup.com.au`.

## LCMB defaults included

Business: LCMB Group  
Phone: 0447563718  
Emails: office@lcmbelectrical.com.au and projects@lcmbelectrical.com.au  
Website: www.lcmbelectrical.com.au  
ABN: 80 680 633 416  
Areas: Gold Coast and Brisbane  
Services: Electrical, air conditioning, solar and battery  
Quote validity: 14 days  
Payment: 50% deposit, COD/on completion balance  
Warranty: 10-year workmanship warranty on LCMB workmanship, subject to conditions.
