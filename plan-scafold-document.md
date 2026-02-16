---
status: unfilled
generated: "{{DATE}}"
agents:
  # Selecione apenas os agents relevantes para este plano.
  # Remova os que nao se aplicam.
  - type: "code-reviewer"
    role: "Review code changes for quality, style, and best practices"
  - type: "bug-fixer"
    role: "Analyze bug reports and error messages"
  - type: "feature-developer"
    role: "Implement new features according to specifications"
  - type: "refactoring-specialist"
    role: "Identify code smells and improvement opportunities"
  - type: "test-writer"
    role: "Write comprehensive unit and integration tests"
  - type: "documentation-writer"
    role: "Create clear, comprehensive documentation"
  - type: "performance-optimizer"
    role: "Identify performance bottlenecks"
  - type: "security-auditor"
    role: "Identify security vulnerabilities"
  - type: "backend-specialist"
    role: "Design and implement server-side architecture"
  - type: "frontend-specialist"
    role: "Design and implement user interfaces"
  - type: "architect-specialist"
    role: "Design overall system architecture and patterns"
  - type: "devops-specialist"
    role: "Design and maintain CI/CD pipelines"
  - type: "database-specialist"
    role: "Design and optimize database schemas"
  - type: "mobile-specialist"
    role: "Develop native and cross-platform mobile applications"
docs:
  # Liste os documentos de contexto que este plano referencia.
  # Ajuste conforme a estrutura do seu projeto.
  - "project-overview.md"
  - "architecture.md"
  - "development-workflow.md"
  - "testing-strategy.md"
  - "glossary.md"
  - "data-flow.md"
  - "security.md"
  - "tooling.md"
phases:
  - id: "phase-1"
    name: "Discovery & Alignment"
    prevc: "P"
  - id: "phase-2"
    name: "Implementation & Iteration"
    prevc: "E"
  - id: "phase-3"
    name: "Validation & Handoff"
    prevc: "V"
---

## Task Snapshot
- **Primary goal:** {{TODO: Descreva o resultado esperado deste plano.}}
- **Success signal:** {{TODO: Defina como a equipe sabera que o plano foi bem-sucedido.}}
- **Key references:**
  - [Documentation Index](../docs/README.md)
  - [Agent Handbook](../agents/README.md)
  - [Plans Index](./README.md)

## Codebase Context

> Preencha esta secao com dados reais do projeto. Use ferramentas de analise
> estatica ou explore o repositorio para coletar as metricas abaixo.

- **Total files analyzed:** {{TODO: numero de arquivos}}
- **Total symbols discovered:** {{TODO: numero de simbolos exportados}}
- **Architecture layers:** {{TODO: ex. Config, Utils, Components, Services, Controllers}}
- **Entry points:** {{TODO: ex. src/index.ts, src/main.tsx}}

### Key Components

**Key Interfaces:**
<!-- Liste as interfaces/tipos centrais do dominio com caminhos relativos ao root do projeto. -->
- `{{InterfaceName}}` — `{{caminho/relativo/ao/arquivo.ts:linha}}`

**Key Services / Modules:**
<!-- Liste os servicos ou modulos principais. -->
- `{{ServiceName}}` — `{{caminho/relativo/ao/arquivo.ts:linha}}`

## Agent Lineup

> Mantenha apenas os agents necessarios para este plano. Remova linhas nao utilizadas.

