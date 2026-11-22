# MCCD Checker (pilot)

Checks the medical certificate of cause of death (MCCD, WHO international form) before it is signed and coded.

- **Who uses it:** certifying doctors (check before signing) and health information coders (review and code).
- **Pilot site:** Wesley Guild Hospital, Ilesa, Osun State, Nigeria.
- **What it does:** reads the cause-of-death section from a photo (or typed entry), runs rule checks (empty or out-of-order lines, missing or inconsistent intervals, more than one condition per line, abbreviations, mode of dying, ill-defined causes) and an AI review, and suggests the underlying cause with ICD-10 and ICD-11 codes for a trained coder to confirm.
- **Privacy:** names of the deceased and doctors are not stored; photos are not stored. Test data only until ethics and hospital approval.
- **Built with:** a single HTML page hosted on Netlify, with a Supabase database and an Edge Function that calls the Anthropic Claude API. No secret keys are kept in this repository.

Institute of Public Health, Obafemi Awolowo University, Ile-Ife.
Principal investigator: Akingbola Sunday Omokanye.
