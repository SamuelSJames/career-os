---
tags: [plan, ccnp, encor, year1]
exam: "CCNP ENCOR 350-401"
length: 26 weeks
updated: 2026-06-26
---
# CCNP ENCOR (350-401) — 26-Week Study Plan

Year 1 spine. Finish this, then ENARSI → **CCNP Enterprise complete**. This is the credential that
makes me the rare SA who deeply understands enterprise networks (see [[MISSION]] / ROADMAP).

## Calendar Anchor

| | |
|---|---|
| **Study Week 1** | week of **Mon Jul 6, 2026** |
| **Holiday break** | weeks of **Nov 23 → Dec 21, 2026** (~5 wks OFF — Thanksgiving→Christmas; banked videos auto-publish) |
| **Resume** | week of **Jan 4, 2027** (Study Week 21) |
| **Exam target** | week of **Feb 8, 2027** (Study Week 26) |

> Study Weeks 1–20 run Jul→mid-Nov 2026. The break pauses the clock. Weeks 21–26 run Jan→early Feb 2027.
> "Study week" ≠ calendar week during the break — the 26 are *active* weeks.

## Blueprint Weights (study time follows these)

| # | Domain | Weight |
|---|---|---|
| 3.0 | Infrastructure (L2/L3/Wireless/IP Services) | **30%** |
| 5.0 | Security | 20% |
| 1.0 | Architecture | 15% |
| 6.0 | Automation | 15% |
| 2.0 | Virtualization | 10% |
| 4.0 | Network Assurance | 10% |

## How to Use This

