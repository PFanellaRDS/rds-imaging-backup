# Issue #19 Preparation Checklist

**Issue**: Assess Storage Infrastructure Requirements
**Phase**: Phase 1 — Planning & Assessment (Weeks 1–2)
**Epic**: EPIC #2 — Image Storage and Backup Infrastructure
**Status**: 🟡 In Preparation

---

## Assessment Scope

This assessment defines storage infrastructure requirements for:

- **Lisle NAS**: Local on-site storage for Lisle imaging operations
- **Portage NAS**: Local on-site storage for Portage imaging operations
- **Grocery Cloud Sync**: Off-site/cloud backup for Grocery environment images

---

## Pre-Assessment Tasks

### Current Infrastructure Discovery

- [ ] **KVM Devices**: What HP KVM devices are currently in use? Models, locations, quantity?
- [ ] **KVM Purpose**: How are KVM devices currently used in RDS operations?
- [ ] **KVM Issues**: What pain points exist with current KVM setup that we're solving?
- [ ] **Current Imaging**: How are systems currently restored/redeployed without FOG?
- [ ] **Network Layout**: Document network topology at each location (Lisle, Portage, Office/Grocery/Hospitality)

### General Discovery

- [ ] Review [[Project Info]] for budget, timeline, and regional locations
- [ ] Read `PfanellaCompReview.pdf` for competitive context
- [ ] Document current RDS imaging patterns (frequency, volume per location)
- [ ] Current Infrastructure & KVM Understanding
- [ ] What HP KVM models/types do we have? (switches, KVM-over-IP like iLO/iLO4, etc.)
- [ ] Which locations have KVM devices? (Lisle, Portage, Office, Grocery, Hospitality?)
- [ ] How many servers/systems does each KVM manage?
- [ ] What is the current manual restoration process using KVM?
- [ ] How long does a typical system restoration take today?
- [ ] What are the failure points/pain points in current KVM-based approach?
- [ ] Will KVM devices remain in use for remote access, or be completely replaced?
- [ ] What is the relationship between KVM devices and the SD card standardization (EPIC #3)?

### C Understand FOG network imaging requirements (throughput, latency, bandwidth)

- [ ] Define imaging scope: OS images only, or application stack?
- [ ] Identify compliance/data residency constraints

---

## Key Questions to Answer

### Capacity & Performance

- [ ] What is estimated imaging storage capacity per location (Lisle, Portage)?
- [ ] What is the expected imaging frequency per location?
- [ ] What are FOG network throughput requirements?
- [ ] What latency/response time is acceptable for deployments?

### Cloud Sync Strategy (Grocery)

- [ ] Should Grocery images be stored locally first, then synced to cloud?
- [ ] Or direct cloud-primary approach?
- [ ] What is expected bandwidth consumption?
- [ ] Recovery time objective (RTO) for Grocery images?
- [ ] Recovery point objective (RPO) acceptable?

### Redundancy & Reliability

- [ ] Single NAS per location, or redundant setup?
- [ ] Backup strategy for NAS systems (local snapshots, off-site backup)?
- [ ] Acceptable downtime for imaging operations?
- [ ] RAID configuration recommendations?

### Hardware Constraints

- [ ] Physical space available for NAS at each location?
- [ ] Power/cooling infrastructure available?
- [ ] Network infrastructure capable of FOG imaging traffic?
- [ ] Budget: $5,000 total hardware + $80/month cloud

---

## Deliverables

### Primary Deliverables

- [ ] Storage Requirements Matrix
  - Capacity (TB) by location
  - Throughput requirements (Gbps)
  - Redundancy approach
  - Backup strategy

- [ ] Cloud Sync Strategy Recommendation
  - Approach (hybrid, cloud-primary, etc.)
  - Estimated monthly costs
  - RTO/RPO alignment
  - Failover procedures

- [ ] Hardware Recommendations
  - NAS models/sizing (Lisle & Portage)
  - Storage configuration (RAID, snapshots)
  - Network considerations
  - Cost breakdown

### Secondary Deliverables

- [ ] Risk Assessment
  - Single points of failure
  - Mitigation strategies
  - Disaster recovery approach

- [ ] Cost-Benefit Analysis
  - Total hardware cost vs. $5,000 budget
  - Monthly cloud cost vs. $80/month budget
  - Justification for any overages

---

## Research & References

- **FOG Documentation**: Official FOG imaging requirements
- **RDS Imaging History**: Current patterns, volume, frequency
- **PfanellaCompReview.pdf**: Competitive approaches
- **Industry Standards**: NAS sizing for imaging workloads

---

## Next Steps

1. ✅ Create this preparation checklist
2. 🔄 Gather RDS imaging volume data
3. 🔄 Research FOG performance requirements
4. 🔄 Draft storage requirements matrix
5. 🔄 Complete assessment document
6. 🔄 Present findings to stakeholders
7. ⏳ Feed results into Issue #5 (Procure Lisle) & Issue #11 (Procure Portage)

---

**Last Updated**: 2026-01-16
**Next Review**: Upon completion of data gathering phase
