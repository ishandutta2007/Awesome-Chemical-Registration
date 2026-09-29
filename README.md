# Awesome-Chemical-Registration

## Top Chemical Registration Platforms Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Compound Registration, Structure Standardization, Inventory Management & Chemical Intelligence*  

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Chemical Registration**. These tools help research labs, biotech companies, and pharmaceutical organizations register chemical compounds, standardize structures, manage inventory, and integrate chemical data with bioassay results.



**Examples** include ChemAxon Instant JChem, BIOVIA CISPro, Dotmatics Studies, ChemInventory, LabCollector, CDD Vault, Scilligence ELN, Signals Notebook, Scispot, and eLabNext (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom registration logic, and transparent chemical data — ideal for labs and startups that need full control over their compound libraries without per-seat SaaS fees or vendor lock-in.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents



- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[ChemAxon Instant JChem](https://chemaxon.com/)**  

  Desktop and web-based chemical database management with structure search, property calculation, and registration capabilities.



- **[BIOVIA CISPro](https://www.3ds.com/)**  

  Chemical inventory and safety management system for tracking reagents, samples, and hazardous materials across multiple locations.



- **[Dotmatics Studies](https://www.dotmatics.com/)**  

  Electronic lab notebook and data management platform for chemistry and biology research with compound registration.



- **[ChemInventory](https://www.cheminventory.net/)**  

  Cloud-based chemical inventory management for labs. Tracks reagents, locations, and safety data.



- **[LabCollector](https://labcollector.com/)**  

  LIMS and lab management platform with chemical inventory and sample tracking modules.



- **[CDD Vault](https://www.collaborativedrug.com/)**  

  Collaborative drug discovery platform with chemical registration, assay data management, and ELN capabilities.



- **[Scilligence ELN](https://www.scilligence.com/)**  

  Electronic lab notebook with chemical structure handling and registration.



- **[Signals Notebook](https://www.dotmatics.com/)**  

  Dotmatics' ELN with chemical registration and structure search.



- **[Scispot](https://www.scispot.com/)**  

  Digital lab platform with ELN, LIMS, and chemical inventory capabilities.



- **[eLabNext](https://www.elabnext.com/)**  

  Digital lab platform combining ELN, LIMS, and inventory management with chemical registration.



## Open-Source GitHub Projects



### Compound Registration & Management



- **[MolTrack](https://github.com/datagrok-ai/mol-track)**  

  **The most complete open-source chemical compound registration system.** Lightweight, flexible, and extendable FastAPI server for managing chemical compounds, batches, and properties, powered by **RDKit-enabled PostgreSQL**. **MIT License**. Features compound registration with unique identifiers, duplicate detection, structure validation and standardization (tautomerization, salts, stereo conventions), custom metadata attributes, batch/lot management with purity and inventory tracking, protocol and assay result registration, structure-based search (exact, substructure, similarity, Markush), audit trails, role-based access control, and RESTful API for integration with ELN/LIMS. Integrates with chemical drawing tools (MarvinJS, ChemDraw, Ketcher). Docker setup scripts for Windows/macOS/Linux .



- **[lwreg](https://github.com/rinikerlab/lightweight-registration)**  

  **Lightweight chemical registration system created by Greg Landrum (RDKit founder).** Open-source, pure Python with minimal dependencies (RDKit only). Designed for **computational workflows** with simple Python API and CLI — no GUI. Captures both **2D structures and 3D conformers**. Supports configurable chemical identity definitions (tautomers, stereochemistry, counter-ions) via customizable standardization and filtering pipelines. Uses RDKit RegistrationHash with layered hashing for duplicate detection. Includes schema for storing experimental data and metadata linked to registered structures. **MIT License** (ETH Zurich) .



- **[OpencanSARchem](https://github.com/)**  

  **Open-source chemical registration and standardization pipeline for FAIR integration of bioassay data.** Published in *Journal of Cheminformatics* (2026). Replaces the commercial canSARchem pipeline with an open-source, computationally efficient alternative. Achieves **100-fold reduction in computational time** compared to original. Carefully assesses tautomeric representations using Gibbs free energy calculations. Deployed within canSAR.ai, unifying disparate biochemical data sources for the drug discovery community .



### Electronic Lab Notebooks with Chemical Registration



- **[eLabFTW](https://github.com/elabftw/elabftw)**  

  **The most popular open-source electronic lab notebook for research labs.** Free, modern, versatile, and secure. **AGPL-3.0**. Features include experiment notes, **resources database for lab reagents and chemical products**, equipment scheduling, **chemical structure editor (Ketcher)**, DNA cloning (OpenCloning), and a **Compounds database** where all teams and users can register and view entries. Trusted timestamping (RFC 3161), audit logs, and advanced permissions. Available in 21 languages. Deployed at research institutions worldwide including Kyoto University .



- **[Chemotion ELN](https://github.com/ComPlat/chemotion_ELN)**  

  **Open-source electronic lab notebook specifically designed for chemistry research.** Developed at Karlsruhe Institute of Technology (KIT). Features structure drawing, reaction planning, and chemistry-aware data management. **Chemotion Repository** is a public collection of synthetic compounds with analytical data (NMR, MS, IR, UV, crystal structures), automatically citable via DOI and available on PubChem. Samples are assigned to molecules with InChI and SMILES identifiers generated via OpenBabel. PubChem API integration for CAS registry number lookup .



- **[Phoenix ELN](https://github.com/abrechts/Phoenix-ELN)**  

  **Open-source electronic lab notebook for organic, organometallic, peptide, resin and polymer chemistry.** Windows platform. Features integrated chemical reaction drawing editor, stoichiometric calculations, self-learning materials database (~200 common reagents/solvents), reaction substructure searches (RSS) and full-text search. Auto-generates "Same Step" experiment lists and synthetic connection graphs. Optional ELN Server Package for MySQL/MariaDB synchronization across teams .



- **[OrChem](https://orchem.sourceforge.net/)**  

  **Open-source chemistry extension for Oracle Database** adding registration and indexing of chemical structures. Supports fast substructure and similarity searching for databases with millions of compounds. Uses Chemistry Development Kit (CDK). **LGPL License**. Powers substructure search in ChEBI database. Provides similarity searching with response times in seconds for millions of compounds .



### Inventory Management



- **[Organilab](https://github.com/Solvosoft/organilab)**  

  Open-source virtual tool for **inventory management of chemical substances**. Designed for compliance with **ISO-17025 and GHS**. Open Collective supported .



- **[LIME](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0336412)**  

  **Free, open-source laboratory inventory management software** using barcode/QR scanning via mobile app. Combines Scan-IT to Office app with Google Sheets/Excel templates. Features real-time alerts, dynamic inventory updates, custom fields, and offline capability. Survey of deployed labs: 87.5% found it moderately easy to set up, 75% described it as extremely/very accurate, and 75% will continue using it. Reduces tracking time and improves accuracy .



- **[ChemSearch](https://github.com/ruzx/ChemSearch)**  

  **Chemical substructure search and inventory management toolkit for Obsidian.** Vault-wide substructure search using Ketcher drawings. Chemical Inventory Manager tracks physical containers with safety data linking (PubChem CIDs, LCSS), smart auto-complete, and structured YAML metadata. Offline calculations for exact mass, elemental analysis, and experimental boilerplate. **MIT License** .



- **[ChemTrack](https://github.com/Yashraj221B/chemical-management-frontend)**  

  Modern web application for **laboratory chemical inventory management**. React 19 + TypeScript + Tailwind CSS. Features search/filter by name/formula/bottle number, detailed chemical information with PubChem integration, visual formula display, location tracking, admin dashboard, and role-based access control .



### Additional Strong Open-Source Options



- **Compound Registration**: **MolTrack** (most complete, FastAPI + RDKit + PostgreSQL), **lwreg** (lightweight, Python API, 2D/3D support), **OpencanSARchem** (FAIR bioassay integration) .

- **Chemistry ELN**: **eLabFTW** (most popular, compounds database, Ketcher), **Chemotion ELN** (KIT, repository integration), **Phoenix ELN** (organic synthesis focused) .

- **Chemical Search**: **OrChem** (Oracle extension, CDK-based, ChEBI-powered) .

- **Inventory Management**: **Organilab** (ISO-17025/GHS), **LIME** (barcode/QR scanning), **ChemSearch** (Obsidian plugin), **ChemTrack** (React web app) .



**Frameworks for building custom systems**: Combine **MolTrack** for complete compound registration with structure search, **lwreg** for lightweight computational workflows, **eLabFTW** or **Chemotion ELN** for chemistry-focused experiment documentation, and **LIME** or **ChemSearch** for inventory management. Add **PostgreSQL with RDKit cartridge** for chemical intelligence and **Docker** for deployment.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Chemical registration platforms handle sensitive research data and hazardous material information; ensure compliance with institutional safety policies and relevant regulations (GHS, ISO-17025).

- **Open-source reality**: The open-source ecosystem for chemical registration is **mature and production-ready**. **MolTrack** provides comprehensive compound registration with RDKit-enabled PostgreSQL . **lwreg**, created by RDKit's founder, offers a lightweight, computationally-focused registration system . **eLabFTW** is the most popular open-source ELN with built-in compound database . **OpencanSARchem** provides FAIR-compliant standardization for bioassay data . For enterprise-scale commercial deployment with dedicated support and advanced cheminformatics features, commercial platforms (ChemAxon, BIOVIA, Dotmatics) remain the primary choice for large pharmaceutical organizations.



---



**Made for medicinal chemists, lab managers, cheminformatics engineers, and research IT teams.**

Let's make chemical registration more open, transparent, and FAIR.