| Agent | Role in this plan | Playbook | First responsibility focus |
| --- | --- | --- | --- |
| Code Reviewer | {{TODO: Por que este agent participa.}} | [Code Reviewer](../agents/code-reviewer.md) | Review code changes for quality, style, and best practices |
| Bug Fixer | {{TODO: Por que este agent participa.}} | [Bug Fixer](../agents/bug-fixer.md) | Analyze bug reports and error messages |
| Feature Developer | {{TODO: Por que este agent participa.}} | [Feature Developer](../agents/feature-developer.md) | Implement new features according to specifications |
| Refactoring Specialist | {{TODO: Por que este agent participa.}} | [Refactoring Specialist](../agents/refactoring-specialist.md) | Identify code smells and improvement opportunities |
| Test Writer | {{TODO: Por que este agent participa.}} | [Test Writer](../agents/test-writer.md) | Write comprehensive unit and integration tests |
| Documentation Writer | {{TODO: Por que este agent participa.}} | [Documentation Writer](../agents/documentation-writer.md) | Create clear, comprehensive documentation |
| Performance Optimizer | {{TODO: Por que este agent participa.}} | [Performance Optimizer](../agents/performance-optimizer.md) | Identify performance bottlenecks |
| Security Auditor | {{TODO: Por que este agent participa.}} | [Security Auditor](../agents/security-auditor.md) | Identify security vulnerabilities |
| Backend Specialist | {{TODO: Por que este agent participa.}} | [Backend Specialist](../agents/backend-specialist.md) | Design and implement server-side architecture |
| Frontend Specialist | {{TODO: Por que este agent participa.}} | [Frontend Specialist](../agents/frontend-specialist.md) | Design and implement user interfaces |
| Architect Specialist | {{TODO: Por que este agent participa.}} | [Architect Specialist](../agents/architect-specialist.md) | Design overall system architecture and patterns |
| Devops Specialist | {{TODO: Por que este agent participa.}} | [Devops Specialist](../agents/devops-specialist.md) | Design and maintain CI/CD pipelines |
| Database Specialist | {{TODO: Por que este agent participa.}} | [Database Specialist](../agents/database-specialist.md) | Design and optimize database schemas |
| Mobile Specialist | {{TODO: Por que este agent participa.}} | [Mobile Specialist](../agents/mobile-specialist.md) | Develop native and cross-platform mobile applications |

## Documentation Touchpoints

> Ajuste os caminhos relativos conforme a estrutura `.context/docs/` do seu projeto.

| Guide | File | Primary Inputs |
| --- | --- | --- |
| Project Overview | [project-overview.md](../docs/project-overview.md) | Roadmap, README, stakeholder notes |
| Architecture Notes | [architecture.md](../docs/architecture.md) | ADRs, service boundaries, dependency graphs |
| Development Workflow | [development-workflow.md](../docs/development-workflow.md) | Branching rules, CI config, contributing guide |
| Testing Strategy | [testing-strategy.md](../docs/testing-strategy.md) | Test configs, CI gates, known flaky suites |
| Glossary & Domain Concepts | [glossary.md](../docs/glossary.md) | Business terminology, user personas, domain rules |
| Data Flow & Integrations | [data-flow.md](../docs/data-flow.md) | System diagrams, integration specs, queue topics |
| Security & Compliance Notes | [security.md](../docs/security.md) | Auth model, secrets management, compliance requirements |
| Tooling & Productivity Guide | [tooling.md](../docs/tooling.md) | CLI scripts, IDE configs, automation workflows |

## Risk Assessment

> Identifique bloqueios potenciais, dependencias e estrategias de mitigacao antes de iniciar.

### Identified Risks
| Risk | Probability | Impact | Mitigation Strategy | Owner |
| --- | --- | --- | --- | --- |
| {{TODO: Descreva o risco}} | Low / Medium / High | Low / Medium / High | {{TODO: Estrategia de mitigacao}} | {{TODO: Responsavel}} |

### Dependencies
- **Internal:** {{TODO: Dependencias de outras equipes, servicos ou infraestrutura interna}}
- **External:** {{TODO: Dependencias de servicos terceiros, vendors ou parceiros}}
- **Technical:** {{TODO: Pre-requisitos tecnicos ou upgrades necessarios}}

### Assumptions
- {{TODO: Documente premissas-chave (ex. "API schema atual permanece estavel")}}
- {{TODO: Descreva o que acontece se a premissa for invalidada}}

## Resource Estimation

### Time Allocation
| Phase | Estimated Effort | Calendar Time | Team Size |
| --- | --- | --- | --- |
| Phase 1 - Discovery | {{TODO: ex. 2 person-days}} | {{TODO: ex. 3-5 days}} | {{TODO: ex. 1-2 people}} |
| Phase 2 - Implementation | {{TODO: ex. 5 person-days}} | {{TODO: ex. 1-2 weeks}} | {{TODO: ex. 2-3 people}} |
| Phase 3 - Validation | {{TODO: ex. 2 person-days}} | {{TODO: ex. 3-5 days}} | {{TODO: ex. 1-2 people}} |
| **Total** | **{{TODO: total}}** | **{{TODO: total}}** | **-** |

