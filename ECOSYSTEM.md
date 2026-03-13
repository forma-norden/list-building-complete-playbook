# Ecosystem: list-building-complete-playbook

How this repo connects to the rest of the Forma Norden GTM library.

## Works With

| Repo | Relationship | When to use together |
|------|-------------|---------------------|
| ``signal-based-list-building-workflow`` | Parallel | This playbook defines the strategic *why* and *who*; the workflow repo dictates the technical *how* (stacking signals in n8n/Clay). |
| ``sales-triggers-taxonomy`` | Upstream | The taxonomy defines the events you must look for during the Account Qualification phase of list building. |
| ``cold-email-copy-playbook`` | Downstream | The target lists built here are ultimately fed into the sequences defined in the copy playbook. |
| ``clay-claude-code-skill-pack`` | Downstream | Use the list building criteria defined here to execute physical enrichment runs inside Clay. |

## Suggested Skill Chains

1. The Data Ops Foundation: ``list-icp-definition`` (define the rules) > ``list-company-sourcing`` (find the logos) > ``list-contact-discovery`` (find the people) > ``list-data-validation-hygiene`` (verify everything).
