---
name: study-summary-rich
description: Gera resumos didáticos extensos e estruturados de aulas/cursos para cards do Notion. Use ao resumir aulas, apostilas, transcrições ou materiais de estudo para incluir no corpo do card (não apenas no campo Descrição), com flashcards, exemplos de código, diagramas Mermaid, mapa conceitual e perguntas de reforço.
---

# Resumos Didáticos Ricos para Estudos

Ao gerar resumos de aulas, apostilas ou transcrições para cards de estudo no Notion, siga **sempre** esta estrutura completa. O conteúdo vai no **corpo da página** (blocks), não só no campo Descrição.

## Estrutura Obrigatória

### 1. 📝 Resumo Executivo
- Principais conceitos da aula
- Objetivos de aprendizagem (bullet points)

### 2. 🧠 Conceitos-Chave (5–8 flashcards)
Formato: **Pergunta → Resposta**
- P: O que é [conceito]?
- R: [Definição clara + exemplo prático quando couber]

### 3. 💻 Exemplos Práticos
- 2–3 exemplos de código (Python, JS, etc.) **comentados** e executáveis
- Foco em aplicações reais do que foi ensinado
- Código deve ser testável

### 4. 🗺️ Mapa Conceitual
```
Tema Principal
├── Subtema 1
│   ├── Conceito A
│   └── Conceito B
└── Subtema 2
    ├── Aplicação X
    └── Aplicação Y
```

### 5. 🧪 Receita Prática
- **Como fazer:** [técnica/metodologia]
1. Passo 1: [descrição clara]
2. Passo 2: [descrição clara]
3. Passo 3: [descrição clara]

### 6. 📊 Diagrama (quando aplicável)
- Usar sintaxe Mermaid (flowchart, sequenceDiagram, etc.)
- Exemplo: `flowchart TD` com nós e arestas

### 7. ❓ Perguntas para Teste de Reforço
- 5–10 perguntas objetivas ou dissertativas curtas
- Respostas breves ao final (ou em toggle)

## Estrutura de Pastas (Full Cycle)

Ao trabalhar com materiais da Engenharia de Computação com IA, use:

```
Apostilas e Materiais de Cursos/[Full Cycle] Engenharia de Computação com IA/
└── Módulo XX - Nome do Módulo/
    ├── Materiais/     # PDFs, slides
    ├── Resumos/       # .md (backup local)
    └── Transcrições/  # .txt
```

Ex.: `Módulo 01 - Fundamentos de IA Generativa/Materiais/Fundamentos de IA Generativa.pdf`

## Regras de Seções e Cards (Notion Studies)

### Seções (OBRIGATÓRIO)
- **Tipo:** sempre `Seção`.
- **Período (obrigatório):** sempre preencher. A data/hora de **início** é igual ao **início da primeira aula**; a data/hora de **fim** é igual ao **fim da última aula**.
  - Exemplo: se a primeira aula começa 2026-02-04 18:47 e a última termina 2026-02-04 20:46, Período = 2026-02-04T18:47:00 até 2026-02-04T20:46:00 (ISO-8601 com timezone).
- **Resumo completo:** quando todas as aulas da seção estiverem concluídas, preencher o **corpo do card da seção** com resumo unificado de todas as aulas (visão geral da seção).

### Aulas
- **Tipo:** sempre `Aula`.
- **Período:** data/hora de início e fim daquela aula específica.

### Implementação
- Ao criar/atualizar **seções** programaticamente: `periodo={"start": "<início_primeira_aula_ISO>", "end": "<fim_última_aula_ISO>"}` com horário (ISO-8601). Nunca deixar seção sem Período.
- Ao usar `update_page` direto: `"Período": build_date_property(inicio_primeira_aula, fim_ultima_aula)`.

## Regras Críticas

1. **Não simplifique** – inclua todo o conteúdo relevante: citações do professor, explicações, anotações e exemplos do material original.
2. **Corpo do card** – o resumo completo vai em blocks (parágrafos, headings, código, listas) no Notion, não só em Descrição.
3. **Código real** – se a aula tiver código ou pseudocódigo, reproduza com comentários explicativos.
4. **Diagramas** – sempre que houver fluxo, arquitetura ou relação entre conceitos, use Mermaid.
5. **Flashcards** – formato fixo P/R para uso em cartões didáticos ou Anki.
6. **Idioma** – manter o idioma do material (PT-BR ou EN conforme o curso).

## Formato de Entrega para Notion

O conteúdo deve ser convertido em blocks da API Notion:
- `heading_1`, `heading_2`, `heading_3` para títulos
- `paragraph` para texto
- `bulleted_list_item` / `numbered_list_item` para listas
- `code` com `language` (python, javascript, mermaid) para trechos de código
- `callout` para destaques e citações do professor
- `quote` para falas ou trechos importantes
- `divider` para separação visual

## Referência do Template Original

```
Atue como tutor de IA e Programação, com foco didático e prático para desenvolvedores.
Estrutura: Resumo Executivo | Conceitos-Chave (flashcards) | Exemplos Práticos |
Mapa Conceitual | Receita Prática | Diagrama Mermaid | Perguntas de Reforço.
Inclua TODO o conteúdo, código, anotações e explicações do professor.
```
