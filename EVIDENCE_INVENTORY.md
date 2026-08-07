# Evidence inventory

**Scope:** public Clinical AI portfolio evidence available on 7 August 2026.  
**Purpose:** distinguish demonstrable artefacts from claims that require future validation.

## Selected projects

| Asset | Evidence available | Evidence type | Current integration | Explicit limit |
|---|---|---|---|---|
| [Clinical NLP Triage](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage-open-source) | Source code, synthetic dataset, lexicon, trace outputs, nine software tests, CI, synthetic baseline report, failure and safety documentation | Applied research prototype / synthetic technical evaluation | [PR #8 merge](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage-open-source/commit/597b677959f3d769ea2a4faee8f22770c7176efb); [PR #9 merge](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage-open-source/commit/8381a93896b1175ffbe1a85b2fa82d6454396d4d) | No clinical validation, patient use, deployment, safety or effectiveness evidence |
| [Clinical Reflection Band](https://github.com/Alfredo-Martin-Gil/clinical-reflection-band) | Concept paper, intended-use boundaries, failure modes, governance questions, research and evaluation roadmap | Research concept / conceptual architecture | [PR #1 merge](https://github.com/Alfredo-Martin-Gil/clinical-reflection-band/commit/8611ecdc95cd6f3dda02694f35a4f237609f57ed) | No implemented algorithm, model, empirical performance or deployment |
| [Prehospital Clinical Decision Uncertainty](https://github.com/Alfredo-Martin-Gil/prehospital-clinical-decision-uncertainty) | Clinical-operational analysis, workflow mapping, uncertainty and responsibility boundaries | Clinical foundation / operational analysis | [PR #1 merge](https://github.com/Alfredo-Martin-Gil/prehospital-clinical-decision-uncertainty/commit/73075aa0d1f24b4a3e541b1fba1ebe02e7b7fe60) | Not a guideline, protocol, validated instrument or software system |

## Historical repositories

| Repository | Status | Verification |
|---|---|---|
| [clinical-nlp-triage](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage) | Historical project description; redirects to the maintained flagship | [Historical-status merge](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage/commit/d9c52d3fb45d4906c2f32b927abc2bb76ade3470) |
| [clinical-nlp-triage-poc](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage-poc) | Historical rules-first POC; redirects to the maintained flagship | [Historical-status merge](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage-poc/commit/42c04c6ebf91042583921911edc1f58e619c1b6c) |

## Flagship synthetic baseline

- Dataset: 180 synthetic cases; no real patient data.
- Agreement with synthetic labels: 0.3611.
- Exact sensitivity for the synthetic `high` label: 0.1190.
- Synthetic `high` cases mapped to the legacy `low` output: 38/84 (0.4524).
- Zero lexicon hits: 106/180; 38 of those cases carry a synthetic `high` label.
- Interpretation: technical failure-characterisation only; not clinical performance, safety, efficacy, or validation evidence.

## Claims register

| Supported statement | Unsupported statement |
|---|---|
| Open research prototype using synthetic data | Validated or safe clinical AI |
| Nine software tests and synthetic evaluation in CI | Clinical sensitivity, efficacy, or improved outcomes |
| Published synthetic confusion matrix and failure analysis | Hospital deployment or real-world implementation |
| Clinical-operational foundation informed by professional experience | Validated guideline or protocol |
| Research-stage conceptual architecture | Implemented Clinical Reflection Band system |
| Governance and documentation scaffolding | Active/certified QMS or regulatory readiness |
| Interest in Canadian roles | Canadian project, residency, work authorisation, or Health Canada compliance |

## Reproducibility boundary

Repository links and integration commits above are public and auditable. Synthetic results can support technical review of logic, contracts, documentation, and failure behaviour. They cannot substitute for protocol-defined clinical validation with representative data, comparator standards, prospective governance, human-factors assessment, or deployment evidence.
