---
titulo: "Do pedido do cliente ao backlog"
trilha: "fundamentos (transversal às quatro trilhas)"
nivel: "intermediário"
tempo_estimado: "Leitura de 15 a 20 min; desafio: 45 a 60 min"
pre_requisitos: "[Módulo 02](modulo-02-scrum-papeis-eventos-artefatos.md) e [Módulo 04](modulo-04-unindo-scrum-e-kanban.md)"
autor: "Diretoria de Projetos — Pi Júnior UFMG"
revisor: "Diretoria de Projetos — Pi Júnior UFMG"
atualizado_em: "13/11/2026"
---

# Do pedido do cliente ao backlog

## Objetivos de aprendizagem

Ao final do módulo, o trainee será capaz de:

- Conduzir uma conversa de levantamento de requisitos seguindo a ordem recomendada.
- Escrever User Stories com critérios de aceite, checando-as com o critério INVEST.
- Priorizar um backlog e definir um Sprint Goal.

---

## 1. Mapa do conceito

### O que é

É o caminho entre o que o cliente diz e o que o time vai construir: entender o problema real, transformar a conversa em itens de trabalho (User Stories), ordená-los por valor e escolher o foco da primeira sprint. Funciona como uma consulta médica: o paciente chega com um pedido (“preciso de um remédio”), mas o bom médico investiga a queixa e o contexto antes de receitar.

### Por que importa na Pi Júnior

No Projeto 2 (trilha de chatbots e agentes de IA), seu time fará uma reunião diagnóstica simulada, em que um membro da empresa faz o papel do cliente, e depois redigirá uma documentação técnica curta. Em consultorias e times pequenos, a pessoa que conduz essa reunião costuma ser a mesma que monta o backlog. O cenário do exercício final, um dashboard de disponibilidade de hotéis, ilustra a trilha de dashboards.

### Como se conecta com o resto

- **Vem antes:** [Scrum: papéis, eventos e artefatos](modulo-02-scrum-papeis-eventos-artefatos.md) e [Unindo Scrum e Kanban](modulo-04-unindo-scrum-e-kanban.md).
- **Vem depois:** [Exercício final: simulação Pijunópolis](modulo-06-simulacao-pijunopolis.md).

### Vocabulário-chave

| Termo | O que significa (em uma linha) |
|---|---|
| Requisito | Necessidade do cliente que a solução precisa atender. |
| User Story | Descrição de uma necessidade do ponto de vista de quem vai usar: Como / Quero / Para. |
| Critério de aceite | Condição clara e verificável que define quando uma User Story está satisfeita. |
| INVEST | Checklist de uma boa User Story: Independente, Negociável, de Valor, Estimável, pequena (*Small*) e Testável. |
| Backlog priorizado | Lista de itens ordenada pelo valor que entregam. |
| Sprint Goal | Frase que resume o que a primeira sprint deve alcançar. |

---

## 2. Mínimo para começar

### O essencial

- **SM + PO:** em times pequenos, o gerente de projetos costuma acumular os dois papéis; quem conduz a reunião com o cliente é quem depois monta o backlog.
- **Ordem da conversa com o cliente:** o problema real (e não só o pedido literal); a decisão que isso vai ajudar a tomar; como as coisas funcionam hoje; as restrições (prazo, orçamento, quem usa); como o processo vai funcionar dali em diante (ciclos curtos, com feedback constante).
- **User Story:** “Como [papel], quero [ação], para [benefício]”. O foco está no valor para quem usa, e não em como a solução será construída.
- **Critério INVEST:** a história deve ser Independente, Negociável, ter Valor claro, ser Estimável, pequena (*Small*) e Testável.
- **Erro comum:** tarefa técnica disfarçada de story, como “Como desenvolvedor, quero programar o backend”.
- **Critérios de aceite:** toda story tem um ou mais; sem eles, “pronto” vira questão de opinião.
- **Do backlog ao Sprint Goal:** priorize o que traz mais valor primeiro (especialmente com prazo apertado) e resuma a primeira sprint em uma frase.

Três exemplos de User Story, em contextos diferentes:

| Contexto | User Story | Critério de aceite |
|----------|------------|--------------------|
| E-commerce | Como cliente de uma loja online, quero receber uma notificação quando meu pedido for despachado, para saber quando esperar a entrega. | O cliente recebe um e-mail em até 1 hora após o despacho. |
| Aplicativo bancário | Como usuário do aplicativo do banco, quero bloquear meu cartão pelo próprio app, para evitar fraude caso eu o perca. | O cartão é bloqueado em tempo real, sem precisar ligar para o banco. |
| Turismo | Como agente de turismo, quero ver a disponibilidade de hotéis organizada por faixa de preço, para negociar pacotes com mais agilidade. | O dashboard mostra pelo menos 3 faixas de preço configuráveis. |

### Preparação do ambiente

Nada a instalar. Basta um editor de Markdown.

**Como conferir que deu certo:** Escreva uma User Story no formato Como / Quero / Para sobre algo do seu dia a dia. O resultado esperado é uma frase que descreve valor para quem usa, sem citar como será construído.

### Referências curadas

