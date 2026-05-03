# GHL Automation Checklist for LCMB Smart Selector

## 1. Create custom fields

Create fields for:

- Selected pathway
- Property type
- Levels
- Bedrooms
- Living areas
- Extra rooms
- Roof type
- Floor plan upload
- AC outcome
- Zoning preference
- AC brand preference
- Ducting preference
- Quarterly power bill
- Daytime power use
- Solar brand preference
- Battery goal
- Backup circuits
- Battery brand preference
- Add-ons
- Preferred consultant
- Indicative estimate band
- AI recommendation notes

## 2. Create form or survey

Use the same question order as `smart-selector.html`.

Use conditional logic:

- if ducted/split selected, show AC questions
- if solar/battery selected, show solar/battery questions
- if battery selected, show backup questions
- if customer has floor plan, show upload field
- if they request inspection, show calendar links

## 3. Create booking calendars

Create one calendar per person:

- Luke
- Ash
- Projects team / next available

Copy each booking URL into `smart-selector.html` inside the `CONFIG.bookingLinks` section.

## 4. Create workflow

Trigger:

- Form submitted or survey submitted

Actions:

- Create/update contact
- Create opportunity in pipeline
- Assign tag based on pathway
- Send internal notification to LCMB team
- Send customer confirmation SMS/email
- Optional: send data to AI automation

## 5. Customer confirmation message

Example:

Hi {{contact.first_name}}, thanks for completing the LCMB system selector. Our team has received your preferences and will confirm the best next step. If you booked a site inspection, we will confirm details shortly.

## 6. Staff notification message

Example:

New LCMB Smart Selector lead.

Pathway: {{custom.selected_pathway}}
Customer: {{contact.name}}
Phone: {{contact.phone}}
Suburb: {{contact.city}}
Preferred consultant: {{custom.preferred_consultant}}
Estimate band: {{custom.indicative_estimate_band}}

Review the form answers and call the lead.
