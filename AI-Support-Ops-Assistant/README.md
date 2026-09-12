# AI Support Ops Assistant

An AI-assisted workflow for classifying and triaging customer support tickets.

## Structure
```
AI-Support-Ops-Assistant/
├── skills/
│   └── ticket_classification.md   # Skill defining categories, priorities, and classification logic
├── test_cases/
│   ├── ticket_test_1.txt          # Sample ticket: account login issue
│   └── ticket_test_2.txt          # Sample ticket: billing/duplicate charge
└── README.md
```

## Overview
- **skills/** contains the classification logic/prompt used to categorize and
  prioritize incoming support tickets (e.g., Billing, Technical, Account,
  Feature Request, General Inquiry) along with urgency levels.
- **test_cases/** contains sample support tickets used to validate the
  classification skill against realistic scenarios.

## Usage
Feed a ticket from `test_cases/` (or a real incoming ticket) into the
classification skill described in `skills/ticket_classification.md` to get
back a category, priority, and reasoning for routing the ticket to the
correct team.
