# 📋 Semana 3 (Días 13-18) — VPC & Networking + Hexagonal Architecture + TOGAF Phase B

> **Fase:** 1 — Fundamentos  
> **Foco:** Refactoring a hexagonal, Entitlements (Roles + Permissions), VPC networking

---

## 🎯 Objetivos de la Semana

- [ ] Cantrill: VPC section completa (subnets, routing, SGs, NACLs, endpoints)
- [ ] SkillBuilder: Networking Basics + Security Intro
- [ ] Refactoring a Hexagonal Architecture iniciado
- [ ] Roles + Permissions domain model implementado
- [ ] ADR-002: "Adopt Hexagonal Architecture"
- [ ] Capability Map v0.2 (business capabilities)
- [ ] Libro: Fundamentals of SA Cap 3-4

---

## 🔗 Recursos

| Recurso | URL |
|---------|-----|
| Cantrill VPC | https://learn.cantrill.io (VPC section) |
| SkillBuilder Networking | https://explore.skillbuilder.aws |
| VPC Docs | https://docs.aws.amazon.com/vpc/latest/userguide/ |
| Hexagonal Architecture (Cockburn) | https://alistair.cockburn.us/hexagonal-architecture/ |
| Netflix Tech Blog (hexagonal) | https://netflixtechblog.com/ |
| TOGAF Phase B | https://pubs.opengroup.org/togaf-standard/adm/chap06.html |

---

## 📅 Distribución Diaria

| Día | AWS (1h) | Arquitectura (1h) | Inglés highlight |
|-----|----------|-------------------|-----------------|
| 13 (Lun) | Cantrill: VPC basics, sizing, subnets | Estudiar hexagonal pattern (Cockburn article) | Speaking: "what are ports and adapters?" |
| 14 (Mar) | Cantrill: Routing, IGW, NAT Gateway | Refactor Identity: extract domain ports | Speaking: "explain VPC subnets" |
| 15 (Mié) | Cantrill: Security Groups, NACLs | Refactor Identity: create infrastructure adapters | Writing: ADR-002 draft |
| 16 (Jue) | Cantrill: VPC Peering, VPC Endpoints | Role entity + Permission entity (domain) | Writing: TOGAF Phase B notes |
| 17 (Vie) | Cantrill: Flow Logs + SkillBuilder Networking | AssignRole use case + CheckPermission use case | Speaking: "explain RBAC model" |
| 18 (Sáb) | SkillBuilder: Security Intro | Tests + Capability Map v0.2 + push | Speaking: "weekly summary" |

---

## ✅ Checklist de Cierre

| Entregable | Status |
|-----------|--------|
| VPC concepts (diagramar de memoria) | ⬜ |
| Hexagonal refactoring iniciado (Identity) | ⬜ |
| Role + Permission domain entities | ⬜ |
| AssignRole + CheckPermission use cases | ⬜ |
| ADR-002: "Adopt Hexagonal Architecture" | ⬜ |
| Capability Map v0.2 | ⬜ |
| Cantrill VPC section completa | ⬜ |
| SkillBuilder: Networking + Security | ⬜ |
| Libro Cap 3-4 | ⬜ |
| Anki: 120 palabras | ⬜ |
| Speaking: 6 grabaciones | ⬜ |

---

## GitHub Issues

```
Issue #12: [S3] Refactor Identity module to Hexagonal Architecture
Labels: arquitectura, fase-1, proyecto
Milestone: Fase 1

Issue #13: [S3] Implement Roles + Permissions domain model
Labels: arquitectura, fase-1, proyecto
Milestone: Fase 1

Issue #14: [S3] Write ADR-002: Hexagonal Architecture
Labels: enterprise, fase-1, documentation
Milestone: Fase 1

Issue #15: [S3] Update Capability Map v0.2
Labels: enterprise, fase-1, documentation
Milestone: Fase 1
```
