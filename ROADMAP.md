# ROADMAP

## Immediate tasks
- Expand/unzip `unisc-fhir-teaching-lab-stage1-netlify-drop.zip` into the repo so files are versioned individually.
  - Recommended: unzip locally, then upload/extract via git/CLI for clean commit history.
  - Keep this repo synthetic-data-only.
- Add `.gitignore`, `README` linking to artifacts, and a `docs/` folder.
- Connect repo to Netlify and trigger a build deploy.

## Stage 2 features
- SMART on FHIR app launch + patient context
- CDS Hooks demo (patient-view hook -> informational card -> open SMART app)
- Terminology: SNOMED CT-AU / AMT / LOINC / UCUM via Ontoserver-style endpoints
- Wearable bridge: simulator first, then optional BLE Garmin broadcast
- Screenii gateway: validate + map Screenii metrics into FHIR Observations + DiagnosticReport
- Add tests: mapping + basic profile validation

## Useful references
- HL7 FHIR overview: https://www.hl7.org/fhir/overview.html
- SMART App Launch IG: https://build.fhir.org/ig/HL7/smart-app-launch/
- CDS Hooks: https://build.fhir.org/ig/HL7/cds-hooks/en/
- ADHA Standards Academy: https://www.digitalhealth.gov.au/digital-health-standards/standards-academy
