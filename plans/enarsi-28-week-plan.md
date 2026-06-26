---
tags: [plan, ccnp, enarsi, year1]
exam: "CCNP ENARSI 300-410"
length: 28 weeks
updated: 2026-06-26
---
# CCNP ENARSI (300-410) — 28-Week Study Plan

The CCNP Enterprise **concentration** that completes the cert. Builds directly on ENCOR's routing
core and goes deep + troubleshooting-heavy. Passing this → **CCNP Enterprise complete** (see ROADMAP).

## Calendar Anchor

| | |
|---|---|
| **Study Week 1** | week of **Mon Feb 15, 2027** (right after the ENCOR exam) |
| **Holiday break** | none in this window (Feb→Aug 2027 is clear) |
| **Exam target** | week of **Aug 23, 2027** (Study Week 28) |

> ⚠️ **Timeline note:** 28 weeks from mid-Feb lands the exam ~**late Aug / Sep 2027**, ~2–3 months
> past the ROADMAP's original "ENARSI ~Jun 2027." This is the deliberate deeper-pace trade. Decide
> whether to (a) accept CCNP completing ~Sep 2027 and shift Year 2 SAA start to ~Oct 2027, or
> (b) compress ENARSI to ~18 weeks to hold the Jun 2027 date. Recorded in DECISION-LOG when chosen.

## Blueprint Weights (study time follows these)

| # | Domain | Weight |
|---|---|---|
| 1.0 | Layer 3 Technologies (EIGRP/OSPF/BGP/redistribution/route control) | **35%** |
| 4.0 | Infrastructure Services (SNMP/syslog/IP SLA/NetFlow/NTP/DHCP/DNS) | 25% |
| 2.0 | VPN Technologies (MPLS L3VPN, DMVPN, IPsec) | 20% |
| 3.0 | Infrastructure Security (ACLs, CoPP, IPv6 FHS, AAA, uRPF) | 20% |

ENARSI's signature is **troubleshooting** — every domain is tested as "find and fix the break,"
not just "configure it." Labs lean diagnostic.

## How to Use This

- Same rhythm as ENCOR: ~10–15 hrs/wk, study + 1 lab + 1 video. Employer-funded resources first
  (OCG ENARSI, Cisco U, Boson ExSim 300-410). pnetlab for every lab.
- **Build broken topologies on purpose** and fix them — that's the exam.
- Each domain → `labs/` folder with the fault, the diagnosis path, and the fix documented.

---

## Phase 1 — Bridge + L3 Foundations (W1–W2)

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 1 | Feb 15 | Troubleshooting methodology (structured: verify→isolate→fix); routing table deep-read, RIB vs FIB, admin distance interactions | "Read the routing table" diagnostic lab | A repeatable troubleshooting method |
| 2 | Feb 22 | IPv4/IPv6 addressing edge cases; PBR intro; static route options (recursive, fully-specified, floating) | Floating static + PBR lab | Policy-based routing explained |

## Phase 2 — EIGRP Deep (W3–W6)

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 3 | Mar 1 | EIGRP named mode, metrics (wide), DUAL deep, feasibility condition | EIGRP named-mode build | EIGRP named mode |
| 4 | Mar 8 | Summarization, stub routing, load balancing (variance), default routing | EIGRP summarization + stub lab | EIGRP stub & summarization |
| 5 | Mar 15 | EIGRP authentication, EIGRP for IPv6, query/SIA behavior | EIGRP IPv6 + auth lab | EIGRP authentication & IPv6 |
| 6 | Mar 22 | **EIGRP troubleshooting** — neighbor, route, path problems | Broken-EIGRP scenario | Fixing EIGRP adjacency problems |

## Phase 3 — OSPF Deep (W7–W11)

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 7 | Mar 29 | OSPF adjacency conditions, network types, timers, DR/BDR deep | OSPF network-types lab | Why OSPF won't form a neighbor |
| 8 | Apr 5 | LSA types, area types (stub/NSSA/totally), path selection | OSPF area-types lab | OSPF LSAs & area types |
| 9 | Apr 12 | Summarization (inter-area/external), filtering (LSA/route), virtual links | OSPF summarization + filtering lab | OSPF route filtering |
| 10 | Apr 19 | OSPFv3 (IPv6 + address families), authentication | OSPFv3 lab | OSPFv3 done right |
| 11 | Apr 26 | **OSPF troubleshooting** — adjacency, LSA, path issues | Broken-OSPF scenario | Troubleshooting OSPF path selection |

