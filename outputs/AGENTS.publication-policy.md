# Computational Research and Publication Policy

Apply requirements in proportion to the work level. Do not burden disposable exploration with publication controls.

## Classification and triggers

Classify computational work as:

- **Exploratory:** scratch calculations, debugging, learning, and hypothesis generation. Not reliable evidence for a paper or consequential decision.
- **Validated:** results shared as reliable or used for internal decisions, talks, reports, or sustained collaboration.
- **Publication-level:** final manuscript/thesis/report results, public research releases, and final numbered computational figures or tables.

Treat an explicit request such as “make this publication-ready,” “publication-level,” or “promote this to final paper production” as activating publication-level requirements. Manuscript submission/public release and designation as a final numbered computational figure or table also activate them. Promote earlier work by regenerating or reconstructing it under the stricter level; do not pretend incomplete provenance is complete.

Follow applicable law, ethics approvals, data-use agreements, funder rules, journal policies, and repository-specific instructions over this block.

## Exploratory work

- Notebooks, interactive work, ad hoc scripts, and temporary outputs are acceptable.
- Preserve only enough context for active use, unless the result is likely to be promoted.
- Label provisional artifacts when they could be mistaken for final results.
- Never expose secrets or mishandle restricted data.

## Validated work

- Version-control consequential code, configuration, and documentation.
- Record input identifiers/checksums, parameters, units, preprocessing, relevant software/runtime versions, and hardware when result-affecting.
- Capture the environment with appropriate specifications or lockfiles.
- For stochastic work, record seeds and random-library versions and use deterministic execution where scientifically appropriate. For unavoidable nondeterminism, quantify variability or define tolerances.
- Retain machine-readable outputs sufficient to audit central results.
- Run meaningful risk-proportionate checks (tests, benchmarks, invariants, convergence, analytical limits, alternative implementations, or independent review) and record limitations.

## Publication-level production

- Every final numbered computational figure and table must be produced by a dedicated, checked-in, non-interactive driver with a clear artifact-specific name such as `generate_figure_2.py` or `generate_table_1.R`.
- Put shared numerical logic in import-safe modules and keep production drivers thin. Do not leave final artifacts dependent solely on notebooks, interactive state, manual plotting, copied values, or undocumented commands.
- Encode or read versioned configuration for the exact model, inputs, parameters, grids, seeds, normalization, labels, dimensions, and output filenames used by the manuscript. Accept an output-directory option when practical.
- Write both the final rendered artifact and compact machine-readable source data sufficient to audit or replot it. Include schemas/data dictionaries, units, and provenance. Use open formats where practical.
- Preserve permitted raw inputs, or record immutable identifiers, checksums, access instructions, and the transformation path. Do not copy restricted or licensed data into the repository.
- Link outputs to the code revision, input versions/checksums, configuration, and generation time, preferably in a machine-readable manifest.
- Provide a documented top-level command that regenerates all final artifacts when practical. For costly or inaccessible computation, document staged commands and retain auditable intermediate data.
- Run production from a clean documented environment. Verify expected files, parseability, finite values, invariants, tolerances, counts, and other internal consistency conditions.
- Visually inspect every rendered figure and compiled table/manuscript for labels, units, legends, accessibility, cropping, resolution, typography, significant figures, and caption agreement.
- Compare manuscript prose and equations against implementation and outputs. Resolve discrepancies in conventions, parameters, sample sizes, exclusions, uncertainty, normalization, filenames, plotted quantities, and reported numbers.
- Require review by a qualified person other than the primary producer for central/high-risk artifacts. Record the review and unresolved concerns; prefer independent recomputation for central or surprising claims.

## Documentation, versioning, and archive

- Maintain a README or reproduction guide with scope, prerequisites, data access, environment setup, exact commands, expected outputs, runtime/resources, validation checks, and limitations.
- Include licensing and contributor/citation metadata (`CITATION.cff` when suitable), or explain restrictions.
- Use meaningful commits and review publication-critical changes. Tag exact submitted and accepted states; do not rewrite released history.
- Create one GitHub repository for each published paper. It must contain, or unambiguously retrieve, the data and scripts needed to reproduce every published computational figure and, where applicable, final computational tables and numerical claims.
- Map every published figure to its production driver, required inputs, machine-readable source data, expected output, and exact reproduction command.
- Tag the exact paper release, archive that GitHub release with Zenodo, obtain a version-specific DOI, and cite it in the paper. Include permitted data, source-data tables, environment metadata, and documentation; add the paper DOI to the repository/deposit metadata after publication.
- Inspect or retrieve the Zenodo deposit and test reproduction from the archived release. GitHub is the working record; the Zenodo release is the preservation record.
- If an input cannot be deposited for legal or ethical reasons, include all distributable scripts plus a persistent data identifier or precise access procedure, permitted checksums, a description of the restriction, and a test or synthetic dataset sufficient to exercise the workflow. Record an approved exception; never silently omit required inputs.

