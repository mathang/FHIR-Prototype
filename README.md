# FHIR-Prototype
Stage 1 teaching sandbox for HL7 FHIR R4, synthetic Screenii cases, Netlify Functions + React.

## Why Stage 1 is a sandbox (important)

This repo is a teaching sandbox for FHIR concepts. It is **not** a production FHIR server and **not** connected to real patient data. Data is synthetic Screenii-style older adult cases.

## Stage 1 architecture

- Frontend: React (TypeScript) in Vite
- Hosting: Netlify
- API: Netlify Functions that simulate a small subset of FHIR endpoints
- Data storage: synthetic JSON resources in the repo + browser localStorage for student-created observations
- Safety: loud "synthetic data" warning on every page

## What is included in the Stage 1 bundle

- Synthetic patient cases (Screenii-style measurements)
- FHIR R4 resource examples: Patient, Encounter, Observation, Device, Questionnaire, QuestionnaireResponse, DiagnosticReport
- Patient workspace + tabs
- FHIR resource browser
- Observation builder (creates Observations and stores them locally)

## Stage 2+ roadmap (from our planning chats)

1. SMART on FHIR app launch and context
2. CDS Hooks demo (patient-view card -> open SMART app)
3. Terminology integration: SNOMED CT-AU / AMT / LOINC / UCUM via Ontoserver/NCTS-style endpoints
4. Garmin/wearable data pathway (sim first; BLE broadcast if feasible)
5. Screenii gateway: validate + map Screenii metrics into FHIR Observations/DiagnosticReport

## Netlify deploy targets

- Build command: `npm run build`
- Publish directory: `dist`
- Functions directory: `netlify/functions`

## Continuing work

- Add tests for mapping functions and basic validator
- Add docs: clinical mapping notes and student workbook tasks
- Add GitHub issue templates for Stage 2 features
