# Business Requirements — Sales Pipeline Automation

## Scenario
A fictional consulting business wants a lightweight process for capturing prospects and ensuring new leads receive a timely follow-up.

## Goals
1. Store prospective customers as Salesforce Lead records.
2. Support a sales process that can convert qualified Leads into Accounts, Contacts, and Opportunities.
3. Automatically create a follow-up task when a new Lead is created.
4. Make task ownership and relationship to the Lead visible to sales users.

## Functional requirements
- **BR-01:** A user can create and save a Lead using Salesforce standard fields.
- **BR-02:** When a Lead is created, the active record-triggered Flow creates a Task.
- **BR-03:** The Task subject is “Follow up with new lead”.
- **BR-04:** The Task is related to the triggering Lead.
- **BR-05:** The Task starts with status “Not Started” and priority “Normal”.
- **BR-06:** The Task due date is set to the following day.
- **BR-07:** Qualified Leads can be converted using standard Salesforce functionality, subject to the configured org settings.

## Out of scope
Email/SMS delivery, production deployment, integrations, advanced duplicate handling, and formal security review are not included in this demonstration.

## Acceptance evidence
The current evidence verifies Task creation and that the Flow is active. Other acceptance scenarios are listed in the test plan and should be re-tested before formal sign-off.
