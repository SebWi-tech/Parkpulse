# ParkPulse — Acceptance Tests

## Status
These tests are planned. No execution results are recorded yet.

| Test ID | Requirement | Test action | Expected result | Status |
|---|---|---|---|---|
| T-01 | REQ-02 | Select a destination with three assigned facilities. | Exactly those three facilities appear. | Not tested |
| T-02 | REQ-04 | Open a facility with simulated availability. | A visible demo notice is displayed. | Not tested |
| T-03 | REQ-06 | Apply a valid EUR 2 code to a EUR 6 parking fee. | The parking amount is EUR 4. | Not tested |
| T-04 | REQ-06 | Enter an invalid or used code. | The code is rejected and a clear message appears. | Not tested |
| T-05 | REQ-14 | Reload a successful payment confirmation. | No additional stamp is created. | Not tested |
| T-06 | REQ-15 | Complete an eligible session with five stamps already recorded. | Exactly one voucher is issued and the counter resets. | Not tested |
| T-07 | REQ-17 | Simulate payment failure with a selected voucher. | The voucher remains available and no stamp is added. | Not tested |
| T-08 | REQ-08 | Open checkout for a parking and charging session. | Parking and charging costs are shown separately. | Not tested |

## Execution log
After running a test, record:
- Date
- Tester
- Tested app version or commit
- Actual result
- Passed or Failed
- Screenshot or issue reference, if relevant
