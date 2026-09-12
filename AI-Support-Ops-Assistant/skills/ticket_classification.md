# Ticket Classification Skill

## Purpose
Classify incoming support tickets into categories so they can be routed to the
right team and prioritized correctly.

## Categories
- **Billing** — payment failures, invoices, refunds, subscription/plan changes
- **Technical** — bugs, errors, crashes, integration/API issues
- **Account** — login/access issues, password resets, permissions, profile changes
- **Feature Request** — suggestions or requests for new functionality
- **General Inquiry** — questions that don't fit the above categories

## Priority Levels
- **Urgent** — service outage, security issue, data loss, payment blocking access
- **High** — major feature broken, affects many users
- **Medium** — minor bug or issue affecting a single user's workflow
- **Low** — cosmetic issues, general questions, feature requests

## Classification Steps
1. Read the ticket subject and body.
2. Identify keywords that map to a category (e.g., "invoice", "charge" → Billing;
   "error", "crash", "500" → Technical; "can't log in", "password" → Account).
3. Assign a category based on the strongest keyword/context match.
4. Assess urgency based on impact (outage/security > broken feature > minor bug > question).
5. Output the ticket with: `category`, `priority`, and a one-line `reason`.

## Example Output Format
```
Category: Technical
Priority: High
Reason: User reports the API is returning 500 errors on all requests.
```
