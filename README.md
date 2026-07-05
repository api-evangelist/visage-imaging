# Visage Imaging (visage-imaging)

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
