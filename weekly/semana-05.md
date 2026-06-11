# 📋 Semana 5 (Días 25-30) — ELB/ASG/RDS + Bounded Contexts + Governance

> **Fase:** 1 — Fundamentos  
> **Foco:** Accounts module completo, bounded contexts, flujo end-to-end, AS-IS document

---

## 🎯 Objetivos de la Semana

- [ ] Cantrill: ELB + ASG + RDS + Aurora
- [ ] SkillBuilder: ELB Deep Dive + RDS Intro + SAA Exam Prep Mod 1
- [ ] Accounts module completo (open, close, balance, deposit, withdraw)
- [ ] Flyway migrations
- [ ] Flujo end-to-end: register → assign role → open account → deposit
- [ ] ADR-003: "Separate bounded contexts"
- [ ] AS-IS document del monolito
- [ ] Tag: `v0.3-modules`
- [ ] Libro: Fundamentals of SA Cap 11

---

## 🔗 Recursos

| Recurso | URL |
|---------|-----|
| Cantrill ELB/ASG/RDS | https://learn.cantrill.io |
| SkillBuilder SAA Prep Mod 1 | https://explore.skillbuilder.aws |
| RDS Docs | https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/ |
| DDD Bounded Context | https://martinfowler.com/bliki/BoundedContext.html |
| Flyway | https://documentation.red-gate.com/fd |

---

## 📅 Distribución Diaria

| Día | AWS (1h) | Arquitectura (1h) | Inglés highlight |
|-----|----------|-------------------|-----------------|
| 25 (Lun) | Cantrill: ELB (ALB architecture, listeners, rules) | Accounts domain: Account entity, value objects | Speaking: "explain ALB vs NLB" |
| 26 (Mar) | Cantrill: ASG (scaling policies, lifecycle) | Accounts use cases: OpenAccount, Deposit, Withdraw | Speaking: "explain auto scaling" |
| 27 (Mié) | Cantrill: RDS (architecture, Multi-AZ) | Accounts adapters (persistence + web) | Writing: ADR-003 draft |
| 28 (Jue) | Cantrill: Aurora (serverless, read replicas) | Flyway setup + migrations | Speaking: "RDS Multi-AZ vs Read Replica" |
| 29 (Vie) | SkillBuilder: ELB Deep Dive + RDS Intro | Integration tests + end-to-end flow | Writing: AS-IS document |
| 30 (Sáb) | SkillBuilder: SAA Exam Prep Mod 1 | Pulir, tag v0.3, push | Speaking: "describe my system architecture" |

---

## ✅ Checklist de Cierre

| Entregable | Status |
|-----------|--------|
| Accounts: open, close, balance, deposit, withdraw | ⬜ |
| 3 bounded contexts (Identity, Entitlements, Accounts) | ⬜ |
| Flyway migrations working | ⬜ |
| End-to-end flow functional | ⬜ |
| ADR-003: "Separate bounded contexts" | ⬜ |
| AS-IS document | ⬜ |
| Tag: `v0.3-modules` | ⬜ |
| Cantrill ELB+ASG+RDS+Aurora | ⬜ |
| SkillBuilder: ELB + RDS + SAA Mod 1 | ⬜ |
| Libro Cap 11 | ⬜ |
| Anki: 120 palabras | ⬜ |

---

## GitHub Issues

```
Issue #20: [S5] Implement Accounts module (open, close, deposit, withdraw)
Labels: arquitectura, fase-1, proyecto
Milestone: Fase 1

Issue #21: [S5] Setup Flyway migrations
Labels: devops, fase-1
Milestone: Fase 1

Issue #22: [S5] End-to-end flow: register → role → account → deposit
Labels: arquitectura, fase-1, proyecto
Milestone: Fase 1

Issue #23: [S5] Write ADR-003: Bounded Contexts
Labels: enterprise, fase-1, documentation
Milestone: Fase 1

Issue #24: [S5] Document AS-IS architecture
Labels: enterprise, fase-1, documentation
Milestone: Fase 1
```
