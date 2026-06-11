# 🛠️ Semana 0 — Setup & Preparación (Día 0, 1-2 días antes de iniciar)

> **Propósito:** Tener TODO listo para que el Día 1 sea 100% productivo. Sin fricción.  
> **Duración estimada:** 3-4 horas (se puede hacer en 1 sábado)  
> **NO cuenta como día del plan** — es preparación previa.

---

## ✅ Checklist Completo

### 1. Cuentas y Suscripciones

| # | Tarea | URL | Status |
|---|-------|-----|--------|
| 1.1 | Crear cuenta AWS (o verificar existente) | https://aws.amazon.com/free/ | ⬜ |
| 1.2 | Comprar curso Cantrill SAA-C03 ($40) | https://learn.cantrill.io/p/aws-certified-solutions-architect-associate-saa-c03 | ⬜ |
| 1.3 | Registrarse en AWS SkillBuilder (gratuito) | https://explore.skillbuilder.aws/ | ⬜ |
| 1.4 | Comprar TutorialsDojo SAA Practice Exams ($15) | https://portal.tutorialsdojo.com/courses/aws-certified-solutions-architect-associate-practice-exams/ | ⬜ |
| 1.5 | Suscribirse a ChatGPT Plus ($20/mes) | https://chat.openai.com/ | ⬜ |
| 1.6 | Crear cuenta Grammarly (free) | https://www.grammarly.com/ | ⬜ |
| 1.7 | Registrarse en SmallTalk2Me (free) | https://www.smalltalk2.me/ | ⬜ |

**💡 NO comprar aún:**
- AWS SkillBuilder suscripción ($29) → se activa en S15
- Examen SAA-C03 ($150) → se agenda en S19-S20

---

### 2. Herramientas de Desarrollo

| # | Tarea | URL / Comando | Status |
|---|-------|---------------|--------|
| 2.1 | Instalar Java 17+ (preferido: Java 21 LTS) | `brew install openjdk@21` | ⬜ |
| 2.2 | Instalar Maven | `brew install maven` | ⬜ |
| 2.3 | Instalar Docker Desktop | https://www.docker.com/products/docker-desktop/ | ⬜ |
| 2.4 | Instalar/verificar Git | `git --version` | ⬜ |
| 2.5 | Instalar IDE (IntelliJ / VS Code + Kiro) | https://www.jetbrains.com/idea/ | ⬜ |
| 2.6 | Instalar AWS CLI v2 | `brew install awscli` | ⬜ |
| 2.7 | Instalar Postman o HTTPie | https://www.postman.com/ o `brew install httpie` | ⬜ |

**Verificar versiones:**
```bash
java --version      # ≥ 17
mvn --version       # ≥ 3.8
docker --version    # ≥ 24
git --version       # ≥ 2.x
aws --version       # ≥ 2.x
```

---

### 3. Anki — Vocabulario

| # | Tarea | URL | Status |
|---|-------|-----|--------|
| 3.1 | Instalar Anki (desktop) | https://apps.ankiweb.net/ | ⬜ |
| 3.2 | Instalar Anki (móvil) para repaso en movimiento | Android: Play Store / iOS: App Store ($25) | ⬜ |
| 3.3 | Descargar deck "4000 Essential English Words" | https://ankiweb.net/shared/info/413429709 | ⬜ |
| 3.4 | Configurar: 20 new cards/day, 100 max reviews | Settings → New cards: 20, Reviews: 100 | ⬜ |
| 3.5 | Hacer primera sesión de prueba (10 cards) | — | ⬜ |

---

### 4. GitHub — Repositorios y Project Board

| # | Tarea | Detalles | Status |
|---|-------|----------|--------|
| 4.1 | Crear repositorio: `banking-docs` | Público, con README, licencia MIT | ⬜ |
| 4.2 | Crear repositorio: `banking-identity-service` | Público, vacío (lo inicializamos en S1) | ⬜ |
| 4.3 | Crear GitHub Project Board: "Banking Platform — 120 Days" | Tipo: Board (Kanban) | ⬜ |
| 4.4 | Crear Milestones en cada repo | Fase 1, Fase 2, Fase 3, Fase 4 | ⬜ |
| 4.5 | Crear Labels | Ver tabla abajo | ⬜ |
| 4.6 | Crear Issues de Semana 1 | 6 issues (ver semana-01.md) | ⬜ |

**Labels a crear:**

| Label | Color | Uso |
|-------|-------|-----|
| `fase-1` | 🟦 Blue | Semanas 1-7 |
| `fase-2` | 🟧 Orange | Semanas 8-14 |
| `fase-3` | 🟥 Red | Semanas 15-18 |
| `fase-4` | 🟪 Purple | Semanas 19-20 |
| `aws` | ☁️ Light blue | Tareas AWS |
| `arquitectura` | 🏗️ Green | Patrones, código |
| `enterprise` | 📐 Teal | ADRs, TOGAF, Capability Maps |
| `inglés` | 🇬🇧 Yellow | Speaking, writing |
| `saa-practice` | 📝 Gray | Simulacros |
| `devops` | ⚙️ Dark gray | Docker, CI/CD, infra |
| `documentation` | 📄 White | READMEs, docs |
| `setup` | 🔧 Brown | Configuración inicial |