### Required Skills
- {{TODO: Liste expertise necessaria (ex. "React", "Database optimization", "Infrastructure")}}
- {{TODO: Identifique gaps de conhecimento e necessidades de treinamento}}

### Resource Availability
- **Available:** {{TODO: Membros da equipe e disponibilidade}}
- **Blocked:** {{TODO: Membros com prioridades conflitantes}}
- **Escalation:** {{TODO: Contato para escalar se recursos forem insuficientes}}

## Working Phases

### Phase 1 — Discovery & Alignment

**Steps**
1. {{TODO: Descreva tarefas de discovery e atribua o responsavel.}}
2. {{TODO: Capture perguntas abertas que precisam de esclarecimento.}}

**Commit Checkpoint**
- Ao concluir esta fase, capture o contexto acordado e crie um commit:
  `git commit -m "chore(plan): complete phase 1 discovery"`

### Phase 2 — Implementation & Iteration

**Steps**
1. {{TODO: Descreva tarefas de build, expectativas de pairing e cadencia de review.}}
2. {{TODO: Referencie docs ou playbooks para manter mudancas alinhadas.}}

**Commit Checkpoint**
- Sumarize progresso, atualize cross-links e crie um commit:
  `git commit -m "chore(plan): complete phase 2 implementation"`

### Phase 3 — Validation & Handoff

**Steps**
1. {{TODO: Detalhe testes, verificacao e atualizacoes de documentacao.}}
2. {{TODO: Documente evidencias que a equipe deve capturar para mantenedores.}}

**Commit Checkpoint**
- Registre evidencias de validacao e crie um commit:
  `git commit -m "chore(plan): complete phase 3 validation"`

## Rollback Plan

> Documente como reverter mudancas caso problemas surjam durante ou apos a implementacao.

### Rollback Triggers
Quando iniciar rollback:
- Critical bugs afetando funcionalidade core
- Degradacao de performance alem dos limites aceitaveis
- Problemas de integridade de dados detectados
- Vulnerabilidades de seguranca introduzidas
- Erros user-facing excedendo limites de alerta

### Rollback Procedures

#### Phase 1 Rollback
- **Action:** Descartar branch de discovery, restaurar estado anterior da documentacao
- **Data Impact:** Nenhum (sem mudancas em producao)
- **Estimated Time:** < 1 hora

#### Phase 2 Rollback
- **Action:** {{TODO: Reverter commits, restaurar banco para snapshot pre-migracao}}
- **Data Impact:** {{TODO: Descreva perda de dados ou preocupacoes de consistencia}}
- **Estimated Time:** {{TODO: ex. 2-4 horas}}

#### Phase 3 Rollback
- **Action:** {{TODO: Rollback completo de deploy, restaurar versao anterior}}
- **Data Impact:** {{TODO: Documente requisitos de sincronizacao de dados}}
- **Estimated Time:** {{TODO: ex. 1-2 horas}}

### Post-Rollback Actions
1. Documentar razao do rollback em incident report
2. Notificar stakeholders sobre rollback e impacto
3. Agendar post-mortem para analisar a falha
4. Atualizar plano com licoes aprendidas antes de nova tentativa

## Evidence & Follow-up

> Liste artefatos a coletar (logs, PR links, test runs, design notes).
> Registre acoes de follow-up e responsaveis.

| Artifact | Type | Link / Location | Owner |
| --- | --- | --- | --- |
| {{TODO: ex. PR de implementacao}} | Pull Request | {{TODO: link}} | {{TODO: responsavel}} |
| {{TODO: ex. Resultado de testes}} | Test Report | {{TODO: link}} | {{TODO: responsavel}} |
| {{TODO: ex. Notas de design}} | Document | {{TODO: link}} | {{TODO: responsavel}} |
