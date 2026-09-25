# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Implementation codebase for a PhD research project: **Affect-Aware Graded Reading** — detecting learner confusion/disengagement from webcam facial signals while someone reads Japanese, and adapting LLM-generated story text (vocabulary, kanji/furigana, grammar, pacing) in response, then measuring whether that adaptation improves vocabulary retention against random-adaptation and static-text controls.

Three planned components, built across three studies:
- **Detector** — webcam → facial feature extraction (action units, head pose, gaze) → confusion/disengagement classifier.
- **Generator** — LLM story generation constrained to a JLPT level, enforced by a verifier (Japanese morphological tokenization + level lookup + regeneration on violation), with furigana rendering and spaced-repetition scheduling of target vocabulary.
- **Reading interface** — displays text, captures webcam, calls the detector, triggers adaptation, logs timestamped events; must support switching between affect-adaptive, random-adaptive, and static experimental conditions.

The full research brief (research questions, decisions of record with rationale, evidence base, study plan, open engineering decisions) is tracked in this assistant's memory system, not in this repo — consult it before making architecture or scoping calls, since many choices are already decided and justified rather than open for re-litigation.

## Status

No code has been written yet — the repository currently contains only this file and a stub README. There are no build, lint, or test commands to document. Update this file once a language/stack is chosen and the first component takes shape.