**Estructura de columnas del Project Board:**

```
| Backlog | To Do (esta semana) | In Progress | Done |
```

---

### 5. Estructura Inicial de `banking-docs`

```bash
# Clonar y crear estructura
git clone git@github.com:TU_USER/banking-docs.git
cd banking-docs

mkdir -p docs/plan
mkdir -p docs/adr
mkdir -p docs/enterprise
mkdir -p docs/katas
mkdir -p weekly

# Mover archivos existentes
cp PLAN-MAESTRO-120-DIAS.md docs/plan/
cp weekly/semana-01.md weekly/
```

**Estructura resultante:**
```
banking-docs/
├── README.md
├── docs/
│   ├── plan/
│   │   └── PLAN-MAESTRO-120-DIAS.md
│   ├── adr/
│   │   └── (ADR-001 se crea en S1)
│   ├── enterprise/
│   │   └── (Capability Map se crea en S1)
│   └── katas/
│       └── (Kata #1 se crea en S9)
├── weekly/
│   ├── semana-00-setup.md (este archivo)
│   └── semana-01.md
└── LICENSE
```

---

### 6. Configuración AWS (se completa en Día 1, pero se prepara aquí)

| # | Tarea | Detalles | Status |
|---|-------|----------|--------|
| 6.1 | Crear cuenta AWS (email dedicado recomendado) | No usar email personal principal | ⬜ |
| 6.2 | Activar MFA en root account | Authenticator app | ⬜ |
| 6.3 | Crear IAM admin user (no usar root para trabajo diario) | — | ⬜ |
| 6.4 | Configurar AWS CLI con IAM user credentials | `aws configure` | ⬜ |
| 6.5 | Crear Budget alarm ($10/mes) | AWS Console → Billing → Budgets | ⬜ |

---

### 7. Inglés — Setup adicional

| # | Tarea | URL | Status |
|---|-------|-----|--------|
| 7.1 | Instalar app de grabación de voz | Voice Memos (iOS) o Easy Voice Recorder (Android) | ⬜ |
| 7.2 | Crear carpeta "speaking-recordings/" en Drive/local | Para guardar grabaciones diarias | ⬜ |
| 7.3 | Suscribirse a AWS Podcast | https://aws.amazon.com/podcasts/aws-podcast/ | ⬜ |
| 7.4 | Suscribirse a Software Engineering Daily | https://softwareengineeringdaily.com/ | ⬜ |
| 7.5 | Descargar 2-3 episodios para tener offline | — | ⬜ |

---

### 8. Libros — Obtener

| # | Libro | Formato | Status |
|---|-------|---------|--------|
| 8.1 | Fundamentals of Software Architecture (Richards & Ford) | PDF / físico / O'Reilly | ⬜ |
| 8.2 | Designing Data-Intensive Applications (Kleppmann) | PDF / físico / O'Reilly | ⬜ |
| 8.3 | Release It! (Nygard) | PDF / físico | ⬜ |
| 8.4 | TOGAF Pocket Guide | PDF gratuito (overview) | ⬜ |

**Nota:** Solo necesitas el #1 para empezar. Los demás se usan desde S8 (DDIA) y S15 (Release It!).

---

## 📋 Resumen de Costos — Fase 0

| Item | Costo |
|------|-------|
| Cantrill SAA-C03 | $40 |
| TutorialsDojo | $15 |
| ChatGPT Plus (1er mes) | $20 |
| Anki iOS (si usas iPhone) | $25 (o $0 si Android/desktop) |
| **Total Fase 0** | **$75-100** |

---

## ⏰ Orden sugerido para completar (3-4 horas)

```
Hora 1:  Instalar herramientas dev (Java, Maven, Docker, AWS CLI)
Hora 2:  Crear cuentas (AWS, Cantrill, SkillBuilder, TutorialsDojo)
Hora 3:  GitHub setup (repos, project board, labels, milestones, issues S1)
Hora 4:  Anki setup + descargar podcasts + obtener libro FSA
```

---

## ✅ Criterio de "Fase 0 Completada"

Estás listo para el Día 1 cuando:

- [ ] `java --version` funciona (≥ 17)
- [ ] `docker --version` funciona
- [ ] `aws --version` funciona
- [ ] Cantrill comprado y puedes ver videos
- [ ] Anki instalado con deck de 4000 palabras cargado
- [ ] GitHub repos creados (`banking-docs`, `banking-identity-service`)
- [ ] Project Board creado con issues de S1
- [ ] Libro "Fundamentals of SA" disponible para leer
- [ ] 2-3 podcasts descargados
- [ ] Grabadora de voz lista en el teléfono

**Si todo está ✅ → arrancas Día 1 sin fricción.**
