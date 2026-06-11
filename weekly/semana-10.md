# 📋 Semana 10 (Días 55-60) — API Gateway/Cognito/KMS + CQRS

> **Fase:** 2 — Avanzado  
> **Foco:** CQRS en Transactions service, command/query separation, Kata #2

---

## 🎯 Objetivos de la Semana

- [ ] Cantrill: API Gateway + Cognito + KMS + Secrets Manager + SSM
- [ ] SkillBuilder: API Gateway + Security Services + SAA Prep Mod 4
- [ ] CQRS implementado en Transactions service
- [ ] Command handlers (register transaction) + Query handlers (movements)
- [ ] Read model: account movements projection
- [ ] ADR-006: "Apply CQRS to Transactions service"
- [ ] Capability Map v0.4
- [ ] Kata #2: Sistema de pagos con alta disponibilidad
- [ ] Tag: `v0.6-cqrs`
- [ ] TutorialsDojo: SQS+SNS+Lambda ≥ 72%
- [ ] Libro: DDIA Cap 5

---

## 🔗 Recursos

| Recurso | URL |
|---------|-----|
| Cantrill API GW/Cognito/KMS | https://learn.cantrill.io |
| CQRS (Martin Fowler) | https://martinfowler.com/bliki/CQRS.html |
| CQRS (microservices.io) | https://microservices.io/patterns/data/cqrs.html |
| DDIA Cap 5 | Designing Data-Intensive Applications — Replication |

---

## 📅 Distribución Diaria

| Día | AWS (1h) | Arquitectura (1h) | Inglés highlight |
|-----|----------|-------------------|-----------------|
| 55 (Lun) | Cantrill: API Gateway (REST, HTTP APIs) | Study CQRS pattern (Fowler + microservices.io) | Speaking: "explain CQRS and why we need it" |
| 56 (Mar) | Cantrill: Cognito (user pools, identity pools) | Implement Command side: RegisterTransaction handler | Speaking: "explain Cognito user pools" |
| 57 (Mié) | Cantrill: KMS (symmetric, asymmetric, key policies) | Implement Query side: GetMovements projection | Writing: ADR-006 draft |
| 58 (Jue) | Cantrill: Secrets Manager + SSM Parameter Store | Separate read DB (in-memory/H2 for now) + projection update | Writing: Kata #2 solution |
| 59 (Vie) | SkillBuilder: API Gateway + Security + SAA Mod 4 | Integration tests CQRS, Capability Map v0.4 | Speaking: "explain CQRS trade-offs" |
| 60 (Sáb) | TutorialsDojo: 15 preguntas SQS+SNS+Lambda | Tag v0.6, push, Kata #2 documented | Speaking: "weekly summary" |

---

## ✅ Checklist de Cierre

| Entregable | Status |
|-----------|--------|
| CQRS in Transactions service | ⬜ |
| Command handlers working | ⬜ |
| Query handlers + read model | ⬜ |
| Separate read DB (projection) | ⬜ |
| ADR-006: "CQRS in Transactions" | ⬜ |
| Capability Map v0.4 | ⬜ |
| Architecture Kata #2 | ⬜ |
| Tag: `v0.6-cqrs` | ⬜ |
| Cantrill API GW+Cognito+KMS+SSM | ⬜ |
| TutorialsDojo ≥ 72% | ⬜ Score: ___% |
| DDIA Cap 5 | ⬜ |
| Anki: 120 palabras | ⬜ |

---

## GitHub Issues

```
Issue #42: [S10] Implement CQRS — Command side (RegisterTransaction)
Labels: arquitectura, fase-2, proyecto
Milestone: Fase 2

Issue #43: [S10] Implement CQRS — Query side (Movements projection)
Labels: arquitectura, fase-2, proyecto
Milestone: Fase 2

Issue #44: [S10] Write ADR-006: CQRS in Transactions
Labels: enterprise, fase-2, documentation
Milestone: Fase 2

Issue #45: [S10] Architecture Kata #2: High-availability payments
Labels: enterprise, fase-2, documentation
Milestone: Fase 2
```
