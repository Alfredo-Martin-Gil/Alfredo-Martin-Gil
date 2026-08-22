# Public portfolio audit — 22 August 2026

## Scope and method

This audit covers all nine public repositories owned by Alfredo Martín Gil. It compares the public state found at the beginning of the improvement sprint with the verified state on 22 August 2026. Evidence is limited to public files, integration commits, pull requests, tests, generated artefacts, and GitHub Actions results. No claim is inferred from a title, draft, proposed roadmap, or professional interest.

## Executive result

The portfolio now has a coherent recruiter-facing structure for **Clinical AI & Healthcare Implementation**:

1. a clinical-operational foundation;
2. an auditable synthetic-data research prototype;
3. a bounded human-factors research concept;
4. two reproducible implementation case studies;
5. historical and basic exercises clearly separated from selected work.

The central improvement is not higher claimed performance. It is stronger traceability: reproducible code, explicit evidence levels, visible negative results, tests, CI, and clearer boundaries between an idea, a technical prototype, and clinical evidence.

## Repository-by-repository comparison

| Repository | Before | Verified state on 22 August 2026 | Portfolio role | Remaining limit |
|---|---|---|---|---|
| [Alfredo-Martin-Gil](https://github.com/Alfredo-Martin-Gil/Alfredo-Martin-Gil) | Profile did not consistently distinguish project maturity or connect evidence across repositories | Recruiter-facing narrative, evidence inventory, professional-development record, selected-project navigation, explicit non-claims, and this audit | Portfolio entry point | Public profile text cannot substitute for independent credential or employment verification |
| [clinical-nlp-triage-open-source](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage-open-source) | Prototype documentation, outputs, evaluation language, and safety claims were not fully coherent | Research prototype with 180 synthetic cases, deterministic outputs, nine tests, CI, traceability artefacts, failure analysis, and negative results preserved | Applied research prototype | Synthetic exact agreement 0.3611; sensitivity for the synthetic high label 0.1190; no clinical validation or patient use |
| [clinical-reflection-band](https://github.com/Alfredo-Martin-Gil/clinical-reflection-band) | Concept risked being read as an implemented capability | Explicitly bounded conceptual architecture with evidence/maturity inventory, failure modes, and proposed validation path | Research concept | No algorithm, dataset, benchmark, human-factors evaluation, clinical validation, or deployment |
| [prehospital-clinical-decision-uncertainty](https://github.com/Alfredo-Martin-Gil/prehospital-clinical-decision-uncertainty) | Clinical ideas were not positioned as a distinct evidence type | Clinical-operational foundation centred on uncertainty, reassessment, workflow, and responsibility boundaries | Clinical foundation | Not a guideline, protocol, validated instrument, or software system |
| [ehr-fhir-readmissions](https://github.com/Alfredo-Martin-Gil/ehr-fhir-readmissions) | README promised a cloud/BI workflow not reproducible from the repository; examples and SQL were not adequately bounded | Deterministic local workflow using six fully synthetic encounters; five quality rules; Patient, Encounter, and Observation resources; derived 30-day table; eight tests; MIT licence; CI on Python 3.11/3.12 | Interoperability implementation case study | FHIR-shaped subset has not been validated against an external validator, implementation guide, or national profile; no predictive model or deployment |
| [TFM_Cardiovascular_AI](https://github.com/Alfredo-Martin-Gil/TFM_Cardiovascular_AI) | Learned preprocessing and, for one dataset, SMOTE occurred before the train/test split, causing leakage | Split-first evaluation; training-only imputation, scaling, and Framingham SMOTE inside a pipeline; isolated test; fixed logistic baseline; six tests; CI; hashes and reproducible holdout report | Methodology-repair case study | Technical holdout only; no external validation, calibration for clinical use, fairness or geographic generalisation; dataset redistribution terms still need confirmation |
| [clinical-nlp-triage](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage) | Earlier description could be mistaken for the current implementation | README marks it historical and redirects to the maintained prototype | Historical record | GitHub repository archive flag remains unset |
| [clinical-nlp-triage-poc](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage-poc) | Early proof of concept competed with the flagship in discovery | README marks it historical and redirects to the maintained prototype | Historical record | GitHub repository archive flag remains unset |
| [EDA_BreastCancer_Sklearn](https://github.com/Alfredo-Martin-Gil/EDA_BreastCancer_Sklearn) | Basic notebook appeared without a maturity or portfolio-status boundary | README identifies it as a historical learning exercise using scikit-learn's built-in dataset and points reviewers to the current portfolio | Historical/basic exercise | No tests or CI are claimed; GitHub repository archive flag remains unset |

## Verified integrations

- Flagship safety/evaluation coherence: [merge commit 597b677](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage-open-source/commit/597b677959f3d769ea2a4faee8f22770c7176efb)
- Flagship residual-claim correction: [merge commit 8381a93](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage-open-source/commit/8381a93896b1175ffbe1a85b2fa82d6454396d4d)
- Clinical Reflection Band consolidation: [merge commit 8611ecd](https://github.com/Alfredo-Martin-Gil/clinical-reflection-band/commit/8611ecdc95cd6f3dda02694f35a4f237609f57ed)
- Prehospital foundation consolidation: [merge commit 73075aa](https://github.com/Alfredo-Martin-Gil/prehospital-clinical-decision-uncertainty/commit/73075aa0d1f24b4a3e541b1fba1ebe02e7b7fe60)
- Synthetic EHR-to-FHIR repair: [PR #1](https://github.com/Alfredo-Martin-Gil/ehr-fhir-readmissions/pull/1), [merge commit a1959bc](https://github.com/Alfredo-Martin-Gil/ehr-fhir-readmissions/commit/a1959bcb74c3195c354d2758ab3938a6376a6e28)
- Cardiovascular methodology repair: [PR #1](https://github.com/Alfredo-Martin-Gil/TFM_Cardiovascular_AI/pull/1), [merge commit 1efc3e6](https://github.com/Alfredo-Martin-Gil/TFM_Cardiovascular_AI/commit/1efc3e6bbbf0a29e759415ac1631d6ed4425b94c)
- Historical redirects: [clinical-nlp-triage](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage/commit/d9c52d3fb45d4906c2f32b927abc2bb76ade3470), [clinical-nlp-triage-poc](https://github.com/Alfredo-Martin-Gil/clinical-nlp-triage-poc/commit/42c04c6ebf91042583921911edc1f58e619c1b6c)
- Basic-exercise classification: [EDA commit 9d374f0](https://github.com/Alfredo-Martin-Gil/EDA_BreastCancer_Sklearn/commit/9d374f0a11b744870a58e7ed160ec28ca2c597f2)

## Reproducibility and CI checks

- The flagship's 180-case synthetic evaluation is versioned with machine-readable outputs and nine software tests.
- The EHR-to-FHIR workflow regenerates its artefacts and passes eight tests on Python 3.11 and 3.12.
- The cardiovascular workflow regenerates the locked holdout report, passes six methodology checks, and passed GitHub Actions on Python 3.11 and 3.12.
- The concept and clinical-foundation repositories intentionally contain no executable performance claim.
- Historical repositories and the basic EDA exercise are excluded from the selected portfolio narrative.

## Outstanding work that is real—not cosmetic

1. Set GitHub's archive flag for the two historical triage repositories and the basic EDA exercise if repository-administration access is used. Their README status is already aligned.
2. Confirm the original redistribution licences and authoritative provenance for both cardiovascular data files before treating the repository as a reusable dataset package.
3. If the cardiovascular study continues, pre-register an evaluation plan and add external/temporal validation, calibration, subgroup analysis, and clinically meaningful comparator work before any clinical-performance claim.
4. Validate the synthetic FHIR Bundle with an external validator and a deliberately selected implementation guide before making interoperability-conformance claims.
5. Improve the flagship only through versioned error analysis and protocol-defined evaluation. Its poor synthetic high-label sensitivity must remain visible until a reproducible change improves it.
6. Repository descriptions and topics should mirror the maturity labels when a repository-metadata editing capability is available.

## Permitted portfolio interpretation

The portfolio demonstrates clinical workflow analysis, safety-oriented problem framing, synthetic evaluation, interoperability prototyping, reproducibility, leakage repair, documentation, and governance boundaries. It does **not** demonstrate clinical validation, hospital deployment, improved outcomes, a medical device, an active QMS, Health Canada compliance, Canadian work authorisation, or production-scale software engineering.

## Resumen ejecutivo en español

El portfolio quedó organizado por nivel real de evidencia: fundamento clínico-operativo, prototipo de investigación con datos sintéticos, concepto de investigación y dos casos reproducibles de implementación. Los repositorios históricos y el ejercicio básico están separados del escaparate principal. Los resultados negativos y las limitaciones permanecen visibles; no se afirma validación clínica, despliegue ni cumplimiento regulatorio.
