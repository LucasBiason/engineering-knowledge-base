# Princípios do Engineering Knowledge Base

Este documento define os princípios fundamentais que guiam a criação, organização e evolução de todo o ecossistema.

---

## Princípio 1: Documentação de Aprendizado Real

> **Você não ensina. Você documenta aprendizado real.**  
> **Você não cria cursos. Você constrói conhecimento versionado.**

### O que isso significa:

- Conteúdo nasce de estudo ativo, não de pesquisa genérica
- Cada notebook/documento reflete entendimento pessoal
- Decisões técnicas são justificadas, não apenas apresentadas
- Erros e correções são documentados

### O que NÃO fazer:

- ❌ Criar conteúdo que parece "curso de XXXXX"
- ❌ Usar linguagem promocional ("aprenda X em Y dias")
- ❌ Gerar conteúdo automaticamente sem revisão
- ❌ Prometer completude que não existe

---

## Princípio 2: Clareza sobre Trade-offs

> **Toda decisão técnica tem custos e benefícios. Documente ambos.**

### O que isso significa:

- Sempre explicar "por que" além de "como"
- Listar alternativas consideradas
- Documentar limitações assumidas
- Ser honesto sobre complexidade

### Exemplos:

- "Usamos YOLO porque precisamos localização precisa, mas isso exige dataset maior"
- "CQRS aumenta complexidade operacional, mas permite escalar leitura e escrita independentemente"

---

## Princípio 3: Tom Técnico Profissional

> **Escreva como engenheiro, não como influenciador.**

### Características do tom:

- **Declarativo:** "Este repositório documenta..."
- **Técnico:** Termos precisos, sem simplificação excessiva
- **Neutro:** Pouca opinião emocional, muita justificativa
- **Pessoal no sentido de autoria:** "Eu implementei", não "você vai aprender"

### Evitar:

- ❌ "Neste tutorial você vai aprender..."
- ❌ "Aprenda X do zero!"
- ❌ Emojis excessivos (apenas em documentação quando apropriado)
- ❌ Linguagem de marketing

---

## Princípio 4: Estrutura Consistente

> **Templates reduzem atrito e aumentam qualidade.**

### Padrões obrigatórios:

- **README.md:** Sempre segue template canônico (8 seções)
- **Notebooks:** Sempre seguem estrutura definida
- **Documentação:** Sempre em `docs/` ou equivalente
- **Código:** Sempre comentado e testado quando possível

### Benefícios:

- Facilita navegação
- Reduz decisões desnecessárias
- Cria "cheiro de senioridade"

---

## Princípio 5: Evolução Contínua

> **Nada nasce completo. Tudo cresce incrementalmente.**

### O que isso significa:

- Projetos começam estruturados, não completos
- Conteúdo é adicionado gradualmente
- Refatoração é parte do processo
- Status é sempre explícito ("em desenvolvimento", "completo", "arquivado")

### Mensagem implícita:

> "Isso é um trabalho contínuo, não um produto fechado."

---

## Princípio 6: Conexões Explícitas

> **Cada componente sabe seu lugar no sistema maior.**

### Como aplicar:

- READMEs linkam para outros KBs
- Projetos referenciam conceitos dos KBs
- Engineering Knowledge Base serve como hub central
- Nada vive isolado

### Exemplo:

No README do Microservices KB:
```markdown
## Relação com o Ecossistema

Este repositório faz parte do Engineering Knowledge Base.

- **Base teórica para:** CQRS Architecture Lab
- **Conecta com:** Programming KB (algoritmos de grafos)
- **Aplica em:** Threat Modeling AI (STRIDE)
```

---

## Princípio 7: Autoria Humana

> **Conteúdo é escrito manualmente, não gerado automaticamente.**

### O que isso significa:

- Zero tolerância para conteúdo gerado por IA sem revisão
- Cada commit representa aprendizado real
- Comentários no código explicam decisões, não apenas funcionamento
- Documentação reflete pensamento, não apenas informação

### Por quê:

- Credibilidade técnica
- Qualidade real
- Aprendizado genuíno

---

## Princípio 8: Escopo Claro

> **Cada repositório tem limites explícitos.**

### Como aplicar:

- README sempre define "o que você vai encontrar" e "o que você NÃO vai encontrar"
- Escopo é declarado claramente
- Não há sobreposição desnecessária entre KBs

### Exemplo:

Programming KB:
- ✅ Algoritmos fundamentais
- ✅ Estruturas de dados
- ✅ Análise de complexidade
- ❌ Frameworks específicos
- ❌ Tutoriais de linguagem

---

## Princípio 9: Qualidade sobre Volume

> **Melhor 2 projetos excelentes do que 7 medianos.**

### Aplicação:

- Preferir profundidade a largura
- Completar um módulo antes de começar outro
- Testar antes de publicar
- Documentar antes de expandir

---

## Princípio 10: Público vs Privado

> **GitHub público mostra resultado, não o caos mental.**

### Regra de ouro:

- **Público:** Conteúdo consolidado, READMEs profissionais, código limpo
- **Privado:** Planejamentos detalhados, rascunhos, regras internas

### Estrutura:

- `docs-private/` para planejamento interno
- `README.md` para apresentação pública
- Commits pequenos e semânticos

---

## Aplicação Prática

Estes princípios guiam:

1. **Criação de novos conteúdos**
2. **Revisão de conteúdo existente**
3. **Decisões de estrutura**
4. **Tom de escrita**
5. **Priorização de tarefas**

---

## Validação

Antes de adicionar qualquer conteúdo, pergunte:

- ✅ Reflete aprendizado real?
- ✅ Explica trade-offs?
- ✅ Tem tom técnico profissional?
- ✅ Segue estrutura padrão?
- ✅ Está conectado ao ecossistema?
- ✅ Foi escrito manualmente?
- ✅ Tem escopo claro?

Se todas as respostas forem "sim", o conteúdo está alinhado com os princípios.

---

*Última atualização: 2025-01-13*

