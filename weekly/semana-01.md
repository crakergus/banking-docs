# 📋 Semana 1 (Días 1-6) — AWS Accounts & IAM + Clean Architecture + TOGAF Intro

> **Fase:** 1 — Fundamentos  
> **Fechas:** ___/___ al ___/___  
> **Foco:** Configurar AWS, inicializar proyecto con Clean Architecture, primer ADR, Capability Map borrador

---

## 🎯 Objetivos de la Semana

- [ ] Cuenta AWS configurada con MFA + Budget alarm
- [ ] Proyecto `banking-identity-service` inicializado (Spring Boot 3, Java 17, Maven)
- [ ] User entity + CRUD básico (register, get) con Clean Architecture
- [ ] Dockerfile funcional
- [ ] ADR-001 escrito en inglés
- [ ] Capability Map v0.1 (borrador)
- [ ] Cantrill: IAM sección completa
- [ ] Anki: 120 palabras nuevas esta semana (20/día)

---

## 📅 Día a Día

---

### Día 1 (Lunes)

| Bloque | Duración | Actividad | Recurso |
|--------|----------|-----------|---------|
| 🇬🇧 Input pasivo | 15 min | Podcast: AWS Podcast — episodio reciente | podcasts.apple.com/aws-podcast |
| 🇬🇧 Anki | 10 min | 20 palabras nuevas (cloud/IAM vocabulary) | Anki deck propio |
| 🇬🇧 Shadowing | 10 min | Repetir frases de Cantrill intro IAM | learn.cantrill.io |
| 🇬🇧 Input activo | 15 min | Leer: AWS IAM docs — "What is IAM?" | docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html |
| 🇬🇧 Speaking | 20 min | Grabarse 2 min: "What is IAM and why do we need it?" | Grabadora del teléfono |
| 🇬🇧 Writing | 20 min | Escribir README.md del proyecto en inglés (draft) | VS Code |
| ☁️ AWS | 60 min | Cantrill SAA-C03: Course intro + AWS Accounts + IAM basics (users, groups) | learn.cantrill.io |
| 🏗️ Arquitectura | 60 min | Leer Clean Architecture (Dependency Rule, capas). Inicializar proyecto Spring Boot: `banking-identity-service`, estructura de packages | Fundamentals of SA Cap 1 + Spring Initializr |

**Entregables del día:**
- [ ] Anki: 20 palabras
- [ ] Cantrill: AWS Accounts + IAM intro completado
- [ ] Proyecto Maven creado con estructura Clean Architecture
- [ ] README.md (draft, en inglés)
- [ ] Grabación speaking: 2 min

**Estructura de proyecto a crear:**
```
banking-identity-service/
├── src/main/java/com/banking/identity/
│   ├── domain/           (entities, value objects, repository interfaces)
│   ├── application/      (use cases, DTOs, ports)
│   ├── infrastructure/   (persistence adapters, web controllers)
│   └── BankingIdentityApplication.java
├── src/test/java/com/banking/identity/
├── pom.xml
├── Dockerfile
└── README.md
```

---

### Día 2 (Martes)

| Bloque | Duración | Actividad | Recurso |
|--------|----------|-----------|---------|
| 🇬🇧 Input pasivo | 15 min | Podcast: AWS Podcast — otro episodio | podcasts.apple.com/aws-podcast |
| 🇬🇧 Anki | 10 min | Repaso + 20 palabras nuevas (architecture terms) | Anki |
| 🇬🇧 Shadowing | 10 min | Cantrill: repetir frases de IAM policies | learn.cantrill.io |
| 🇬🇧 Input activo | 15 min | Leer: IAM Policies docs (JSON structure, Effect/Action/Resource) | docs.aws.amazon.com/IAM |
| 🇬🇧 Speaking | 20 min | Grabarse 2 min: "Explain IAM policies — Effect, Action, Resource" | Grabadora |
| 🇬🇧 Writing | 20 min | Escribir primeros commits del proyecto en inglés | Git |
| ☁️ AWS | 60 min | Cantrill: IAM Policies (identity vs resource), Policy evaluation logic, IAM Roles | learn.cantrill.io |
| 🏗️ Arquitectura | 60 min | Implementar User domain entity + RegisterUser use case (application layer). Escribir tests unitarios del domain | IDE + JUnit 5 |

**Entregables del día:**
- [ ] Anki: 20 palabras (total: 40)
- [ ] Cantrill: IAM Policies + Roles completado
- [ ] User.java (domain entity) implementado
- [ ] RegisterUserUseCase.java (application layer)
- [ ] UserRepository.java (port/interface en domain)
- [ ] Tests unitarios de domain
- [ ] Commits en inglés

---

### Día 3 (Miércoles)

