# Solution Design — Sales Pipeline Automation

## Data model
Uses standard Salesforce objects:
- **Lead:** initial prospect record and Flow trigger.
- **Task:** follow-up activity created by automation and related to the Lead.
- **Account, Contact, Opportunity:** standard sales records used in the lead-conversion demonstration.

## Automation design
1. A Lead is created.
2. The record-triggered Flow **New Lead Follow-Up Task** runs on Lead creation.
3. The Flow's Create Records element creates one Task with subject “Follow up with new lead”, status “Not Started”, priority “Normal”, a due date on the next day, and the triggering Lead as its related record.
4. A sales user can view the Task from the Lead's activity/task area.

## Configuration notes
- Confirm the Flow trigger and run settings in Flow Builder before modifying.
- Validate date/time behavior and any org-specific field requirements in the target org.
- Re-test lead conversion and opportunity association independently; they are standard Salesforce processes and are not created by the follow-up Flow itself.

## Limitations
This is a small Developer Org demonstration, not a production architecture. It does not include error monitoring, integrations, scale testing, or a formal deployment pipeline.
