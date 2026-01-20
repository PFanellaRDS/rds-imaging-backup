# Copilot Instructions for rds-imaging-backup

## Project Overview
**rds-imaging-backup** is a comprehensive ground-up initiative by **Retail Data Systems (RDS)** to establish reliable imaging and backup systems for Office, Grocery, and Hospitality environments. Built on **FOG (Free Open-source Ghost)** for network imaging, this project designs core infrastructure, automation workflows, and operational procedures from scratch. The project is deadline-driven (June 30, 2026) and organized around 4 major epics with 25+ child issues spanning infrastructure, automation, documentation, and knowledge transfer.

## Architecture & Major Components

### 1. Four Strategic Epics (Reference: ROADMAP.md)
- **EPIC #1 — Office Imaging & Deployment**: Rapid OS restoration for office systems; eliminates KVM-based manual restoration
- **EPIC #2 — Image Storage Infrastructure**: Local NAS in Lisle and Portage + cloud sync for Grocery images
- **EPIC #3 — KVM Device Standardization**: Standardized HP KVM device images on SD cards with centralized repository
- **EPIC #4 — Documentation & Knowledge Transfer**: SOPs, runbooks, and troubleshooting guides for operational handoff

### 2. Critical Integration Points
- **Hardware Assets**: Three regional locations (Lisle, Portage, Office/Grocery/Hospitality) with distinct storage models
- **Imaging Workflow**: Office → Deployment automation; KVM → SD card provisioning; Grocery → Cloud sync
- **Documentation Dependency**: All epics feed into Phase 8 (Weeks 18-24) for comprehensive runbooks

## Key Workflows & Commands

### Tracking Issue Progress & Documentation
- **Master reference**: `ROADMAP.md` contains full chronological execution order (Phases 1-8) and all issue dependencies
- Each issue is dependency-mapped; verify Phase prerequisites before starting work
- Example: Infrastructure deployment (Phase 3, Issues #8, #6, #22) must complete before Image Development (Phase 4)
- **Primary documentation hub**: `rds-project-vault/` (Obsidian vault) — all notes, design documents, assessments, and project tracking live here
- Network assessment work is housed in `rds-project-vault/Network Assesment/` (note: intentional spelling)

### Documentation Standards
- All procedures must be documented before sign-off (see Phase 8 requirements)
- Runbooks and SOPs are tracked and authored in the Obsidian vault
- Runbooks are critical for operational handoff post-June 2026
- Ground-up design means establishing new procedures; reference competitive review (PfanellaCompReview.pdf) for context

## PCompany**: Retail Data Systems (RDS) — imaging system spans 3 regional locations
- **Locations**: Lisle (ON-site NAS), Portage (ON-site NAS), Office/Grocery/Hospitality (imaging targets)
- **Imaging Platform**: FOG (Free Open-source Ghost) — network-based OS imaging and deployment

### Naming & Organization
- **Locations**: Lisle (ON-site NAS), Portage (ON-site NAS), Office/Grocery/Hospitality (imaging targets)
- **Hardware**: HP-based KVM devices (standardized images), NAS systems (local storage)
- **Cloud Service**: Cloud sync for Grocery images (separate from local NAS)

### Verification Checklist (Project Completion)
Before declaring work complete, verify:
- [ ] All infrastructure deployed and tested (Lisle & Portage NAS)
- [ ] Office imaging solution implemented with base image
- [ ] KVM images created, SD cards provisioned, validated
- [ ] Cloud sync configured and validated for Grocery
- [ ] Validation reports completed
- [ ] All SOPs/runbooks written and reviewed
- [ ] Training sign-offs obtained

## Key Files & References
- [ROADMAP.md](ROADMAP.md) — Master epic list, dependency order, and verification checklist
- [rds-project-vault/copilot/copilot-custom-prompts/](rds-project-vault/copilot/copilot-custom-prompts/) — Custom Copilot prompts (Emojify, Summarize, Translate, etc.)
- [PfanellaCompReview.pdf](PfanellaCompReview.pdf) — Competitive review/assessment document

## Guidance for AI Agents
 and Phase execution order
2. Verify Phase prerequisites are complete before proceeding
3. Reference the Verification Checklist for completion criteria
4. All work must include documentation plan (required for Phase 8)
5. Check Obsidian vault (`rds-project-vault/`) for existing design notes, assessments, and earlier decisions

### Common Task Patterns
- **Infrastructure Setup**: Reference Phase 3 issues (#8, #6, #22) for NAS and cloud sync patterns; log decisions/notes in Obsidian
- **Imaging Development**: Phases 4-5 establish FOG workflow patterns; reference Office/KVM approaches
- **Design & Assessment**: Network assessments, infrastructure requirements, and design specs go in `rds-project-vault/` with appropriate folder structure
- **Documentation**: Phase 8 requires SOPs, runbooks, and troubleshooting guides — author in Obsidian vault for Phase 8 compilation

### Cross-Epic Coordination
- Office Imaging (Epic #1) depends on Storage Infrastructure (Epic #2) completion
- KVM Standardization (Epic #3) enables Office Imaging alternatives  
- All epics feed into Documentation Phase (Epic #4) — block major documentation compilation until Phase 8
- Ground-up design approach means designs established in Phase 1-2 drive all downstream work
- KVM Standardization (Epic #3) enables Office Imaging alternatives
- All epics feed into Documentation Phase (Epic #4) — block documentation tasks until Phase 8
