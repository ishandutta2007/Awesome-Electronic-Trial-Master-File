# Awesome-Electronic-Trial-Master-File

# Top Electronic Trial Master File (eTMF) Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Clinical Trial Document Management, Regulatory Compliance, Inspection Readiness & TMF Reference Model Alignment*  
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Electronic Trial Master File (eTMF)** management. These tools help sponsors, CROs, and clinical research sites organize, track, and maintain essential trial documents in compliance with ICH-GCP, FDA 21 CFR Part 11, and the TMF Reference Model.

**Examples** include Veeva Vault eTMF, Medidata eTMF, Phlexglobal, MasterControl eTMF, Ennov eTMF, TransPerfect Trial Interactive, DOCS eTMF, Florence eTMF, Montrium eTMF, and Box Clinical (the category leaders).

**Open-source emphasis**: This is one of the most commercially consolidated categories in clinical research software. **No mature, production-ready open-source eTMF platform exists.** The practical open-source path is **configuring a general-purpose Document Management System (DMS)** — such as **OpenKM** — to implement the TMF Reference Model taxonomy, or using emerging **AI-powered quality management platforms** like **QAtrial** that include eTMF documentation modules. This section documents these foundations honestly.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Veeva Vault eTMF](https://www.veeva.com/)**  
  The market-leading cloud eTMF platform. Deep integration with Veeva Vault CTMS, Study Startup, and SiteVault. Provides automated document filing, completeness tracking, inspection readiness dashboards, and full 21 CFR Part 11 compliance. Enterprise-focused with significant implementation and licensing costs.

- **[Medidata eTMF](https://www.medidata.com/)**  
  eTMF module within the Medidata Clinical Cloud. Integrates with Medidata Rave EDC and other clinical systems. Provides document management, TMF completeness metrics, and inspection support.

- **[Phlexglobal](https://www.phlexglobal.com/)**  
  Specialist TMF services and technology provider. Offers PhlexTMF (eTMF platform) alongside TMF consulting, migration, and managed services. Deep expertise in TMF Reference Model implementation and inspection readiness.

- **[MasterControl eTMF](https://www.mastercontrol.com/)**  
  eTMF solution within MasterControl's quality and compliance platform. Integrates with MasterControl's QMS, training, and document control modules for unified GxP compliance.

- **[Ennov eTMF](https://www.ennov.com/)**  
  eTMF module within Ennov's regulatory and quality suite. Provides document management, workflow, and compliance tracking for clinical trials.

- **[TransPerfect Trial Interactive](https://www.transperfect.com/)**  
  eTMF platform with integrated translation and linguistic validation services. Provides document management, TMF completeness tracking, and global regulatory support.

- **[DOCS eTMF](https://www.docs.com/)**  
  Purpose-built eTMF platform from DOCS (formerly TrialWorks). Provides document filing, TMF completeness, and inspection readiness for sponsors and CROs.

- **[Florence eTMF](https://florencehc.com/)**  
  eTMF solution focused on site-level and sponsor-level document management. Provides eISF (electronic Investigator Site File) and eTMF capabilities with a focus on usability.

- **[Montrium eTMF](https://www.montrium.com/)**  
  eTMF platform built on Microsoft SharePoint. Provides TMF Reference Model alignment, document management, and inspection readiness. Popular for organizations already invested in Microsoft 365.

- **[Box Clinical](https://www.box.com/)**  
  General-purpose content management platform configured for clinical trial document management. Provides eTMF capabilities through Box's compliance, workflow, and security features.

## Open-Source GitHub Projects

- **[OpenKM](https://github.com/openkm/document-management-system)**  
  **The most viable open-source foundation for building an eTMF.** OpenKM is an open-source Document Management System (DMS) that can be configured to implement the TMF Reference Model taxonomy. Features document metadata customization for trial-specific classification, electronic workflows for consent form review/approval, complete API for integration with CTMS systems, audit trail and version control, and support for regulatory compliance (Spanish AEMPS and equivalent agencies). Clinical research teams can use OpenKM to build a customized eTMF with structured folders, metadata, and access controls. **Open source (GPL)**. ~1.8k stars .

- **[QAtrial](https://github.com/MeyerThorsten/QAtrial)**  
  Open-source AI-powered quality management platform for regulated industries. Includes **eTMF documentation management** as a core module alongside eConsent, batch records, design control, CAPA, and deviations. Features 45+ database models, 100+ API endpoints, 18 country templates, 12 languages, and 10 GxP industry verticals. **Runs in standalone mode** (browser-only, localStorage) for demos or **server mode** (PostgreSQL-backed, multi-user, API-driven) for enterprise use. Deploys via Docker or Helm chart for Kubernetes. **AGPL-3.0** .

- **[clinicedc](https://github.com/clinicedc)**  
  Django-based clinical trial data management framework from the Botswana-Harvard AIDS Institute Partnership. Provides a collection of Python modules for building EDC/eSource systems, including document archiving capabilities. The `edc-document-archive` module provides an EDC mobile app for document archiving . While primarily an EDC framework, its document management modules can be extended for eTMF-adjacent workflows. **GPL-3.0**.

- **[TMF Reference Model Exchange Framework](https://github.com/TmfRef/exchange-framework/)**  
  The TMF Reference Model EMS (Exchange Mechanism Standard) provides a machine-readable format for exchanging eTMF information between systems and organizations. This GitHub repository contains the open-source implementation of the EMS specification, enabling interoperability between different eTMF systems. The standard was developed under the TMF Reference Model initiative and migrated to CDISC governance .

### Additional Strong Open-Source Options

- **General-Purpose DMS**: **OpenKM** (most viable eTMF foundation, GPL), **Alfresco Community** (enterprise DMS with workflow), **Nuxeo** (content management platform).
- **Clinical Data Management**: **clinicedc** (Django-based, document archiving modules), **OpenClinica** (EDC platform, community edition available) .
- **Regulatory Documentation**: **innolitics/rdm** (regulatory documentation manager for 62304, 14971, 510(k) — medical device focus, 142 stars) .
- **Government/Legal Document Management**: **PolicyWiki** (MediaWiki-based for policy documents, configurable hierarchies) .

**Frameworks for building custom systems**: Combine **OpenKM** for the core document management engine, **TMF Reference Model Exchange Framework** for standardized metadata and interoperability, **QAtrial** for AI-powered quality management and eTMF modules, and **PostgreSQL** for persistence. Add **CTMS integration** via OpenKM's API and **Docker** for deployment. Note that significant custom development is required to achieve a production-ready eTMF compliant with ICH-GCP and 21 CFR Part 11.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- eTMF systems handle regulated clinical trial documentation; ensure compliance with ICH-GCP, FDA 21 CFR Part 11, EU CTR, and applicable regional regulations.
- **Open-source reality**: **No production-ready open-source eTMF platform exists.** The practical path is configuring **OpenKM** (or a similar DMS) with the TMF Reference Model taxonomy, or using emerging platforms like **QAtrial** that include eTMF modules. Both require significant validation, configuration, and compliance work before use in regulated trials. For organizations requiring immediate regulatory compliance, commercial platforms (Veeva, Medidata, Phlexglobal) remain the dominant choice .
