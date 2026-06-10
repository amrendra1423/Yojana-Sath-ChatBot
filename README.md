# Yojana Sathi — Multilingual Welfare Scheme Chatbot

Challenge 1.1 solution. Single-file web app: open `yojana-sathi.html` in any browser.

## Features
- **3 languages**: English, Hindi, Telugu (toggle in header; full UI + content translated)
- **10 high-impact schemes**: PM-KISAN, Ayushman Bharat (PM-JAY), PMAY-Gramin, Ujjwala, Jan Dhan, Atal Pension, PMMVY, NSAP old-age pension, Mudra, Sukanya Samriddhi
- **Eligibility flow**: 5 simple tap-button questions (age, gender, occupation, BPL/income, household) → personalised shortlist with reasons + where to apply
- **Document checklist**: downloadable `.txt` in the user's language + Share/SMS button
- **Voice**: mic input and text-to-speech in all 3 languages (Chrome recommended)

## Two modes
- **LLM mode**: click ⚙, paste an Anthropic API key → free-form chat powered by Claude, grounded in the scheme catalogue (won't invent schemes or amounts).
- **Demo mode** (no key): built-in rule-based flow, fully offline — safe for demos.

## Notes
- Scheme facts verified June 2026; amounts indicative — users are told to confirm at CSC/Gram Panchayat.
- All data lives in one `SCHEMES` array; adding a scheme or language is a data change only.
