# 📋 Semana 6 (Días 31-36) — DynamoDB/Route53/CloudFront + Deploy AWS

> **Fase:** 1 — Fundamentos  
> **Foco:** Deploy a AWS (ECS/Fargate + RDS), CI/CD, TO-BE document, primer simulacro seccional

---

## 🎯 Objetivos de la Semana

- [ ] Cantrill: DynamoDB + Route53 + CloudFront + ACM
- [ ] SkillBuilder: DynamoDB + Route53 + CloudFront + SAA Prep Mod 2
- [ ] Banking Platform corriendo en ECS/Fargate
- [ ] RDS PostgreSQL en subnet privada
- [ ] CI/CD pipeline (GitHub Actions)
- [ ] ADR-004: "Deploy strategy with ECS Fargate"
- [ ] TO-BE document + Gap Analysis
- [ ] Technology Radar v0.1
- [ ] TutorialsDojo seccional ≥ 70%
- [ ] Tag: `v0.4-aws-deploy`

---

## 🔗 Recursos

| Recurso | URL |
|---------|-----|
| Cantrill DynamoDB/Route53/CF | https://learn.cantrill.io |
| ECS Docs | https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ |
| GitHub Actions ECS deploy | https://docs.github.com/en/actions/deployment/deploying-to-amazon-ecs |
| Technology Radar (Thoughtworks) | https://www.thoughtworks.com/radar |
| TutorialsDojo | https://portal.tutorialsdojo.com/ |

---

## 📅 Distribución Diaria

| Día | AWS (1h) | Arquitectura (1h) | Inglés highlight |
|-----|----------|-------------------|-----------------|
| 31 (Lun) | Cantrill: DynamoDB (tables, LSI, GSI) | ECS task definition + Dockerfile optimization | Speaking: "explain DynamoDB GSI vs LSI" |
| 32 (Mar) | Cantrill: DynamoDB (streams, DAX) | Create VPC + subnets + ALB in AWS console | Speaking: "explain my deploy architecture" |
| 33 (Mié) | Cantrill: Route53 (routing policies) | Deploy app to ECS/Fargate + connect to RDS | Writing: ADR-004 draft |
| 34 (Jue) | Cantrill: CloudFront + ACM | GitHub Actions CI/CD pipeline (build → test → deploy) | Writing: TO-BE document |
| 35 (Vie) | SkillBuilder: DynamoDB + Route53 + SAA Prep Mod 2 | Technology Radar v0.1 + Gap Analysis | Speaking: "explain our TO-BE vision" |
| 36 (Sáb) | TutorialsDojo: 15 preguntas IAM+S3+VPC+EC2 | Verificar deploy end-to-end, tag v0.4, push | Speaking: "weekly summary" |

---

## ✅ Checklist de Cierre

| Entregable | Status |
|-----------|--------|
| App running on ECS/Fargate | ⬜ |
| RDS PostgreSQL in private subnet | ⬜ |
| ALB with health checks | ⬜ |
| CI/CD pipeline (GitHub Actions) | ⬜ |
| ADR-004: "Deploy with ECS Fargate" | ⬜ |
| TO-BE document | ⬜ |
| Gap Analysis (AS-IS → TO-BE) | ⬜ |
| Technology Radar v0.1 | ⬜ |
| Tag: `v0.4-aws-deploy` | ⬜ |
| TutorialsDojo score ≥ 70% | ⬜ Score: ___% |
| Cantrill DynamoDB+Route53+CloudFront | ⬜ |
| Anki: 120 palabras | ⬜ |

---

## GitHub Issues

```
Issue #25: [S6] Deploy Banking Platform to ECS/Fargate
Labels: aws, devops, fase-1
Milestone: Fase 1

Issue #26: [S6] Setup CI/CD pipeline (GitHub Actions)
Labels: devops, fase-1
Milestone: Fase 1

Issue #27: [S6] Write ADR-004: Deploy strategy
Labels: enterprise, fase-1, documentation
Milestone: Fase 1

Issue #28: [S6] Create TO-BE document + Gap Analysis
Labels: enterprise, fase-1, documentation
Milestone: Fase 1

Issue #29: [S6] Create Technology Radar v0.1
Labels: enterprise, fase-1, documentation
Milestone: Fase 1
```
