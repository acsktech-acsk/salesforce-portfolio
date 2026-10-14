# Test Scenarios — Sales Pipeline Automation

| ID | Test action | Expected result | Current status |
|---|---|---|---|
| TC-01 | Create a new Lead | Lead record is saved | Not formally re-tested |
| TC-02 | Create a Lead while the Flow is active | Follow-up Task is created and related to the Lead | **Pass — verified** |
| TC-03 | Inspect the Flow in Flow Builder | Flow status shows Active | **Pass — verified** |
| TC-04 | Convert a qualified Lead | Account and Contact are created or matched as configured | Performed during setup; re-test before formal sign-off |
| TC-05 | Create an Opportunity during conversion | Opportunity is associated with the intended Account | Performed during setup; re-test before formal sign-off |
| TC-06 | Create a Lead with missing optional fields | Flow behavior matches the intended business rules | Not tested |
| TC-07 | Review duplicate or repeat submissions | Tasks are created only according to the intended process | Not tested |

## Evidence
- evidence/follow-up-task-created.png shows the follow-up Task on a Lead record.
- evidence/flow-active.png shows the Flow active in Flow Builder.

**Testing note:** Only TC-02 and TC-03 are marked passed based on the checks confirmed so far. Do not describe the entire test suite as passed until the remaining cases are re-tested and documented.
