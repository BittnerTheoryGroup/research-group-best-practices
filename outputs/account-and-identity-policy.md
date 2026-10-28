# Account and Identity Policy

## Purpose

This policy ensures that work produced in the Bittner Theory Group is associated with institutional identities, remains accessible after personnel transitions, and is governed by the University of Houston's agreements and data controls rather than individual personal terms of service.

## University accounts for work-related activities

All students, postdocs, and researchers in the group must use accounts associated with the **central.uh.edu** domain for work-related activities. This applies to:

- GitHub (see below)
- AI tools and coding assistants used for research (see the [Research Computing and Paper Production Policy](research-computing-policy.md))
- Cloud storage, compute platforms, and collaboration services used for group work
- Any service where the account identity governs data ownership, retention, or access controls

Personal accounts must not be used as a substitute for institutional accounts on services that process unpublished research, grant-related work, proprietary data, or code that may have intellectual-property implications.

## GitHub accounts

Day-to-day development under a personal GitHub account is fine. However, when a paper or project is ready for release — at or before manuscript submission — the repository must be published under the [BittnerTheoryGroup](https://github.com/BittnerTheoryGroup) organization so that it is discoverable, persistent, and not tied to any one individual's account.

Acceptable approaches at release time include:

- **Transfer the repository** to the BittnerTheoryGroup organization via GitHub's repository transfer feature (Settings → General → Transfer ownership).
- **Fork or re-push** to a new repository under the organization if transfer is not possible or not desired.

When moving the repository, preserve the full commit history. Update any external links, citations, or references (e.g., in manuscripts or Zenodo deposits) to point to the new canonical location under the organization.

## Repository visibility and public release

All repositories — whether on personal accounts or under the BittnerTheoryGroup organization — must remain **private** until public release is authorized (see below). Do not make a repository public without explicit approval from the group lead.

### Pre-publication

Research code, data, notebooks, and computational results must not be released publicly before the associated work has been disclosed through a peer-reviewed journal publication. Premature public release can:

- compromise patent rights and invention disclosure procedures under the University of Houston's intellectual property policy;
- establish prior art in ways that damage the group's or institution's ability to protect commercially valuable discoveries;
- breach funder, sponsor, data-use, or collaboration agreements that restrict disclosure timing.

When in doubt, treat unpublished work as confidential and consult the group lead before sharing outside the group.

### Public release at publication

When a manuscript is accepted or published, the corresponding repository may be made public and transferred to the BittnerTheoryGroup organization. The release workflow is:

1. Confirm with the group lead that public release is appropriate and that no IP holds, export controls, or data-use restrictions apply.
2. Review the repository for credentials, restricted data, or third-party-licensed material that must not be released; remove or redact before making the repository public.
3. Transfer or publish the repository under BittnerTheoryGroup with an appropriate open-source license (discuss with the group lead if uncertain).
4. Tag the release, archive with Zenodo, and obtain a DOI as described in the [Research Computing and Paper Production Policy](research-computing-policy.md).

### UH intellectual property policy

All research conducted at the University of Houston is subject to the UH Intellectual Property Policy. Research code, datasets, and computational methods developed using university resources or funding may constitute university intellectual property. Group members should familiarize themselves with the policy and contact the UH Office of Technology Transfer and Innovation ([tti.uh.edu](https://tti.uh.edu)) before publicly releasing any work that may have commercial value or patentable novelty. When in doubt, file an invention disclosure with TTI before public release.

## Rationale

Personal accounts are governed by individual terms of service and are not subject to the university's institutional agreements, data controls, or security reviews. Work hosted under personal accounts may become inaccessible when a group member departs, and ownership or continuity of the research record may be unclear. Using institutional accounts protects both the researcher and the group's long-term interests.

## Responsibility

- **Group members** are responsible for ensuring their work-related accounts are linked to their university identity and for migrating existing work promptly.
- **Group/project lead** is responsible for verifying that all active repositories are under the organization and that departing members' work has been transferred before offboarding is complete.

---

*Last reviewed: October 2026. Review annually or when institutional account policies change.*