## AI tools and potential intellectual property

Treat submission to a hosted AI service as external disclosure and processing. Ownership language in a provider’s terms does not by itself preserve patentability, prove human inventorship/authorship, guarantee confidentiality, ensure output uniqueness, or clear third-party rights.

This area is legally and professionally unsettled. Apply a precautionary standard to frontier, commercially valuable, highly competitive, or research-priority-sensitive work; lack of proven misuse or model-training use does not eliminate disclosure, priority, trade-secret, contractual, credit, or evidentiary risk.

- Before sending unpublished inventions, enabling technical details, confidential code, embargoed results, grant concepts, or proprietary data to an AI tool, classify the material and check institutional, sponsor, NDA, export-control, ethics, and data-use restrictions.
- Use potentially valuable or confidential material only with institutionally approved services, organizational accounts, models/features, and data controls approved for that classification. Do not use a personal/free account as a substitute. Distinguish “not used for training” from retention, logging, application state, human access, and third-party processing.
- Disable every setting that permits an AI provider to use research chats, files, prompts, or outputs for model training or improvement. Do not opt into voluntary feedback, evaluation, or data sharing with research content. For managed/API accounts, require an administrator to verify and periodically audit organization- and project-level settings rather than relying only on defaults.
- Minimize and redact inputs; prefer synthetic or abstracted data. Do not submit full invention disclosures, patent claims, credentials, restricted data, or third-party confidential material without specific authorization.
- Check the full data path. Connectors, plug-ins, remote tools, browsing, file stores, feedback, caches, and subprocessors may have separate retention and use terms. Disable unneeded integrations.
- Before high-risk use, consult the project lead and the institution’s technology-transfer, research-security, privacy, or legal office. Obtain advice about filing an invention disclosure before external disclosure.
- Treat unpublished enabling ideas, proof strategies, negative results, research road maps, and detailed notes for competitive or landmark problems as confidential. Until publication or clearance, prefer approved local/offline models or use only compartmentalized, non-enabling prompts with hosted systems.
- For validated/publication work, record the service/account class, model/version when available, date, purpose, disclosed data categories, relevant controls, and human verification. Keep sensitive prompts/outputs in approved restricted storage or record a non-sensitive audit reference; do not commit them reflexively.
- Treat AI output as untrusted assistance. Humans must verify science, citations, code, originality, licensing, and compliance and assess possible third-party IP. Preserve dated human design notes, commits, and decisions supporting conception and substantive contribution.
- For high-risk use, retain an access-controlled snapshot of applicable terms, data-control documentation, institutional approval, and account settings so the governing conditions can be reconstructed later.
- Do not designate an AI system as an author or inventor. Escalate authorship/inventorship questions under applicable institutional, journal, funder, and legal rules.
- If protected material reaches an unapproved system, stop further disclosure and promptly follow institutional security/privacy and technology-transfer incident procedures.

Maintain an approved-AI-use matrix covering services/account types, permitted data classes, training/retention settings, enabled external tools, owner, and review date. Designate who verifies that training/improvement sharing remains disabled. Review it at least annually, after material provider-policy changes, and before new high-risk uses. Treat this block as risk management, not a legal conclusion; institutional legal and technology-transfer advice controls.

## Naming and separation

Keep immutable/raw inputs, derived data, reusable source, notebooks, production drivers, tests, machine-readable results, manuscript files, and rendered artifacts distinguishable. Prefer stable manuscript-aligned names (`figure_2`, `table_1`) over ambiguous names (`final2`, `new`). Never hand-edit generated artifacts.

## Exceptions

When a requirement is impossible, unethical, legally barred, scientifically inappropriate, or grossly disproportionate, document before release:

1. the unmet requirement and reason;
2. the verification/reuse risk;
3. compensating evidence or controls;
4. the approving project lead and date.

Make material exceptions visible in the reproduction guide and manuscript availability/limitations statement. Do not use exceptions to avoid ordinary cleanup.

## Completion gate

Before calling publication-level work complete:

- inventory all final computational artifacts and numerical claims;
- confirm each artifact has an owner, driver, source data, provenance, and reviewer;
- regenerate through documented commands in a clean environment;
- complete numerical, visual, and manuscript/code consistency checks;
- record approved exceptions and review sign-off;
- review AI-use records and resolve confidentiality, patentability, inventorship/authorship, third-party-rights, and acknowledgment issues before release;
- confirm the paper has its own GitHub repository and every computational figure maps to its scripts and included or precisely retrievable data;
- tag the exact release, archive it with Zenodo, obtain/cite the version-specific DOI, and verify the archived package and metadata.
