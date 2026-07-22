# AIxcellentSport Agent Guide

## Product
- Open-source, browser-based AI movement coach.
- Raw camera frames stay on-device in the MVP.
- Feedback is educational and must not be presented as medical diagnosis.

## Run
- Install: `npm ci`
- Develop: `npm run dev`
- Verify: `npm run lint && npm test`

## Architecture
- `app/page.tsx`: camera, MediaPipe inference, exercise rules, UI.
- `app/globals.css`: visual system and responsive layout.
- `tests/`: product-contract checks.
- `docs/`: architecture and product decisions.

## Conventions
- Keep movement rules explainable and exercise-specific.
- Do not upload or persist video without explicit user consent.
- New exercises need a phase definition, rep rule, feedback rule, and test.
- Avoid accuracy or safety claims without reproducible evidence.
- Keep the public demo usable without an account or paid API.

## Current State
- MVP supports squat, push-up, and jumping-jack feedback.
- Next: calibration, session history, and extensible exercise profiles.
