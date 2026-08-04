# Visage Imaging (visage-imaging)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Visage Imaging is a global enterprise imaging vendor and a wholly-owned subsidiary of Pro Medicus Limited (ASX: PME). Its flagship Visage 7 Enterprise Imaging Platform delivers server-side rendered images adaptively streamed to an intelligent zero-footprint thin-client viewer for diagnostic radiology, cardiology, and mobile reading, alongside Visage 7 Open Archive and the Visage AI Accelerator research platform. Interoperability is built on healthcare imaging standards (DICOM / DICOMweb, HL7, FHIR, and IHE profiles), and Visage exposes REST and open-API surfaces for AI algorithm integration and QA workflows.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/visage-imaging/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/visage-imaging/refs/heads/main/apis.yml)

## Access Model (important)

Visage Imaging does **not** operate a public, self-service developer portal. There is no openly published API reference, OpenAPI description, or free API key signup. API and integration material lives behind gated channels:

- **Client Portal** and **Product Documentation** require a customer login.
- The **Visage AI Accelerator Program** (the open-API / AI research server surface) is described as **by invitation only**.
- Release notes that mention the newer REST API (a QA "delete and resend" workflow) are distributed to customers, not published as a public reference.

Because of this, the API entries in `apis.yml` are **logically modeled** from public product pages, press releases, and release-note summaries rather than transcribed from an official API reference. Individual endpoints, authentication, and base URLs are deployment-specific and are marked `endpointsModeled` in each API's description. This entry is an honest, gated stub - not a claim that these are open, self-serve APIs.

## Standards

Visage 7 is an archive-neutral enterprise imaging platform whose interoperability is grounded in healthcare imaging standards:

- **DICOM / DICOMweb** - QIDO-RS (query), WADO-RS / WADO-URI (retrieve), STOW-RS (store).
- **HL7 v2** messaging and **FHIR** resources (e.g. ImagingStudy, DiagnosticReport) for order/result and imaging-context exchange with the EHR and RIS.
- **IHE** enterprise-imaging profiles for cross-system workflow.
- **Open AI API** with FHIR, Python, NIfTI, webforms, 2D/3D segmentations, semantic annotations, radiomics, bulk de-identification, and ground-truth labeling for the AI Accelerator research server.

## Ownership

Visage 7 was "developed exclusively by Pro Medicus' wholly-owned subsidiary, Visage Imaging," on a single code base. Visage Imaging is the enterprise-imaging arm of **Pro Medicus** ([promedicus.com](https://www.promedicus.com/)).

## Tags

- Enterprise Imaging
- Medical Imaging
- Radiology
- PACS
- DICOM
- DICOMweb
- HL7
- FHIR
- Healthcare
- AI
- Pro Medicus

## Timestamps

- **Created:** 2026-07-05
- **Modified:** 2026-07-05

## APIs (modeled)

### Visage 7 AI Open API

Open API for integrating third-party and customer AI algorithms into Visage 7 and the Visage AI Accelerator research server (FHIR, Python, NIfTI, segmentations, semantic annotations, radiomics, de-identification). Invitation-only; endpoints modeled.

- **Human URL:** [https://visageimaging.com/platform/acceleratedai/](https://visageimaging.com/platform/acceleratedai/)

### Visage 7 QA REST API

REST API (from Visage 7 release notes) for a QA workflow based on delete-and-resend of studies between Visage 7 and connected archives/modalities. Gated; endpoints modeled.

- **Human URL:** [https://visageimaging.com/visage-7/](https://visageimaging.com/visage-7/)

### Visage 7 DICOMweb API

Standards-based DICOMweb interface - QIDO-RS, WADO-RS / WADO-URI, STOW-RS - against the archive-neutral Visage 7 platform. Per-deployment base URL; endpoints modeled.

- **Human URL:** [https://visageimaging.com/visage-7/](https://visageimaging.com/visage-7/)

### Visage 7 HL7 / FHIR Interoperability API

HL7 v2 messaging and FHIR resources for order/result and imaging-context exchange with the EHR and RIS. Deployment-specific; endpoints modeled.

- **Human URL:** [https://visageimaging.com/platform/acceleratedai/](https://visageimaging.com/platform/acceleratedai/)

### Visage 7 Viewer Launch API

Context / URL launch interface to open the Visage 7 thin-client viewer to a specific patient, study, or accession from an EHR, RIS, or portal (SSO + deep-link parameters). Deployment-specific; endpoints modeled.

- **Human URL:** [https://visageimaging.com/visage-7/](https://visageimaging.com/visage-7/)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/visage-imaging)
- [Website](https://visageimaging.com/)
- [Documentation](https://visageimaging.com/support/product-documentation/) (login required)
- [Client Portal](http://www2013.visageimaging.com/support/client-portal/) (login required)
- [Parent Company - Pro Medicus](https://www.promedicus.com/)

## Pricing

No public pricing. Visage 7 is sold as an enterprise contract (PACS-replacement / enterprise imaging) via direct sales; the AI Accelerator Program is invitation-only. Pricing is contact-sales only.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