| Bloque | Duración | Actividad | Recurso |
|--------|----------|-----------|---------|
| 🇬🇧 Input pasivo | 15 min | Podcast: Software Engineering Daily — episodio de arquitectura | se-radio.net |
| 🇬🇧 Anki | 10 min | Repaso + 20 nuevas (DDD/architecture terms) | Anki |
| 🇬🇧 Shadowing | 10 min | Cantrill: frases de Organizations/SCPs | learn.cantrill.io |
| 🇬🇧 Input activo | 15 min | Leer: MADR template (ADR format) | adr.github.io/madr |
| 🇬🇧 Speaking | 20 min | Grabarse 2 min: "What is Clean Architecture and the Dependency Rule?" | Grabadora |
| 🇬🇧 Writing | 20 min | Escribir ADR-001 draft en inglés | Markdown |
| ☁️ AWS | 60 min | Cantrill: AWS Organizations, SCPs, CloudTrail basics | learn.cantrill.io |
| 🏗️ Arquitectura | 60 min | Implementar infrastructure layer: JPA adapter (UserJpaRepository), Web controller (UserController). docker-compose con PostgreSQL | IDE + Docker |

**Entregables del día:**
- [ ] Anki: 20 palabras (total: 60)
- [ ] Cantrill: Organizations + SCPs + CloudTrail
- [ ] UserJpaRepository.java (infrastructure adapter)
- [ ] UserController.java (REST endpoint: POST /users, GET /users/{id})
- [ ] docker-compose.yml con PostgreSQL
- [ ] ADR-001 draft iniciado

---

### Día 4 (Jueves)

| Bloque | Duración | Actividad | Recurso |
|--------|----------|-----------|---------|
| 🇬🇧 Input pasivo | 15 min | Podcast: The Cloudcast — episodio reciente | thecloudcast.net |
| 🇬🇧 Anki | 10 min | Repaso + 20 nuevas (AWS terms: SCP, OU, policy) | Anki |
| 🇬🇧 Shadowing | 10 min | Cantrill: frases de CloudTrail | learn.cantrill.io |
| 🇬🇧 Input activo | 15 min | Leer: TOGAF ADM cycle overview (Wikipedia/OpenGroup resumen) | opengroup.org/togaf |
| 🇬🇧 Speaking | 20 min | Grabarse 2 min: "Explain the layers of my Banking project" | Grabadora |
| 🇬🇧 Writing | 20 min | Completar ADR-001: "Use Clean Architecture for Banking Platform" | Markdown |
| ☁️ AWS | 60 min | Cantrill: IAM avanzado (cross-account access, permission boundaries) + crear cuenta AWS con MFA | learn.cantrill.io + AWS Console |
| 🏗️ Arquitectura | 60 min | Tests de integración (UserController + DB). Crear Dockerfile. Verificar que docker-compose levanta app + DB | IDE + Docker |

**Entregables del día:**
- [ ] Anki: 20 palabras (total: 80)
- [ ] Cantrill: IAM avanzado completado
- [ ] Cuenta AWS creada con MFA + IAM admin user
- [ ] Tests de integración pasando
- [ ] Dockerfile funcional
- [ ] ADR-001 completado en formato MADR

---

### Día 5 (Viernes)

| Bloque | Duración | Actividad | Recurso |
|--------|----------|-----------|---------|
| 🇬🇧 Input pasivo | 15 min | Podcast: InfoQ Podcast — episodio de enterprise architecture | infoq.com/podcasts |
| 🇬🇧 Anki | 10 min | Repaso + 20 nuevas (TOGAF terms: ADM, phase, capability) | Anki |
| 🇬🇧 Shadowing | 10 min | Cantrill: frases de IAM advanced | learn.cantrill.io |
| 🇬🇧 Input activo | 15 min | Leer: Capability Mapping intro (Martin Fowler o similar) | martinfowler.com |
| 🇬🇧 Speaking | 20 min | Grabarse 2 min: "What is a Capability Map and why I need one?" | Grabadora |
| 🇬🇧 Writing | 20 min | Escribir Capability Map v0.1 borrador (Markdown + Mermaid) | Markdown |
| ☁️ AWS | 60 min | AWS SkillBuilder: Cloud Practitioner Essentials Módulos 1-2 (Cloud concepts, Compute) + Budget alarm en AWS | explore.skillbuilder.aws |
| 🏗️ Arquitectura | 60 min | TOGAF intro: leer ADM cycle, entender Phase A (Architecture Vision). Documentar vision statement del Banking Platform | Fundamentals of SA Cap 1 (completar) |

**Entregables del día:**
- [ ] Anki: 20 palabras (total: 100)
- [ ] SkillBuilder: Módulos 1-2 completados
- [ ] Budget alarm configurado en AWS ($10 threshold)
- [ ] Capability Map v0.1 borrador (Mermaid)
- [ ] Architecture Vision statement (1 párrafo en inglés)

---

### Día 6 (Sábado)

