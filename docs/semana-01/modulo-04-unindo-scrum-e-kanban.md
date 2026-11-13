---
titulo: "Unindo Scrum e Kanban"
trilha: "fundamentos (transversal às quatro trilhas)"
nivel: "iniciante"
tempo_estimado: "Leitura de 15 a 20 min; desafio: 40 a 60 min"
pre_requisitos: "[Módulo 02](modulo-02-scrum-papeis-eventos-artefatos.md) e [Módulo 03](modulo-03-kanban-na-pratica.md)"
autor: "Diretoria de Projetos — Pi Júnior UFMG"
revisor: "Diretoria de Projetos — Pi Júnior UFMG"
atualizado_em: "13/11/2026"
---

# Unindo Scrum e Kanban

## Objetivos de aprendizagem

Ao final do módulo, o trainee será capaz de:

- Descrever como um quadro Kanban funciona dentro de uma sprint Scrum.
- Aplicar as boas práticas de quem usa Kanban dentro do Scrum.
- Distinguir Definition of Done de Critério de Aceite e escrever uma Definition of Done verificável.

---

## 1. Mapa do conceito

### O que é

Usar Scrum e Kanban juntos significa ter **um quadro Kanban por sprint**: as colunas são as etapas do fluxo e os cartões são os itens do Sprint Backlog. A **Definition of Done (DoD)** é o combinado do time sobre o que significa “pronto”. Na cozinha do restaurante, é a diferença entre “o prato foi cozido” e “o prato foi temperado, provado e está na bancada”: sem esse combinado, cada pessoa tem uma ideia diferente de terminado.

### Por que importa na Pi Júnior

No Projeto 2 (trilha de chatbots e agentes de IA), seu time conduzirá uma sprint de uma semana com Kanban e entregará um chatbot via Docker. A avaliação de qualidade técnica olha justamente se o código é legível e reprodutível (README, pyproject.toml/uv.lock, Docker), e o Code Review dos Pull Requests só faz sentido se o time combinou antes o que significa “pronto”.

### Como se conecta com o resto

- **Vem antes:** [Scrum: papéis, eventos e artefatos](modulo-02-scrum-papeis-eventos-artefatos.md) e [Kanban na prática](modulo-03-kanban-na-pratica.md).
- **Vem depois:** [Do pedido do cliente ao backlog](modulo-05-do-pedido-ao-backlog.md).

### Vocabulário-chave

| Termo | O que significa (em uma linha) |
|---|---|
| Scrumban | Combinação do ritmo do Scrum com o quadro de fluxo do Kanban. |
| Quadro da sprint | Quadro Kanban cujos cartões são os itens do Sprint Backlog. |
| WIP | Limite de cartões em andamento ao mesmo tempo em uma coluna. |
| Definition of Done (DoD) | Padrão de qualidade único que vale para todos os itens do time. |
| Critério de aceite | Condições específicas de uma única User Story. |
| Sprint Backlog | Itens que o time se comprometeu a entregar na sprint. |

---

## 2. Mínimo para começar

### O essencial

- **Um quadro por sprint:** as colunas representam as etapas do fluxo e os cartões são os itens do Sprint Backlog (exemplo na tabela abaixo).
- **Boas práticas:** atualizar o quadro na Daily; respeitar o limite de WIP; escrever cartões claros, com critério de aceite; mover em vez de acumular.
- **Definition of Done:** lista de critérios que qualquer item precisa cumprir para estar realmente pronto, e não só “codado”. É combinada pelo time e pelo Scrum Master no início do projeto e pode evoluir.
- **DoD x Critério de aceite:** a DoD é um padrão único, que vale para *todos* os itens; o critério de aceite vale para *uma única* User Story (ex.: “o sistema envia um e-mail em até 1 hora”).

Um quadro no meio de uma sprint:

| Backlog da Sprint | Fazendo (WIP: 2) | Em Validação | Concluído |
|-------------------|------------------|--------------|-----------|
| Configurar ambiente | Criar formulário de coleta | Modelar estrutura de dados | Levantar requisitos com cliente |
| Documentar API | Ajustar layout do dashboard | | |

Três exemplos de DoD, em contextos diferentes:

| Contexto | Exemplo de DoD |
|----------|----------------|
| Desenvolvimento de software | Código revisado por outra pessoa do time, testes automatizados passando, sem bugs críticos conhecidos, disponível na branch principal |
| Design de uma tela | Protótipo aprovado pelo PO, testado em pelo menos dois tamanhos de tela, seguindo o guia visual da marca |
| Tratamento de dados | Dados conferidos com a fonte original, sem duplicidade, atualizados na última semana, carregando no dashboard sem erro |

