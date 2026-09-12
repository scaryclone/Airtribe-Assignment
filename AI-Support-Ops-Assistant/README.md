# AI Support Ops Assistant

An AI-assisted workflow for classifying and triaging customer support tickets.

## Structure
```
AI-Support-Ops-Assistant/
├── skills/
│   └── ticket_classification.md          # Skill defining categories, severity, priority, and escalation logic
├── test_cases/
│   └── ticket_classification/            # Test cases for the ticket_classification skill
│       ├── ticket_test_1.txt             # Sample ticket: refund request
│       └── ticket_test_2.txt             # Sample ticket: security breach
└── README.md
```

## Overview
- **skills/** contains the classification logic/prompt used to categorize and
  prioritize incoming support tickets (Billing, Technical, Product, Security,
  Legal) along with severity, priority, escalation status, and team assignment.
- **test_cases/** contains sample support tickets used to validate each skill,
  grouped into a subfolder named after the skill being tested.

## Usage
Feed a ticket from `test_cases/ticket_classification/` (or a real incoming
ticket) into the classification skill described in
`skills/ticket_classification.md` to get back structured JSON with category,
severity, priority, escalation status, assigned team, and reasoning.