- **~10–15 focused hrs/week**: study + 1 lab + 1 video. Pre-holiday weeks (W17–W20) bank ~2 videos/wk.
- **Resources are employer-funded** — pull ENCOR material from the work learning platform first
  (O'Reilly/Skillsoft/Cisco U/OCG) before buying anything. Boson ExSim for practice exams.
- **Labs in pnetlab** (homelab). Every lab → its own folder in `labs/` (README + diagram + configs + write-up).
- **Teaching is studying**: each week's video explains that week's lab/topic. No silent weeks.
- Trilium "CCNP ENCOR Study" folder holds the domain notes.

---

## Phase 1 — Foundations + Architecture (W1–W2)

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 1 | Jul 6 | Enterprise design: 2-tier/3-tier, collapsed core, spine-leaf; high-level SD-WAN & SD-Access; campus design principles. Tooling: repo-per-lab + Git branching habit. | pnetlab base topology + Git repo scaffold | "Why enterprise network design matters" (channel intro/rep #0) |
| 2 | Jul 13 | Architecture cont.: WLAN deployment models, AP modes, cloud vs on-prem mgmt; QoS concepts (classification, marking, queuing, shaping/policing); network programmability intro. | Baseline router/switch topology, save configs to Git | QoS concepts explained simply |

## Phase 2 — Infrastructure: Layer 2 (W3–W7)

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 3 | Jul 20 | VLANs, access/trunk ports, 802.1Q, VTP, native VLAN, voice VLAN | Inter-VLAN routing (router-on-a-stick + SVI) | VLANs & trunking |
| 4 | Jul 27 | EtherChannel — LACP/PAgP/static, L2 vs L3, load-balancing, troubleshooting | LACP + L3 EtherChannel lab | EtherChannel deep-dive |
| 5 | Aug 3 | STP fundamentals: 802.1D, PVST+, root election, port roles/states | STP root manipulation lab | How STP picks a root |
| 6 | Aug 10 | RSTP + MST, STP toolkit (PortFast, BPDU Guard/Filter, Root Guard, Loop Guard) | RSTP + protection features lab | STP protection features |
| 7 | Aug 17 | L2 troubleshooting + consolidation (trunks, EtherChannel, STP together) | Broken-L2 troubleshooting scenario | Troubleshooting a Layer 2 loop |

## Phase 3 — Infrastructure: Layer 3 Routing (W8–W12)

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 8 | Aug 24 | Routing fundamentals, longest-match, admin distance; static/default; IPv6 addressing refresh | Static + IPv6 routing lab | How routers choose paths |
| 9 | Aug 31 | OSPF single-area: adjacencies, LSAs, DR/BDR, network types, timers | OSPFv2 single-area lab | OSPF neighbors & DR/BDR |
| 10 | Sep 7 | OSPF multi-area: area types, summarization, path selection, OSPFv3 | OSPF multi-area + summarization lab | OSPF areas explained |
| 11 | Sep 14 | EIGRP basics (DUAL, metrics, feasible successor) — ENCOR depth | EIGRP basics lab | EIGRP in 15 minutes |
| 12 | Sep 21 | eBGP fundamentals: peering, path attributes, best-path basics | eBGP single-homed lab | What BGP actually does |

## Phase 4 — Wireless + IP Services (W13–W16)

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 13 | Sep 28 | Wireless: RF basics, 802.11, AP/WLC, CAPWAP, roaming, WLAN config flow | WLC config walkthrough (sim/diagram) | Wireless for the CCNP |
| 14 | Oct 5 | FHRP: HSRP, VRRP, GLBP — design + config + failover | HSRP/VRRP failover lab | First-hop redundancy explained |
| 15 | Oct 12 | NAT/PAT, NTP, DHCP, SLA + object tracking | NAT + NTP + tracking lab | NAT/PAT done right |
| 16 | Oct 19 | IP services consolidation + IPv6 services | Mixed IP-services scenario | IPv6 services overview |

## Phase 5 — Network Assurance (W17) + 🦃🎄 BANK WINDOW (W17–W20)

> **W17–W20 = bank ~2 videos/week** ahead of the break. These are normal study weeks too.

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 17 | Oct 26 | Assurance: SNMP, syslog, NetFlow/Flexible NetFlow, SPAN/RSPAN/ERSPAN, IP SLA, debugs, DNA Center assurance | NetFlow + SPAN capture lab | Network telemetry tools (BANK x2) |
| 18 | Nov 2 | Security 1: device access (lines, SSH, password mgmt), AAA (RADIUS/TACACS+), ACLs (v4/v6) | AAA + ACL hardening lab | Securing device access (BANK x2) |
| 19 | Nov 9 | Security 2: CoPP, 802.1X, MAB, MACsec, wireless security (WPA2/3, PSK/Enterprise) | 802.1X + CoPP lab | Port security & 802.1X (BANK x2) |
| 20 | Nov 16 | Security 3: network security design — TrustSec/SGT, threat defense concepts; finish banking | Security design diagram + review | Enterprise security design (BANK x2) |

### 🛑 Nov 23 → Dec 21, 2026 — OFF. Banked videos publish. Accountability paused. Rest.

## Phase 6 — Virtualization + Automation (W21–W24, resume Jan 2027)

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 21 | Jan 4 | Virtualization: VRF-lite, GRE, IPsec basics; LISP & VXLAN overview | VRF-lite + GRE tunnel lab | VRF & tunnels explained |
| 22 | Jan 11 | Device/network virtualization: hypervisors, containers, NFV; SD-Access & SD-WAN architecture deeper | SD-Access/SD-WAN architecture diagram | SDN & overlays for CCNP |
| 23 | Jan 18 | Automation 1: data formats (JSON/XML/YAML), Python fundamentals, REST APIs, NETCONF/RESTCONF | Python script hitting a device API | Network automation basics |
| 24 | Jan 25 | Automation 2: EEM, Ansible/Puppet/Chef concepts, Cisco DNA Center APIs, controllers | EEM applet + simple Ansible playbook | EEM & Ansible intro |

## Phase 7 — Review + Exam (W25–W26)

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 25 | Feb 1 | Full blueprint review; **practice exam #1 (Boson)**; rebuild weakest 2–3 labs | Weak-area redo labs | "What I'd tell someone starting ENCOR" |
| 26 | Feb 8 | Practice exams #2–3 to passing margin; final OCG skim; **SIT ENCOR 350-401** ✅ | — | Exam debrief / lessons learned |

---

## Milestones
- **W7** — Layer 2 solid.
- **W12** — Core routing (OSPF/EIGRP/BGP basics) solid → the ENARSI on-ramp.
- **W20** — Security done + video buffer banked → break with a clear head.
- **W26** — **Pass ENCOR.** ~26 videos, ~22 labs from this exam alone.

## Definition of Done (per mission)
ENCOR isn't "done" at a passing score — it's done when each domain has a lab + write-up + video I can
point to. Cert = recognition; the portfolio = proof.