### Preparação do ambiente

Reaproveite o quadro do GitHub Projects criado no módulo 03.

**Como conferir que deu certo:** Seu quadro tem colunas de fluxo e você consegue criar um cartão novo e movê-lo de coluna. Se ainda não criou o quadro, volte à preparação do módulo 03.

### Referências curadas

| Recurso | Tipo | Idioma | Tempo | O que aproveitar |
|---|---|---|---|---|
| [Guia do Scrum 2020 (pt-BR)](https://scrumguides.org/docs/scrumguide/v2020/2020-Scrum-Guide-Portuguese-BR.pdf) | documentação oficial | pt | 15 min | Trecho sobre os compromissos dos artefatos, em especial a Definição de Pronto. |
| [What is a Definition of Done?, Scrum.org](https://www.scrum.org/resources/what-definition-done) | artigo | en | 10 min | Compare a definição com os exemplos de DoD do módulo. |
| [Quickstart for Projects, GitHub Docs](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/quickstart-for-projects) | tutorial | en | 20 min | Revisite como mover e descrever cartões no quadro. |

### Autoteste rápido

Tente responder antes de abrir as respostas.

1. **Escreva você mesmo:** crie uma Definition of Done para a tarefa “Criar formulário de cadastro de cliente”.

    ??? success "Confira"
        Resposta livre. Compare com os exemplos de DoD; o importante é ter critérios objetivos e verificáveis.

2. **Cenário:** a coluna “Fazendo” tem WIP limite 2 e já tem 2 cartões nela. Chega uma tarefa urgente. O que fazer, seguindo as boas práticas de Kanban?

    ??? success "Confira"
        Terminar ou pausar formalmente algo em andamento antes de puxar a nova tarefa, ou negociar a prioridade com o time; nunca simplesmente ignorar o limite.

3. **Verdadeiro ou falso:** a Definition of Done pode variar de pessoa para pessoa dentro do mesmo time.

    ??? success "Confira"
        Falso. A DoD é combinada pelo time inteiro e vale igual para todos.

### Estou pronto para o desafio?

- [ ] Consigo explicar com minhas palavras o que o mapa do conceito descreve.
- [ ] Meu ambiente está funcionando (verificação acima).
- [ ] Sei onde consultar a documentação oficial quando travar.

---

## 3. Desafio aberto

### Contexto

No Projeto 2, seu time de 3 a 4 pessoas vai conduzir uma sprint de uma semana com Kanban para entregar um chatbot. Antes de começar, o time precisa de um quadro e de um combinado sobre o que significa “pronto”.

### Enunciado

Monte, no GitHub Projects, o quadro da Sprint 1 de um chatbot de perguntas frequentes para um cliente fictício, com a Definition of Done do time registrada, e simule a chegada de uma tarefa urgente no meio da sprint com a coluna “Fazendo” cheia.

### Requisitos e restrições

- Quadro com pelo menos 4 colunas que representem etapas do fluxo, com WIP declarado onde fizer sentido.
- Pelo menos 6 cartões com título claro e verificável; pelo menos 2 deles com critério de aceite.
- Definition of Done do time com pelo menos 4 critérios objetivos e verificáveis, registrada no README ou na nota.
- Registro curto (antes e depois) mostrando como o quadro absorveu a tarefa urgente sem estourar o WIP.
- O time é fictício, de 3 pessoas, e a sprint dura uma semana.
- Tempo sugerido: 40 a 60 min.

### Pistas

Abra uma pista por vez, só quando estiver realmente travado.

??? tip "Pista 1: por onde começar"

    Pergunte-se: o que precisa ser verdade para eu mostrar este item ao cliente sem constrangimento?

??? tip "Pista 2: uma ferramenta ou conceito útil"

    DoD e critério de aceite respondem a perguntas diferentes: uma vale para todos os itens, a outra só para um. Veja como o módulo os diferencia.

??? tip "Pista 3: um ponto de atenção"

    “Código de qualidade” não é um critério verificável: outra pessoa precisa conseguir dizer sim ou não. E a urgência negocia com o WIP, não o ignora.

### Critérios de pronto

O desafio está concluído quando:

- [ ] Cada coluna do quadro representa uma etapa do fluxo.
- [ ] A DoD tem pelo menos 4 critérios que outra pessoa consegue verificar sem perguntar ao autor.
- [ ] Pelo menos 2 cartões trazem critério de aceite específico.
- [ ] O registro da tarefa urgente mostra o que saiu, parou ou foi negociado para respeitar o WIP.
- [ ] O trabalho está em uma branch, com commits seguindo a convenção do time.

**Para quem terminar cedo:** Acrescente uma coluna Bloqueado e escreva a regra do time para cartões bloqueados por mais de um dia.

---

## 4. Pergunta de pesquisa

### A pergunta

Como um time decide o que entra na sua Definition of Done, e o que muda quando ela é rígida demais ou frouxa demais?

### Por que essa pergunta

No Projeto 2 o time precisa combinar o “pronto” antes do primeiro Pull Request; uma DoD mal calibrada trava a sprint ou gera retrabalho no Code Review.

### Por onde começar (opcional)

- Palavras-chave para buscar: Definition of Done, dívida técnica, retrospectiva

### Como responder

Escreva de 3 a 6 linhas na sua nota (seção 5) contendo:

1. a resposta, com suas palavras;
2. as fontes consultadas (com link);
3. se possível, como você testou a resposta na prática.

---
## 5. Entregável documentado

### O que entregar

1. O resultado do desafio, dentro da subpasta `entregaveis/` (e/ou `src/`, quando houver código).
2. Uma **nota em Markdown** com o modelo abaixo, salva em `docs/nota-m04.md`.

**Onde entregar:** no seu **fork** deste repositório, dentro da pasta exclusiva `entregas/<seu-nome>/semana-01/modulo-04/`, abrindo um **Pull Request** para a `main` com título no padrão `feat(s01-m04): entrega <seu-nome>`.

### Estrutura de arquivos da sua entrega

```text
entregas/<seu-nome>/semana-01/modulo-04/
├── docs/                      # Documentação extra, diagramas, esquemas ou notas
│   └── nota-m04.md            # Nota em Markdown com a reflexão e respostas
├── src/                       # Código-fonte (desafios com código; gerenciado com uv)
│   ├── pyproject.toml         # Dependências do desafio (se houver código)
│   └── main.py                # Script/Entrypoint principal
├── entregaveis/               # Artefatos textuais, diagnósticos, prints ou exports
│   └── .gitkeep
└── README.md                  # Apresentação da entrega e como reproduzir
```

### Observações

- Não altere nenhum arquivo fora de `entregas/<seu-nome>/`.
- O `README.md` da sua entrega deve explicar **como reproduzir** o que foi feito (usando comandos `uv run ...` caso haja código Python).
- O `.gitkeep` serve apenas para o Git versionar pastas vazias; pode ser removido assim que você adicionar arquivos reais na pasta.
- Nomes de arquivos e pastas sempre em minúsculas, sem acentos e sem espaços (use hífen).

### Modelo da nota

````markdown
# [Nome do módulo]: nota de [Seu Nome]

## Contexto
O que eu precisava resolver, em 2 ou 3 frases.

## O que eu fiz
As decisões principais, na ordem em que aconteceram.
Inclua trechos de código ou comandos importantes em blocos com a linguagem indicada.

## O que deu errado e como resolvi
Pelo menos um erro, dúvida ou beco sem saída que encontrei, e como saí dele.

## Resposta à pergunta de pesquisa
Minha resposta, com minhas palavras.

**Fontes:**
- [Título da fonte](link)

## Como reproduzir
Passos para outra pessoa conseguir repetir meu resultado.

## Dúvidas que ficaram
O que ainda não está claro para mim.
````

### Diretrizes para a nota

- **Primeira pessoa e linguagem própria.** Não copie trechos de fontes; resuma e cite o link.
- **Curta:** de 1 a 2 páginas. Clareza vale mais que volume.
- **Mostre o processo**, incluindo erros: eles são a parte mais valiosa da nota.
- **Código em blocos** com a linguagem indicada (` ```python `, ` ```bash `).
- **Nada de segredos:** chaves de API, senhas e tokens nunca entram na nota nem no código.
- **Revise antes de enviar:** releia como se você fosse outra pessoa tentando reproduzir.

### Como a nota é avaliada

| Critério | Em desenvolvimento | Adequado | Excelente |
|----------|--------------------|----------|-----------|
| **Funciona** | O resultado não atende aos critérios de pronto | Atende aos critérios de pronto | Atende e trata casos especiais |
| **Entendimento** | Descreve *o que* fez | Explica *por que* fez | Compara alternativas e justifica a escolha |
| **Pesquisa** | Sem fontes ou fontes fracas | Fontes relevantes citadas | Fontes variadas, comparadas e testadas |
| **Documentação** | Difícil de reproduzir | Outra pessoa consegue reproduzir | Clara, organizada e com erros e aprendizados |
| **Autonomia** | Dependeu de ajuda para avançar | Pediu ajuda após tentar e registrar o que tentou | Resolveu sozinho e ajudou outros |

---

Links verificados em: 13/11/2026