| Bloque | Duración | Actividad | Recurso |
|--------|----------|-----------|---------|
| 🇬🇧 Input pasivo | 15 min | Podcast: AWS Podcast — otro episodio | podcasts.apple.com/aws-podcast |
| 🇬🇧 Anki | 10 min | Repaso + 20 nuevas | Anki |
| 🇬🇧 Shadowing | 10 min | Cantrill: frases de SkillBuilder módulos | — |
| 🇬🇧 Input activo | 15 min | Leer: Fundamentals of SA Cap 1 (completar si quedó pendiente) | Libro |
| 🇬🇧 Speaking | 20 min | Grabarse 2-3 min: "Summary of what I learned this week" | Grabadora |
| 🇬🇧 Writing | 20 min | Completar README.md final + revisar todos los commits en inglés | Git |
| ☁️ AWS | 60 min | SkillBuilder: Cloud Practitioner Essentials Módulo 3 (Global Infrastructure) + repaso IAM Cantrill (lo que quedó flojo) | explore.skillbuilder.aws |
| 🏗️ Arquitectura | 60 min | Pulir proyecto: completar tests faltantes, refactor si es necesario, asegurar que todo corre con `docker-compose up`. Push final | IDE + Git |

**Entregables del día:**
- [ ] Anki: 20 palabras (total: 120)
- [ ] SkillBuilder: Módulo 3 completado
- [ ] Proyecto corriendo limpio con docker-compose
- [ ] README.md completo en inglés
- [ ] Speaking resumen semanal grabado (2-3 min)
- [ ] Push a GitHub con todo el trabajo de la semana

---

## ✅ Checklist de Cierre Semanal

| Entregable | Status |
|-----------|--------|
| Cuenta AWS con MFA + Budget alarm | ⬜ |
| IAM admin user (no root) | ⬜ |
| Proyecto `banking-identity-service` con Clean Architecture | ⬜ |
| User entity + RegisterUser use case + tests | ⬜ |
| REST endpoint: POST /users, GET /users/{id} | ⬜ |
| Dockerfile funcional | ⬜ |
| docker-compose (app + PostgreSQL) | ⬜ |
| ADR-001: "Use Clean Architecture for Banking Platform" | ⬜ |
| Capability Map v0.1 (borrador Mermaid) | ⬜ |
| README.md en inglés | ⬜ |
| Cantrill: IAM section completa | ⬜ |
| SkillBuilder: Módulos 1-3 completados | ⬜ |
| Anki: 120 palabras (6 días × 20) | ⬜ |
| Grabaciones speaking: 6 (una por día) | ⬜ |
| Commits en inglés: ≥ 5 | ⬜ |
| Libro: Fundamentals of SA Cap 1 leído | ⬜ |

---

## 📊 Métricas de la Semana

| Métrica | Target | Real |
|---------|--------|------|
| Horas totales | 21h | ___h |
| Anki streak | 6/6 | ___/6 |
| Grabaciones speaking | 6 | ___ |
| Commits en inglés | ≥ 5 | ___ |
| Cantrill videos completados | IAM section | ___ |
| SkillBuilder módulos | 3 | ___ |

---

## 🔗 Links de Recursos — Semana 1

### AWS
- Cantrill SAA-C03: https://learn.cantrill.io (IAM section)
- SkillBuilder gratuito: https://explore.skillbuilder.aws/learn/course/134/cloud-practitioner-essentials
- IAM Docs: https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html
- AWS Free Tier: https://aws.amazon.com/free/

### Arquitectura
- Clean Architecture (resumen): https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html
- MADR template: https://adr.github.io/madr/
- TOGAF overview: https://www.opengroup.org/togaf
- Capability Mapping: https://www.leanix.net/en/wiki/ea/capability-map

### Libro
- Fundamentals of Software Architecture (Richards & Ford) — Cap 1: "Introduction" + "Architectural Thinking"

### Inglés
- Anki (desktop): https://apps.ankiweb.net/
- AWS Podcast: https://aws.amazon.com/podcasts/aws-podcast/
- Software Engineering Daily: https://softwareengineeringdaily.com/

---

## 📝 Notas / Reflexiones

_Espacio para escribir al final de cada día o semana lo que aprendiste, dificultades, ajustes._

---

## GitHub Issues sugeridos para esta semana

```
Issue #1: [S1] Setup AWS Account + MFA + Budget
Labels: aws, fase-1, setup
Milestone: Fase 1

Issue #2: [S1] Initialize banking-identity-service with Clean Architecture
Labels: arquitectura, fase-1, proyecto
Milestone: Fase 1

Issue #3: [S1] Implement User entity + RegisterUser use case
Labels: arquitectura, fase-1, proyecto
Milestone: Fase 1

Issue #4: [S1] Create Dockerfile + docker-compose
Labels: devops, fase-1, proyecto
Milestone: Fase 1

Issue #5: [S1] Write ADR-001: Clean Architecture decision
Labels: enterprise, fase-1, documentation
Milestone: Fase 1

Issue #6: [S1] Draft Capability Map v0.1
Labels: enterprise, fase-1, documentation
Milestone: Fase 1
```
