# Demo 01: Sales Pipeline Automation

**Built by:** ACSKTech  
**Platform:** Salesforce Sales Cloud (Salesforce Developer Org)  
**Project type:** Independent portfolio demonstration using fictional data  
**Status:** Core follow-up automation verified

## Business problem
Sales teams need a consistent process to capture leads and ensure each new lead receives timely follow-up.

## Solution
A record-triggered Flow creates a follow-up Task when a Lead record is created. The wider demonstration also includes Salesforce standard lead, account, contact, and opportunity records.

## Implemented automation
- **Flow:** New Lead Follow-Up Task
- **Trigger:** Lead record is created
- **Action:** Create a Task related to the triggering Lead
- **Task subject:** Follow up with new lead
- **Status / priority:** Not Started / Normal
- **Due date:** Next day

## Evidence
The task-creation result and active Flow were reviewed during setup. Screenshot files still need to be committed to this repository before they can be displayed here.

## Scope and test status
The task creation behavior and active Flow status were checked in the Developer Org. Lead conversion and opportunity records were used during setup, but the full conversion scenarios should be re-tested before presenting them as formal acceptance tests. See [test scenarios](./test-scenarios.md).

## Further documentation
- [Business requirements](./business-requirements.md)
- [Solution design](./solution-design.md)
- [Test scenarios](./test-scenarios.md)

## Disclaimer
This is an independent ACSKTech portfolio demonstration using fictional records in a Salesforce Developer Org. It is not a production client implementation and does not represent endorsement by Salesforce or any customer.
