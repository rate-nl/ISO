# Remote Work Transition Plan – August 2025

## 1. Purpose and Scope
This document outlines Rate's plan to transition from an office-based working model to a fully remote model starting **September 1, 2025**. It ensures business continuity, secure relocation of infrastructure, and compliance with the Information Security Management System (ISMS) based on ISO/IEC 27001:2022.

The plan specifically addresses the controlled relocation of:
- Development Server (incl. VPN endpoint)
- NAS backup device

It also outlines necessary ISMS updates to reflect the new operating model.

---

## 2. Transition Timeline

### **Current (Before September 1)**
- Office remains active
- All ISMS controls as documented (physical access, asset location, etc.) are in place
- Audit scheduled for August 27–28, 2025

### **During the Move (Late August)**
| Task | Responsible | Notes |
|------|-------------|-------|
| Physically disconnect NAS and Dev Server | Team Lead Developer | Confirm offsite transportation readiness |
| Transport devices to secure home office | CEO / Owner | Use vehicle directly (no courier); log transport time |
| Reconnect to home power and internet | CEO | Validate power, cooling, firewall rules |
| Verify VPN accessibility | Team Lead Developer | Ensure no interruption to secure remote access |
| Update internal documentation (temporary) | Team Lead Developer | Pending full ISMS update post-move |

###  **Post-Move (Starting September 1)**
| Action | Responsible | Target Date |
|--------|-------------|-------------|
| Update Asset Inventory | Managing Director | Sept 5 |
| Update Risk Register (e.g., "Home-hosted NAS/Dev Server") | Managing Director | Sept 10 |
| Update BCDR Plan (remove office as fallback location) | Team Lead Developer | Sept 10 |
| Reassess Annex A.7 controls (physical access) | Team Lead Developer | Sept 15 |
| Create home access policy (locked room, access restrictions) | CEO | Sept 15 |
| Record changes in Change Control Log | Managing Director | Immediately |

---

## 3. Infrastructure Relocation Details

### A. NAS (Backup Device)
- **New Location:** CEO's locked home office
- **Power & Connectivity:** Verified stable power & internet
- **Physical Access Control:** Locked room, access only by CEO
- **Backups:** Daily + Incremental remains active

### B. Development Server (VPN Endpoint)
- **New Location:** Same as NAS
- **Firewall Config:** New IP range whitelisted
- **VPN Logs & Monitoring:** Continue as-is
- **RDP + Admin Access:** Maintained securely

---

## 4. Roles and Responsibilities
| Role               | Responsibility During Transition                  |
|--------------------|----------------------------------------------------|
| CEO                | Device relocation, secure setup at home location  |
| Team Lead Developer| Connectivity, VPN, backup validation              |
| Managing Director  | ISMS updates, Change Log, Risk Register           |

---

## 5. Required ISMS Updates Post-Move
- **Asset Inventory:** New location, ownership, and access notes
- **Risk Register:** Add or modify risks for home-hosted systems
- **BCDR Plan:** Remove physical office as fallback; update contact chain
- **Annex A.7 Controls:** Replace office-based physical security with home-based controls (e.g., locked room, no shared access)
- **Access Control Policy:** Ensure VPN usage is logged and restricted to authorized devices
- **Awareness Training (optional):** Remind team of WFH security responsibilities

---

## 6. Change Control Log Entries
The following entries should be included in the Change Control Log:
```md
| CHG-2025-024 | 2025-08-25 | Planned transition to full remote work (effective September 1, 2025) | Office operations still active during audit. ISMS scope and controls to be updated after relocation. | Managing Director |
| CHG-2025-026 | 2025-08-25 | Planned relocation of NAS and Dev Server to owner's home | Devices remain in office until September. Physical access, VPN config, and backup protection will be maintained and ISMS will be updated post-move. | Team Lead Developer |
```

---

## 7. Annex – Checklist & References

### Checklist
- [ ] Devices securely packed and relocated
- [ ] Remote connectivity (VPN, RDP) tested from home
- [ ] NAS backup process verified after relocation
- [ ] Asset inventory updated
- [ ] Physical access policy for home location documented
- [ ] Risk Register updated
- [ ] ISMS Manual and relevant policies updated

### References
- [ISMS Manual](https://github.com/rate-nl/ISO/blob/main/readme.md)
- [Change Control Log](https://your-change-control-log-link)
- [BCDR Plan](https://your-bcdr-plan-link)
- [Risk Register](https://your-risk-register-link)
