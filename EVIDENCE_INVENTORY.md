# Evidence inventory

**Scope:** public Clinical AI portfolio evidence verified on 22 August 2026.  
**Purpose:** distinguish demonstrable artefacts from claims that require future validation. See the [comparative portfolio audit](PORTFOLIO_AUDIT_2026-08-22.md).

## Selected projects

| Asset | Evidence available | Evidence type | Current integration | Explicit limit |
|---|---|---|---|---|
| [Clinical NLP Triage](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage-open-source) | Source code, 180-case synthetic dataset, lexicon, trace outputs, nine software tests, CI, synthetic baseline report, failure and safety documentation | Applied research prototype / synthetic technical evaluation | [PR #8 merge](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage-open-source/commit/597b677959f3d769ea2a4faee8f22770c7176efb); [PR #9 merge](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage-open-source/commit/8381a93896b1175ffbe1a85b2fa82d6454396d4d) | No clinical validation, patient use, deployment, safety or effectiveness evidence |
| [Clinical Reflection Band](https://github.com/Alfredo-Martin-Gil/clinical-reflection-band) | Concept paper, intended-use boundaries, failure modes, governance questions, research and evaluation roadmap | Research concept / conceptual architecture | [PR #1 merge](https://github.com/Alfredo-Martin-Gil/clinical-reflection-band/commit/8611ecdc95cd6f3dda02694f35a4f237609f57ed) | No implemented algorithm, model, empirical performance or deployment |
| [Prehospital Clinical Decision Uncertainty](https://github.com/Alfredo-Martin-Gil/prehospital-clinical-decision-uncertainty) | Clinical-operational analysis, workflow mapping, uncertainty and responsibility boundaries | Clinical foundation / operational analysis | [PR #1 merge](https://github.com/Alfredo-Martin-Gil/prehospital-clinical-decision-uncertainty/commit/73075aa0d1f24b4a3e541b1fba1ebe02e7b7fe60) | Not a guideline, protocol, validated instrument or software system |

## Reproducible implementation case studies

| Asset | Evidence available | Evidence type | Current integration | Explicit limit |
|---|---|---|---|---|
| [Synthetic EHR to FHIR readmissions](https://github.com/Alfredo-Martin-Gil/ehr-fhir-readmissions) | Deterministic workflow; six synthetic encounters; five data-quality rules; Patient, Encounter and Observation resources; derived 30-day table; eight tests; licence; CI on Python 3.11/3.12 | Synthetic interoperability implementation | [PR #1 merge](https://github.com/Alfredo-Martin-Gil/ehr-fhir-readmissions/commit/a1959bcb74c3195c354d2758ab3938a6376a6e28) | FHIR-shaped subset not externally validated against an implementation guide or national profile; no prediction, deployment or clinical validation |
| [Cardiovascular ML methodology audit](https://github.com/Alfredo-Martin-Gil/TFM_Cardiovascular_AI) | Split-first workflow; training-only imputation, scaling and Framingham SMOTE inside pipelines; isolated test; fixed logistic baseline; file hashes; locked holdout report; six tests; CI on Python 3.11/3.12 | Reproducible methodology repair / technical holdout evaluation | [PR #1 merge](https://github.com/Alfredo-Martin-Gil/TFM_Cardiovascular_AI/commit/1efc3e6bbbf0a29e759415ac1631d6ed4425b94c) | Dataset redistribution terms require confirmation; no external validation, clinical calibration, fairness, geographic generalisation or patient-use evidence |

## Historical and basic repositories

| Repository | Status | Verification |
|---|---|---|
| [clinical-nlp-triage](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage) | Historical project description; redirects to the maintained flagship | [Historical-status merge](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage/commit/d9c52d3fb45d4906c2f32b927abc2bb76ade3470) |
| [clinical-nlp-triage-poc](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage-poc) | Historical rules-first POC; redirects to the maintained flagship | [Historical-status merge](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage-poc/commit/42c04c6ebf91042583921911edc1f58e619c1b6c) |
| [EDA_BreastCancer_Sklearn](https://github.com/Alfredo-Martin-Gil/EDA_BreastCancer_Sklearn) | Historical/basic learning exercise; excluded from the selected portfolio | [Status commit](https://github.com/Alfredo-Martin-Gil/EDA_BreastCancer_Sklearn/commit/9d374f0a11b744870a58e7ed160ec28ca2c597f2) |

Their GitHub archive flags were still unset when verified. The public README status, not the archive flag, currently supplies the maturity boundary.

## Flagship synthetic baseline

- Dataset: 180 synthetic cases; no real patient data.
- Agreement with synthetic labels: 0.3611.
- Exact sensitivity for the synthetic `high` label: 0.1190.
- Synthetic `high` cases mapped to the legacy `low` output: 38/84 (0.4524).
- Zero lexicon hits: 106/180; 38 of those cases carry a synthetic `high` label.
- Interpretation: technical failure-characterisation only; not clinical performance, safety, efficacy, or validation evidence.

## Reproducible holdout results

The cardiovascular metrics are bound to the exact versioned files, split, environment and fixed baseline. They are not clinical estimates.

| Dataset | ROC AUC | Balanced accuracy | Precision | Interpretation |
|---|---:|---:|---:|---|
| Cardiovascular 70k secondary copy | 0.778089 | 0.713621 | — | Technical holdout only |
| Framingham secondary copy | 0.696855 | 0.637114 | 0.249191 | Negative precision result retained; technical holdout only |

## Claims register

| Supported statement | Unsupported statement |
|---|---|
| Open research prototype using synthetic data | Validated or safe clinical AI |
| Nine flagship software tests and synthetic evaluation in CI | Clinical sensitivity, efficacy, or improved outcomes |
| Deterministic synthetic EHR-to-FHIR workflow with quality checks | FHIR conformance, hospital integration or operational interoperability |
| Leakage-controlled cardiovascular holdout workflow | Clinical prediction performance or geographic generalisation |
| Clinical-operational foundation informed by professional experience | Validated guideline or protocol |
| Research-stage conceptual architecture | Implemented Clinical Reflection Band system |
| Governance and documentation scaffolding | Active/certified QMS or regulatory readiness |
| Interest in Canadian roles | Canadian project, residency, work authorisation, or Health Canada compliance |

## Reproducibility boundary

Repository links and integration commits above are public and auditable. Synthetic and holdout results can support technical review of logic, contracts, documentation, data handling, and failure behaviour. They cannot substitute for protocol-defined clinical validation with representative data, comparator standards, independent provenance review, prospective governance, human-factors assessment, or deployment evidence.
