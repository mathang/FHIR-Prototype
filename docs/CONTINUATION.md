# Continuation notes (chat -> repo)

This repo started from a request to teach UniSC students modern digital health standards.

**Stage 1 is intentionally a sandbox**: Netlify-hosted React/Vite UI + Netlify Functions that simulate a small subset of FHIR R4 endpoints. All data is synthetic Screenii-style cases and no real patient data.

We parked full FHIR server hosting for later because Netlify is not a good home for a heavy Java/Postgres FHIR server. The Stage 1 goal is pedagogy: get students reading/writing FHIR-like resources, navigating a patient workspace, and understanding Observation/Patient/Encounter/Device relationships.

## Key decisions captured here

- HL7 FHIR R4 for resource language.
- SMART on FHIR as Stage 2 entry point for auth + context.
- CDS Hooks as Stage 3 for workflow-triggered decision support.
- Terminology is core: SNOMED CT-AU, AMT, LOINC, UCUM, ValueSet/CodeSystem/ConceptMap.
- Ontoserver/NCTS as the Australian FHIR terminology service examples.

## Immediate next steps

1. Extract the Stage 1 source zip and commit the files (so issues and diffs are clean).
2. Add `.gitignore` and standard repo hygiene (nvmrc, editorconfig, prettier/eslint configs).
3. Connect the repo to Netlify and deploy.

## Design ideas to revisit later

- Screenii gateway: Screenii -> Bluetooth/USB -> gateway -> validate/map -> FHIR.
- Wearable bridge: Garmin heart-rate broadcast or Health API -> Observation stream.
- Teaching emphasis: provenance, units, coding, “don’t over-interpret screening data”.
