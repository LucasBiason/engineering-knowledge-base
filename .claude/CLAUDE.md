# Engineering Knowledge Base - Claude

Configuracao do Claude para o projeto Engineering Knowledge Base. Regras de padrao de codigo e comandos para tutoriais e notebooks.

---

## Estrutura

```
.claude/
├── CLAUDE.md
├── rules/          # Padroes de codigo e tutoriais
└── commands/       # Comandos uteis para o KB
```

---

## Commands

| Comando                | Descricao                                                                  |
| ---------------------- | -------------------------------------------------------------------------- |
| `/padronizar_notebook` | Aplicar padrao do KB a um notebook (diagramas, explicacoes, passo a passo) |
| `/gerar_tutorial`      | Gerar tutorial a partir de codigo ou topico                                |
| `/review`              | Revisar codigo/notebook (qualidade, padroes)                               |

---

## Regras Criticas

- **Notebooks:** Tutoriais padronizados com diagramas (Mermaid), explicacoes tecnicas e passo a passo do codigo.
- **Python:** Type hints, Ruff (linter/format), uma classe por arquivo quando aplicavel.
- **Documentacao:** Diagramas via Mermaid para fluxogramas, sequencia, classes; sem emojis em codigo/docs tecnicos.
- **Repositorio publico:** Conteudo mostra apenas o que esta feito; sem cronograma nem planos futuros na ROADMAP publica.

Consultar `rules/programming.md` para detalhes.

## Validacao e status dos projetos de estudo

- **Lista de validacao:** `ROADMAP/03-LISTA-VALIDACAO-KNOWLEDGE-BASE.md` — O que ja esta feito, o que falta fazer e o que precisa ser validado (notebooks contra PADRAO-NOTEBOOKS, revisao de codigo em 07-Projects).
- **Padrao de notebooks (IA/ML):** `Arquitetura e Sistemas/ia-ml-knowledge-base/PADRAO-NOTEBOOKS.md`.
- Ao criar/editar notebooks ou reportar status, usar a lista de validacao e o status consolidado (`ROADMAP/01-STATUS-CONSOLIDADO.md`) como referencia.
