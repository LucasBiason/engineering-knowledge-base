# Mapa Conceitual do Ecossistema

Este documento apresenta o mapa conceitual completo do Engineering Knowledge Base, mostrando como cada componente se relaciona e qual seu papel no sistema maior.

---

## Visão Macro

```
Engineering Knowledge Base
│
├── Camada 1: Fundamentos
│   ├── Programming Knowledge Base
│   └── Data Science Knowledge Base
│
├── Camada 2: Arquitetura
│   ├── Microservices Knowledge Base
│   └── IA/ML Knowledge Base
│
├── Camada 3: Infraestrutura
│   └── My Local Place
│
└── Camada 4: Aplicação
    ├── CQRS Architecture Lab
    └── Threat Modeling AI
```

---

## Camadas de Conhecimento

### 🧱 Camada 1 — Fundamentos

**Objetivo:** Base sólida de ciência da computação e dados

#### Programming Knowledge Base
- **Papel:** Fundamentos algorítmicos e estruturas de dados
- **Conteúdo:** 25+ algoritmos, análise de complexidade, implementações
- **Público:** Desenvolvedores, estudantes, entrevistas técnicas
- **Conexões:** Base para todos os outros projetos

#### Data Science Knowledge Base
- **Papel:** Manipulação e análise de dados
- **Conteúdo:** NumPy, Pandas, EDA, visualização, projetos práticos
- **Público:** Engenheiros de dados, analistas
- **Conexões:** Pré-requisito para IA/ML KB

---

### 🏗️ Camada 2 — Arquitetura

**Objetivo:** Padrões, decisões e trade-offs em sistemas distribuídos

#### Microservices Knowledge Base
- **Papel:** Arquitetura de sistemas distribuídos
- **Conteúdo:** Patterns, anti-patterns, STRIDE, mensageria, consistência
- **Público:** Sênior, Staff, Tech Lead
- **Conexões:** Base teórica para CQRS Lab

#### IA/ML Knowledge Base
- **Papel:** IA aplicada, não hype
- **Conteúdo:** LLMs, RAG, fine-tuning, pipelines, casos práticos
- **Público:** Engenheiros de IA, produto
- **Conexões:** Usa fundamentos do Data Science KB

---

### 🧰 Camada 3 — Infraestrutura

**Objetivo:** Ferramentas e ambiente de desenvolvimento

#### My Local Place
- **Papel:** Infraestrutura local e observabilidade
- **Conteúdo:** Docker, serviços locais, monitoramento
- **Público:** Desenvolvedores, engenheiros de infra
- **Conexões:** Suporta todos os projetos de desenvolvimento

---

### 🚀 Camada 4 — Aplicação

**Objetivo:** Projetos que materializam conhecimento

#### CQRS Architecture Lab
- **Papel:** Projeto-síntese de arquitetura
- **Conteúdo:** CQRS, Event Sourcing, decisões documentadas
- **Conexões:** 
  - Usa conceitos do Microservices KB
  - Usa infra do My Local Place
  - Apoia-se nos fundamentos do Programming KB

#### Threat Modeling AI
- **Papel:** Aplicação prática de IA + Segurança
- **Conteúdo:** YOLO, STRIDE, visão computacional, pipeline completo
- **Conexões:**
  - Usa YOLO (IA/ML KB)
  - Aplica STRIDE (Microservices KB)
  - Usa algoritmos de grafos (Programming KB)

---

## Fluxo de Aprendizado Recomendado

### Para Iniciantes
1. Programming Knowledge Base (fundamentos)
2. Data Science Knowledge Base (dados)
3. IA/ML Knowledge Base (aplicação)

### Para Sênior/Staff
1. Microservices Knowledge Base (arquitetura)
2. CQRS Architecture Lab (aplicação)
3. Threat Modeling AI (segurança + IA)

### Para Arquitetos
1. Microservices KB (patterns)
2. CQRS Lab (decisões)
3. My Local Place (infra)

---

## Princípios de Organização

1. **Um conceito = um artefato**
   - Um algoritmo → um notebook
   - Um pattern → um documento
   - Uma decisão → um ADR

2. **Templates reduzem atrito**
   - Todos os notebooks seguem padrão
   - Todos os READMEs seguem estrutura

3. **Conexões explícitas**
   - Cada KB linka para os outros
   - Projetos referenciam KBs

4. **Evolução contínua**
   - Nada nasce completo
   - Tudo cresce incrementalmente

---

## Como Contribuir

Este é um ecossistema pessoal, mas a estrutura e padrões podem ser reutilizados.

Para usar como referência:
1. Clone os repositórios de interesse
2. Siga a estrutura documentada
3. Adapte aos seus contextos

---

*Última atualização: 2025-01-13*

