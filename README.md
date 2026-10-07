# BrightHome Qualification Agent

A Retell AI voice agent prototype built for the Tayana Academy Retell AI Topic 1 assessment. The agent qualifies callers seeking residential cleaning quotes, collects essential details, handles out-of-scope inquiries, and summarizes the caller's requirements.

## Demo
- **Loom walkthrough:** https://www.loom.com/share/c957cb77299f4eb8915e8383ba405247

## Agent configuration
- **Platform:** Retell AI
- **Agent type:** Single Prompt
- **Agent name:** BrightHome Qualification Agent
- **Use case:** Residential cleaning quote qualification
- **Prompt structure:** Role & Persona, Conversation Goal, Disqualification Checks, Qualification Questions, Closing & Summary

## Qualification information collected
- Full name
- Callback phone
- Cleaning type
- Home size (bedrooms, bathrooms, or approximate square footage)
- Property service address
- City and ZIP code
- Preferred start timeframe
- Optional referral source

The agent is instructed to ask one question at a time, remember information already provided during the current call, avoid unnecessary repetition, and confirm the collected details before ending a qualified inquiry.

## Disqualification behavior
- Commercial or office cleaning: politely explain that the agent can only assist with residential cleaning inquiries and end the call.
- Vendor or unrelated sales calls: politely decline and end the call.
- Service-area eligibility: the official approved ZIP-code list was not included in the supplied assessment materials. The agent must not invent ZIP codes or claim that an area is supported or unsupported without verified data; eligibility is deferred for confirmation.

## Test evidence
The following Retell simulation test cases were shown as **Passed** in the dashboard:
- Happy Path Test - Fully Qualified Caller
- Commercial Service Disqualification Test
- Vendor / Spam Call Disqualification Test

These are dashboard-reported simulation results, not a claim that a live phone deployment was tested. Refer to the Loom demo and assessment screenshots for visible evidence.

## Known limitations
- The official service-area ZIP-code list was not provided in the supplied materials.
- The complete official supported-service list was not provided; commercial/office cleaning is explicitly treated as unsupported.
- Live appointment availability and booking are not integrated or verified. The agent does not promise a confirmed appointment.
- Testing should be repeated if the official business data or prompt configuration changes.

## Repository contents
- `README.md` — project summary and usage notes
- `docs/project-documentation.pdf` — assessment project documentation
- `docs/lms-submission-description.txt` — copy-ready LMS description

## Disclaimer
This is an educational assessment project. Do not use it as a production scheduling service until official business policies, service-area data, supported services, privacy requirements, and any needed scheduling integrations are verified.
