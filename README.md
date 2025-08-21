# Advanced Personality Assessment (APA)

Dimensional, context-aware, cross-cultural personality assessment grounded in modern psychometrics. Moves beyond MBTI types and extends Big Five/HEXACO with richer traits, situational profiles, and change tracking.

## Why
- Typologies (e.g., MBTI) lose information and flip at cutoffs.
- Classic trait models underweight context, adaptability, and integrity.
- Personality shows both stability and malleability across time, culture, and situation.

## Core Model (8 dimensions)
- **SC**: Social Connectivity
- **CE**: Cognitive Exploration
- **ER**: Emotional Regulation
- **AE**: Agreeableness/Empathy
- **CS**: Conscientiousness/Self-Discipline
- **IH**: Integrity/Honesty
- **AF**: Adaptability/Flexibility
- **CI**: Creativity/Ingenuity

Each has 3–5 sub-facets. Scores are continuous (0–100). Higher-order factors (e.g., Stability/Plasticity) are derivable.

## Assessment Design
- **Contexts**: Work, Relationships, Leisure (situational specificity).
- **Items**: 120 total (15 per dimension × 3 contexts; 1–7 Likert with reverse-keying).
- **Adaptive logic**: After 2 items/dimension, skip remainder if mean ≤2 or ≥6.
- **Outputs**:
  - Trait scores + context-specific scores
  - Cross-Situational Variability (CSV) index
  - Temporal change indicators (test–retest)
  - Optional clustering into ~64 interpretable profiles (for feedback only)
- **UI**: Web tool (HTML/JS) with real-time scoring and a Chart.js radar plot; client-side by default.

## Psychometrics (Plan)
- **Samples**: ≥1,500 across languages/cultures; 6-month retest.
- **Analyses**: EFA → CFA; fit (CFI/TLI/RMSEA); α/ω ≥ .70; ICC for retest.
- **Invariance**: Configural/metric/scalar across language, gender, culture.
- **Validity**: Convergent/discriminant (BFI/HEXACO), criterion (work/relationship/health/creativity).
- **Bias controls**: Balanced keying, attention checks, response-time flags, social desirability residualization.

## Applications
- Career counseling & development planning
- Team composition & org development
- Personal growth & self-tracking
- Therapy/coaching (monitor change over time)

## Ethics & Privacy
- Built for development, not high-stakes selection.
- Informed consent; anonymize by default; GDPR-aligned options.
- Cultural sensitivity in translation and interpretation.
- Avoid deterministic labels; communicate uncertainty and variability.

## Quick Start (Demo)
1. Open `app/index.html` locally.
2. Complete items; adaptive skipping reduces length.
3. View scores, radar, context profiles, CSV. Export JSON locally.

## Repository Layout
- `/app` — HTML/CSS/JS (Chart.js UI, scoring)
- `/model` — Item bank, translations, scoring rules
- `/analysis` — EFA/CFA/invariance scripts and notebooks
- `/docs` — Method paper, FAQs, ethics guide

## Roadmap
- IRT-calibrated CAT and item bank expansion
- More contexts (school, sport), norms & percentiles
- Intervention tracking and change reports
- Open translation packs; REST/SDK for programmatic use

## License
TBD
