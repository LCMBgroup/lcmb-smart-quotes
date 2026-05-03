# V5 Build Plan - LCMB Smart Selector + Proposal System

## What changed

The project is no longer just a quote landing page. It now has two layers:

1. Smart Selector / Lead Qualifier
   - Used before the site inspection or before the customer knows exactly what they want.
   - Lets the customer choose ducted, split, solar, battery or combined pathways.
   - Asks simple property and preference questions.
   - Produces an indicative recommendation and estimate band.
   - Sends LCMB a summary and pushes the customer to book a site inspection.

2. Formal Proposal / Quote Page
   - Used after ServiceM8/GHL has the official quote.
   - Shows accurate scope, inclusions, optional upgrades, final pricing and acceptance pathway.

## Build stages

### Stage 1 - GitHub front-end MVP

Already started in V5.

- `smart-selector.html`
- customer pathway selection
- basic recommendation logic
- indicative estimate range
- email summary fallback
- booking person cards

### Stage 2 - GHL production form

Build a GHL form/survey with the same questions:

- pathway selected
- bedrooms/living rooms/storeys
- AC preferences
- solar/battery preferences
- floor plan upload
- preferred consultant
- preferred inspection date/time

Use GHL conditional logic so only relevant questions appear.

### Stage 3 - GHL calendar booking

Create three calendar links:

- Luke
- Ash
- Projects team / next available

Replace the placeholder mailto buttons in `smart-selector.html` with those GHL links.

### Stage 4 - Staff notifications

Set up GHL workflow to notify LCMB staff when a customer submits the selector.

Send notification by:

- email
- in-app notification
- SMS or WhatsApp if enabled

### Stage 5 - AI recommendation layer

After the GHL form is working, add AI through Make/Zapier/GHL webhook:

- customer answers go to automation
- AI returns recommended system tier and notes
- staff receive recommendation summary
- customer receives a polished response

### Stage 6 - Floor plan AI review

Floor plan upload is a separate stage.

The customer can upload a floor plan into GHL. Automation can then send it to an AI vision/document workflow for a suggested number of zones, outlets and likely ducted sizing. LCMB must review before quote is sent.

## Rule

AI can recommend and summarise. LCMB confirms sizing, final product selection and official pricing.
