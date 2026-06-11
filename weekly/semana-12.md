# 📋 Semana 12 (Días 67-72) — EKS/CloudWatch/X-Ray + Saga Pattern

> **Fase:** 2 — Avanzado  
> **Foco:** Transfer Saga (debit → credit → confirm), Outbox pattern, compensating transactions

---

## 🎯 Objetivos de la Semana

- [ ] Cantrill: EKS + CloudWatch + X-Ray
- [ ] SkillBuilder: Containers Deep Dive + Monitoring + SAA Prep Mod 6
- [ ] Transfer Saga implementada (InitTransfer → DebitSource → CreditTarget → Confirm)
- [ ] Compensating transactions (RevertDebit on failure)
- [ ] Outbox table
- [ ] ADR-008 (parte 1)
- [ ] ARB presentation document
- [ ] Kata #3: Pipeline de datos real-time
- [ ] TutorialsDojo: CloudFormation+EKS+CloudWatch ≥ 72%
- [ ] Libro: DDIA Cap 7

---

## 🔗 Recursos

| Recurso | URL |
|---------|-----|
| Saga pattern | https://microservices.io/patterns/data/saga.html |
| Outbox pattern | https://microservices.io/patterns/data/transactional-outbox.html |
| Cantrill EKS/CloudWatch | https://learn.cantrill.io |
| DDIA Cap 7 | Designing Data-Intensive Applications — Transactions |

---

## ✅ Checklist de Cierre

| Entregable | Status |
|-----------|--------|
| Transfer Saga (debit → credit → confirm) | ⬜ |
| Compensating transactions working | ⬜ |
| Outbox table implemented | ⬜ |
| ADR-008 (parte 1) drafted | ⬜ |
| ARB presentation document | ⬜ |
| Kata #3 documented | ⬜ |
| TutorialsDojo ≥ 72% | ⬜ Score: ___% |
| DDIA Cap 7 | ⬜ |

---

## GitHub Issues

```
Issue #50: [S12] Implement Transfer Saga (choreography)
Labels: arquitectura, fase-2, proyecto
Milestone: Fase 2

Issue #51: [S12] Implement compensating transactions
Labels: arquitectura, fase-2, proyecto
Milestone: Fase 2

Issue #52: [S12] Implement Outbox table pattern
Labels: arquitectura, fase-2, proyecto
Milestone: Fase 2

Issue #53: [S12] Architecture Kata #3: Real-time data pipeline
Labels: enterprise, fase-2, documentation
Milestone: Fase 2
```