| Recurso | Tipo | Idioma | Tempo | O que aproveitar |
|---|---|---|---|---|
| [User Stories, da Atlassian](https://www.atlassian.com/agile/project-management/user-stories) | tutorial | en | 15 min | Formato da story e exemplos; use para comparar com os exemplos da tabela. |
| [INVEST in Good Stories, and SMART Tasks (Bill Wake)](https://xp123.com/articles/invest-in-good-stories-and-smart-tasks/) | artigo | en | 15 min | Origem do critério INVEST; leia a explicação de cada letra. |
| [Guia do Scrum 2020 (pt-BR)](https://scrumguides.org/docs/scrumguide/v2020/2020-Scrum-Guide-Portuguese-BR.pdf) | documentação oficial | pt | 10 min | Trechos sobre o Product Backlog e o Sprint Goal. |

### Autoteste rápido

Tente responder antes de abrir as respostas.

1. **Transforme em User Story:** o cliente disse “eu preciso saber quando alguém abandona o carrinho de compras no meu site”.

    ??? success "Confira"
        Exemplo: “Como dono de e-commerce, quero ser notificado quando um cliente abandona o carrinho, para tentar recuperar a venda.”

2. **Complemente:** escreva um critério de aceite para a User Story que você acabou de criar.

    ??? success "Confira"
        Exemplo: “O sistema envia um e-mail automático em até 1 hora após o abandono.”

3. **Liste duas perguntas** que você faria antes de aceitar um pedido de funcionalidade de um cliente, sem tentar adivinhar o que ele quis dizer.

    ??? success "Confira"
        Resposta livre. Bons exemplos: “que decisão isso vai ajudar a tomar?” e “como isso funciona hoje, sem essa funcionalidade?”

### Estou pronto para o desafio?

- [ ] Consigo explicar com minhas palavras o que o mapa do conceito descreve.
- [ ] Meu ambiente está funcionando (verificação acima).
- [ ] Sei onde consultar a documentação oficial quando travar.

---

## 3. Desafio aberto

### Contexto

O dono de uma padaria fictícia, a Padaria Pão & Cia, mandou uma mensagem curta: “Preciso de um robô no WhatsApp que organize as encomendas de bolo”. Você é quem vai conduzir a reunião diagnóstica e montar o backlog.

### Enunciado

Entregue o preparo do projeto: um roteiro de reunião diagnóstica, quatro User Stories com critérios de aceite (marcando as suposições que precisariam ser confirmadas com o cliente), um backlog ordenado com uma frase por item e um Sprint Goal.

### Requisitos e restrições

- O roteiro tem pelo menos 6 perguntas, na ordem em que você as faria, e cobre as cinco frentes do levantamento de requisitos.
- Pelo menos 4 User Stories no formato Como / Quero / Para, cada uma com critério de aceite.
- As suposições que você precisou fazer estão marcadas como “a confirmar”.
- Backlog ordenado, com uma frase justificando cada posição.
- Sprint Goal em uma frase.
- Tempo sugerido: 45 a 60 min.

### Pistas

Abra uma pista por vez, só quando estiver realmente travado.

??? tip "Pista 1: por onde começar"

    Antes de escrever qualquer história, pergunte-se: o que o dono da padaria vai decidir ou fazer de diferente quando esse robô existir?

??? tip "Pista 2: uma ferramenta ou conceito útil"

    Use o critério INVEST como checklist para cada história e o formato Como / Quero / Para.

??? tip "Pista 3: um ponto de atenção"

    “Como desenvolvedor, quero…” não é uma User Story. E perguntas que sugerem a resposta (“você quer um menu de opções, né?”) escondem o problema real.

### Critérios de pronto

O desafio está concluído quando:

- [ ] As perguntas do roteiro cobrem problema, decisão, situação atual, restrições e processo de trabalho.
- [ ] Cada User Story descreve valor para quem usa, e não uma tarefa técnica.
- [ ] Cada critério de aceite pode ser verificado por outra pessoa sem perguntar ao autor.
- [ ] O Sprint Goal descreve um resultado, não uma lista de tarefas.
- [ ] O trabalho está em uma branch, com commits seguindo a convenção do time.

**Para quem terminar cedo:** Simule a reunião com um colega da turma que faz o papel do cliente, depois ajuste as histórias e registre o que mudou.

---

## 4. Pergunta de pesquisa

### A pergunta

Como saber se uma User Story é pequena o suficiente para caber em uma sprint, e o que fazer quando ela é grande demais?

### Por que essa pergunta

No Projeto 2 o time tem uma semana de sprint; histórias grandes demais fazem a sprint terminar sem nada entregue.

### Por onde começar (opcional)

- Palavras-chave para buscar: divisão de User Stories, épico, fatia vertical

### Como responder

Escreva de 3 a 6 linhas na sua nota (seção 5) contendo:

1. a resposta, com suas palavras;
2. as fontes consultadas (com link);
3. se possível, como você testou a resposta na prática.

---
## 5. Entregável documentado

### O que entregar

1. O resultado do desafio, dentro da subpasta `entregaveis/` (e/ou `src/`, quando houver código).
2. Uma **nota em Markdown** com o modelo abaixo, salva em `docs/nota-m05.md`.

**Onde entregar:** no seu **fork** deste repositório, dentro da pasta exclusiva `entregas/<seu-nome>/semana-01/modulo-05/`, abrindo um **Pull Request** para a `main` com título no padrão `feat(s01-m05): entrega <seu-nome>`.

### Estrutura de arquivos da sua entrega

```text
entregas/<seu-nome>/semana-01/modulo-05/
├── docs/                      # Documentação extra, diagramas, esquemas ou notas
│   └── nota-m05.md            # Nota em Markdown com a reflexão e respostas
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
