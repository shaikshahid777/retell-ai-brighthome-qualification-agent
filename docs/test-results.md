# Test Results

## Dashboard-reported simulation outcomes

The Retell AI dashboard showed these three test cases as **Passed**:

| Test case | Result | Observed behavior |
| --- | --- | --- |
| Happy Path Test — Fully Qualified Caller | Passed | Captured the key caller details, summarized them for confirmation, and closed politely. |
| Commercial Service Disqualification Test | Passed | Recognized commercial/office cleaning as out of scope and ended the call without continuing qualification. |
| Vendor / Spam Call Disqualification Test | Passed | Identified an unrelated sales inquiry, declined politely, and ended the call. |

## Scope of this evidence

- These are simulation results visible in the Retell AI dashboard.
- They do not prove live phone deployment or real appointment booking.
- The official service-area ZIP list was not provided, so out-of-area ZIP disqualification has not been verified against an authoritative list.
- Keep screenshots sanitized; never publish API keys, credentials, or private caller data.
