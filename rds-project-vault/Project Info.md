# RDS Backup & Imaging Initiative

## Project Overview

**Organization**: Retail Data Systems (RDS)  
**Project Goal**: Establish reliable, repeatable, and documented imaging and recovery system for Office, Grocery, and Hospitality environments  
**Start Date**: January 2026  
**Deadline**: June 30, 2026  
**Status**: Phase 1 — Planning & Assessment (Weeks 1–2)

## Budget & Resources

- Local NAS hardware: $5,000
- Cloud sync: $80/month (ongoing)
- Local hardware: $1,500
- **Total Initial Investment**: $6,500

## Regional Locations

| Location | Purpose | Storage Model |
|----------|---------|---|
| **Lisle** | Regional hub | ON-site NAS |
| **Portage** | Regional hub | ON-site NAS |
| **Office/Grocery/Hospitality** | Imaging targets | Local deployment + cloud sync (Grocery) |

## Core Technology Stack

- **Imaging Platform**: FOG (Free Open-source Ghost) — network-based OS imaging and deployment
- **Hardware**: HP-based KVM devices (standardized images), NAS systems (local storage)
- **Cloud Service**: Cloud sync for Grocery images (separate from local NAS)

## Key Metrics

- **ROI Target**: Eliminate manual KVM-based restoration (save time/labor)
- **Availability Target**: 99%+ uptime for imaging systems
- **Recovery Target**: RTO/RPO to be defined in Issue #19 assessment
- **Documentation**: 100% of procedures documented by Phase 8

## Strategic Epics (4 Major Initiatives)

1. **EPIC #1** — Office Imaging & Deployment (eliminate KVM dependency)
2. **EPIC #2** — Image Storage Infrastructure (NAS + cloud sync)
3. **EPIC #3** — KVM Device Standardization (HP KVM → SD cards)
4. **EPIC #4** — Documentation & Knowledge Transfer (SOPs, runbooks)

## Key Documents

- [[ROADMAP]] — Master execution plan (Phases 1-8, all issues & dependencies)
- [[PfanellaCompReview]] — Competitive review & context
- [[Network Assessment/preparation-checklist]] — Issue #19 preparation

## Project Assumptions

- Ground-up design approach (not migrating existing systems)
- FOG expertise available or to be learned
- Budget constraints are firm
- June 30 deadline is fixed
- All procedures must be documented for operational handoff

## Links & References

- Current Phase: [[Phase 1 - Planning & Assessment]]
- Active Issues: [[Issue #19 - Storage Assessment]]