## Phase 4 — BGP Deep (W12–W16)

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 12 | May 3 | eBGP vs iBGP, neighbor states, next-hop, split-horizon rule | iBGP + eBGP peering lab | iBGP vs eBGP |
| 13 | May 10 | Path attributes + best-path algorithm (full order) | BGP best-path lab | BGP best-path, step by step |
| 14 | May 17 | Route filtering: prefix-lists, route-maps, AS-path filters, communities | BGP filtering + communities lab | BGP filtering & communities |
| 15 | May 24 | BGP for IPv6 (MP-BGP), peer groups/templates, authentication | MP-BGP IPv6 lab | BGP for IPv6 |
| 16 | May 31 | **BGP troubleshooting** — peering, advertisement, path manipulation | Broken-BGP scenario | Why isn't this BGP route installed? |

## Phase 5 — Redistribution + Route Control (W17–W18)

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 17 | Jun 7 | Multi-protocol redistribution, seed metrics, admin-distance pitfalls, route tagging to stop loops | 3-protocol redistribution lab | Redistribution without loops |
| 18 | Jun 14 | Route maps + prefix/distribute lists in anger; VRF-lite; redistribution troubleshooting | VRF-lite + filtered redistribution lab | VRF-lite explained |

## Phase 6 — VPN Technologies (W19–W21)

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 19 | Jun 21 | MPLS fundamentals: labels, LDP, LSR/LER, forwarding | MPLS LDP lab | MPLS in plain English |
| 20 | Jun 28 | MPLS L3VPN: VRF, RD/RT, PE-CE routing, MP-BGP VPNv4 | MPLS L3VPN lab | How MPLS L3VPN works |
| 21 | Jul 5 | DMVPN Phase 1 (NHRP, mGRE) + site-to-site IPsec concepts | DMVPN single-hub lab | DMVPN from scratch |

## Phase 7 — Infrastructure Security (W22–W23)

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 22 | Jul 12 | ACLs deep (v4/v6, time-based, troubleshooting), uRPF, CoPP | ACL + CoPP lab | CoPP & uRPF |
| 23 | Jul 19 | IPv6 first-hop security (RA Guard, DHCPv6 Guard, ND inspection), AAA/device hardening | IPv6 FHS lab | IPv6 first-hop security |

## Phase 8 — Infrastructure Services (W24–W25)

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 24 | Jul 26 | SNMP v2c/v3, syslog, NTP (auth), DHCP (server/relay/client + troubleshooting), DNS | DHCP relay + SNMPv3 lab | DHCP relay troubleshooting |
| 25 | Aug 2 | IP SLA + object tracking, NetFlow/Flexible NetFlow, network mgmt (SSH/file transfer/restore) | IP SLA tracking + NetFlow lab | IP SLA & object tracking |

## Phase 9 — Cross-Domain TS + Exam (W26–W28)

| Wk | Wk of | Focus | Lab | Video |
|----|-------|-------|-----|-------|
| 26 | Aug 9 | **Cross-domain troubleshooting** — multi-protocol break/fix tickets (ENARSI's real test) | Full mixed-fault scenario | How to attack an ENARSI trouble ticket |
| 27 | Aug 16 | **Practice exam #1–2 (Boson)**; rebuild weakest labs; OCG gap-fill | Weak-area redo labs | — |
| 28 | Aug 23 | Practice exams to passing margin; final review; **SIT ENARSI 300-410 → CCNP COMPLETE** 🎉 | — | "CCNP done — what it took" |

---

## Milestones
- **W6 / W11 / W16** — each routing protocol (EIGRP/OSPF/BGP) deep + troubleshootable.
- **W18** — redistribution & route control mastered (the classic CCNP gauntlet).
- **W21** — VPN technologies covered (MPLS/DMVPN — strong video content).
- **W26** — can attack any multi-domain trouble ticket methodically.
- **W28** — **Pass ENARSI → CCNP Enterprise complete.**

## Definition of Done
CCNP complete = ENCOR + ENARSI passed **and** a networking portfolio of ~40+ documented labs and
~50 videos across both exams — the proof that backs the credential.
