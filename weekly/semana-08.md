# 📋 Semana 8 (Días 43-48) — SQS/SNS/EventBridge + Microservicios Split (parte 1)

> **Fase:** 2 — Avanzado  
> **Foco:** Split monolito → Identity + Accounts microservicios, API Gateway, messaging AWS

---

## 🎯 Objetivos de la Semana

- [ ] Cantrill: SQS + SNS + EventBridge
- [ ] SkillBuilder: Serverless Foundations + Messaging + SAA Prep Mod 3
- [ ] Identity service como microservicio independiente (repo propio)
- [ ] Accounts service como microservicio independiente (repo propio)
- [ ] API Gateway (Spring Cloud Gateway)
- [ ] ADR-005: "Decompose to microservices"
- [ ] Capability Map v0.3
- [ ] Migration plan (TOGAF Phase E-F)
- [ ] TutorialsDojo: Route53+CloudFront+DynamoDB ≥ 70%
- [ ] Libro: DDIA Cap 1

---

## 🔗 Recursos

| Recurso | URL |
|---------|-----|
| Cantrill SQS/SNS/EventBridge | https://learn.cantrill.io |
| Spring Cloud Gateway | https://docs.spring.io/spring-cloud-gateway/reference/ |
| Microservices.io decomposition | https://microservices.io/patterns/decomposition/ |
| TOGAF Phase E-F | https://pubs.opengroup.org/togaf-standard/ |
| DDIA | Designing Data-Intensive Applications — Cap 1 |

---

## 📅 Distribución Diaria

| Día | AWS (1h) | Arquitectura (1h) | Inglés highlight |
|-----|----------|-------------------|-----------------|
| 43 (Lun) | Cantrill: SQS (standard, FIFO, DLQ) | Planificar split: qué queda en cada servicio | Speaking: "justify why we split the monolith" |
| 44 (Mar) | Cantrill: SQS (visibility timeout, polling) | Create `banking-identity-service` repo, extract code | Speaking: "explain SQS vs SNS" |
| 45 (Mié) | Cantrill: SNS (topics, fan-out) | Create `banking-accounts-service` repo, extract code | Writing: ADR-005 draft |
| 46 (Jue) | Cantrill: EventBridge (rules, event bus) | Create `banking-api-gateway` + `banking-shared-kernel` | Writing: Migration plan |
| 47 (Vie) | SkillBuilder: Serverless + Messaging + SAA Mod 3 | Wire services together (REST calls through gateway) | Speaking: "explain API Gateway pattern" |
| 48 (Sáb) | TutorialsDojo: 15 preguntas Route53+CF+DynamoDB | Test end-to-end through gateway, push all repos | Speaking: "weekly summary" |

---

## ✅ Checklist de Cierre

| Entregable | Status |
|-----------|--------|
| `banking-identity-service` repo + running independently | ⬜ |
| `banking-accounts-service` repo + running independently | ⬜ |
| `banking-api-gateway` repo + routing working | ⬜ |
| `banking-shared-kernel` repo (DTOs, events) | ⬜ |
| Each service has own DB | ⬜ |
| ADR-005: "Decompose to microservices" | ⬜ |
| Capability Map v0.3 | ⬜ |
| Migration plan (TOGAF E-F) | ⬜ |
| Cantrill SQS+SNS+EventBridge | ⬜ |
| TutorialsDojo ≥ 70% | ⬜ Score: ___% |
| DDIA Cap 1 | ⬜ |
| Anki: 120 palabras | ⬜ |

---

## GitHub Issues

```
Issue #33: [S8] Extract Identity to independent microservice
Labels: arquitectura, fase-2, proyecto
Milestone: Fase 2

Issue #34: [S8] Extract Accounts to independent microservice
Labels: arquitectura, fase-2, proyecto
Milestone: Fase 2

Issue #35: [S8] Create API Gateway (Spring Cloud Gateway)
Labels: arquitectura, fase-2, proyecto
Milestone: Fase 2

Issue #36: [S8] Create shared-kernel (domain events, common DTOs)
Labels: arquitectura, fase-2, proyecto
Milestone: Fase 2

Issue #37: [S8] Write ADR-005 + Migration Plan
Labels: enterprise, fase-2, documentation
Milestone: Fase 2
```
