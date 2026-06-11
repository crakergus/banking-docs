# 📋 Semana 9 (Días 49-54) — Step Functions/Lambda + Microservicios completado

> **Fase:** 2 — Avanzado  
> **Foco:** Transactions + Notifications services, Docker Compose multi-service, Kata #1

---

## 🎯 Objetivos de la Semana

- [ ] Cantrill: Step Functions + Lambda
- [ ] SkillBuilder: Lambda Deep Dive + Step Functions
- [ ] Transactions service creado (`banking-transactions-service`)
- [ ] Notifications service stub (`banking-notifications-service`)
- [ ] Docker Compose multi-service (4 services + gateway)
- [ ] Architecture Kata #1: Sistema de notificaciones multi-canal
- [ ] Tag: `v0.5-microservices`
- [ ] TutorialsDojo: SQS+SNS+EventBridge ≥ 70%
- [ ] Libro: DDIA Cap 2 + Cap 3

---

## 🔗 Recursos

| Recurso | URL |
|---------|-----|
| Cantrill Lambda/Step Functions | https://learn.cantrill.io |
| Architecture Katas | https://nealford.com/katas/ |
| Docker Compose networking | https://docs.docker.com/compose/networking/ |
| DDIA | Designing Data-Intensive Applications — Cap 2-3 |

---

## 📅 Distribución Diaria

| Día | AWS (1h) | Arquitectura (1h) | Inglés highlight |
|-----|----------|-------------------|-----------------|
| 49 (Lun) | Cantrill: Step Functions (standard, express) | Create `banking-transactions-service` (domain model) | Speaking: "explain Step Functions use cases" |
| 50 (Mar) | Cantrill: Lambda basics (invocation, permissions) | Transactions: use cases (CreateTransaction, GetMovements) | Speaking: "explain our microservice boundaries" |
| 51 (Mié) | Cantrill: Lambda (layers, concurrency, DLQ) | Create `banking-notifications-service` (stub: logs events) | Writing: Kata #1 context + constraints |
| 52 (Jue) | Cantrill: Lambda + Step Functions integration | Docker Compose: 4 services + gateway + 2 DBs | Writing: Kata #1 solution + diagram |
| 53 (Vie) | SkillBuilder: Lambda Deep Dive | Test communication between services (REST) | Speaking: "present Kata #1 solution" |
| 54 (Sáb) | TutorialsDojo: 15 preguntas SQS+SNS+EventBridge | Tag v0.5, push all repos, Kata doc final | Speaking: "weekly summary" |

---

## ✅ Checklist de Cierre

| Entregable | Status |
|-----------|--------|
| `banking-transactions-service` running | ⬜ |
| `banking-notifications-service` (stub) running | ⬜ |
| Docker Compose: 4 services + gateway | ⬜ |
| Services communicate via REST | ⬜ |
| Architecture Kata #1 documented | ⬜ |
| Tag: `v0.5-microservices` | ⬜ |
| Cantrill Lambda + Step Functions | ⬜ |
| TutorialsDojo ≥ 70% | ⬜ Score: ___% |
| DDIA Cap 2+3 | ⬜ |
| Anki: 120 palabras | ⬜ |

---

## GitHub Issues

```
Issue #38: [S9] Create Transactions service (domain + use cases)
Labels: arquitectura, fase-2, proyecto
Milestone: Fase 2

Issue #39: [S9] Create Notifications service (stub)
Labels: arquitectura, fase-2, proyecto
Milestone: Fase 2

Issue #40: [S9] Docker Compose multi-service (4 services + gateway)
Labels: devops, fase-2
Milestone: Fase 2

Issue #41: [S9] Architecture Kata #1: Notifications system
Labels: enterprise, fase-2, documentation
Milestone: Fase 2
```
