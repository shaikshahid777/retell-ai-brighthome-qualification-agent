# BrightHome Qualification Agent — Project Documentation

## 1. Project overview
This educational project uses Retell AI's Single Prompt setup to qualify callers requesting residential cleaning quotes for BrightHome Cleaning Services.

**Demo:** https://www.loom.com/share/c957cb77299f4eb8915e8383ba405247

## 2. Objectives
- Collect essential caller and property details.
- Keep the conversation structured and natural.
- Avoid re-asking information already supplied.
- Identify commercial/office cleaning and unrelated vendor/sales inquiries as out of scope.
- Summarize collected information and request confirmation.
- Avoid unsupported claims about service area or live appointment availability.

## 3. Agent configuration
- Platform: Retell AI
- Agent type: Single Prompt
- Agent name: BrightHome Qualification Agent
- Prompt sections: Role & Persona; Conversation Goal; Disqualification Checks; Qualification Questions; Closing & Summary.

## 4. Qualification fields
- Full name
- Callback phone
- Cleaning type
- Home size (bedrooms, bathrooms, or approximate square footage)
- Service address
- City
- ZIP code
- Preferred start timeframe
- Optional referral source

## 5. Disqualification behavior
- Commercial/office cleaning: explain that only residential cleaning inquiries can be assisted with, then end politely.
- Vendor/unrelated sales: decline politely and end the call.
- Service-area ZIP: do not guess. The official approved ZIP list was not supplied in the provided assessment materials, so eligibility must be confirmed.

## 6. Test results
The Retell dashboard showed the following simulation cases as Passed:
1. Happy Path Test — Fully Qualified Caller
2. Commercial Service Disqualification Test
3. Vendor / Spam Call Disqualification Test

These are dashboard-reported simulation results, not evidence of live phone deployment or successful real appointment booking.

## 7. Known limitations
- Official approved service-area ZIP list not provided.
- Complete official supported-services list not provided; commercial/office cleaning is treated as unsupported.
- Live availability lookup and appointment booking are not implemented or verified.
- The agent should not promise a confirmed appointment.

## 8. Assessment assets
- Loom demonstration: https://www.loom.com/share/c957cb77299f4eb8915e8383ba405247
- Repository: https://github.com/shaikshahid777/retell-ai-brighthome-qualification-agent
- LMS submission text: [lms-submission-description.txt](lms-submission-description.txt)
- Test results: [test-results.md](test-results.md)
- Limitations: [limitations.md](limitations.md)

## 9. Production-readiness note
Before real-world use, confirm official service-area data, supported services, business policies, privacy/data-retention requirements, and any scheduling integrations. This repository documents an educational assessment prototype.
