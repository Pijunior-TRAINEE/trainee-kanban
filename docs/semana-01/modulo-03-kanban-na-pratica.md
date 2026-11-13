---
titulo: "Kanban na prática"
trilha: "fundamentos (transversal às quatro trilhas)"
nivel: "iniciante"
tempo_estimado: "Leitura de 15 a 20 min; desafio: 40 a 60 min"
pre_requisitos: "[Módulo 01: Fundamentos do Ágil](modulo-01-fundamentos-do-agil.md); conta no GitHub"
autor: "Diretoria de Projetos — Pi Júnior UFMG"
revisor: "Diretoria de Projetos — Pi Júnior UFMG"
atualizado_em: "13/11/2026"
---

# Kanban na prática

## Objetivos de aprendizagem

Ao final do módulo, o trainee será capaz de:

- Explicar a origem do Kanban e seus três princípios básicos.
- Montar um quadro Kanban com colunas por etapa e limite de trabalho em andamento (WIP).
- Comparar Scrum e Kanban e explicar por que muitas equipes usam os dois juntos.

---

## 1. Mapa do conceito

### O que é

Kanban é um método para **visualizar e controlar o fluxo** de qualquer tipo de trabalho. Nasceu no sistema de produção da Toyota, como forma visual de evitar sobrecarga. Imagine um cozinheiro com dez panelas no fogo ao mesmo tempo: nada fica pronto. O Kanban propõe o contrário: pôr o trabalho à vista num quadro e limitar quantas coisas estão em andamento, para terminar antes de começar.

### Por que importa na Pi Júnior

Na turma do trainee você vai usar um quadro Kanban no GitHub Projects com as colunas Backlog, Em andamento, Bloqueado, Em revisão e Concluído, e com limite de 2 cartões em andamento por pessoa. O planejamento do quadro acontece na segunda e a retrospectiva na sexta; cartões bloqueados por mais de um dia entram na pauta da mentoria. O mesmo quadro será usado nos projetos de dashboards (Projeto 1) e de chatbots e agentes de IA (Projeto 2).

### Como se conecta com o resto

- **Vem antes:** [Fundamentos do Ágil](modulo-01-fundamentos-do-agil.md) e, para o contraste, [Scrum: papéis, eventos e artefatos](modulo-02-scrum-papeis-eventos-artefatos.md).
- **Vem depois:** [Unindo Scrum e Kanban](modulo-04-unindo-scrum-e-kanban.md).

### Vocabulário-chave

| Termo | O que significa (em uma linha) |
|---|---|
| Kanban | Método visual para controlar o fluxo de trabalho. |
| Cartão (*card*) | Representação de uma tarefa no quadro. |
| Quadro | Conjunto de colunas que representam as etapas do fluxo. |
| WIP (*work in progress*) | Número máximo de cartões permitidos ao mesmo tempo em uma coluna. |
| Fluxo | Movimento constante dos cartões, da esquerda para a direita. |
| Gargalo | Ponto do fluxo onde os cartões se acumulam. |
| Scrumban | Uso combinado de Scrum (ritmo) e Kanban (fluxo). |

---

## 2. Mínimo para começar

### O essencial

- **Origem:** o Kanban veio do sistema de produção da Toyota. Diferente do Scrum, não tem sprints, papéis fixos nem reuniões obrigatórias.
- **Visualizar o trabalho:** cada tarefa vira um cartão num quadro, e todo mundo vê o que está sendo feito.
- **Limitar o WIP:** cada coluna tem um número máximo de cartões ao mesmo tempo, para evitar que todos comecem tudo e não terminem nada.
- **Gerenciar o fluxo:** o objetivo é fazer os cartões andarem de forma constante da esquerda para a direita, sem gargalos. Idealmente, o cartão nunca volta para trás.
- **Kanban com Scrum:** o Scrum estrutura o *ritmo* das entregas e o Kanban visualiza o *fluxo* dentro de cada sprint; a combinação se chama **Scrumban**.

Um quadro simples:

| A Fazer | Fazendo (WIP: 2) | Em Revisão | Concluído |
|---------|------------------|------------|-----------|
| Card D | Card B | Card C | Card A |
| Card E | | | |

Scrum x Kanban:

| | Scrum | Kanban |
|---|-------|--------|
| Ciclo | Sprints fixas | Fluxo contínuo |
| Papéis | PO, SM e Time (definidos) | Não define papéis fixos |
| Mudanças no meio do ciclo | Evitadas durante a sprint | Podem entrar a qualquer momento (respeitando o WIP) |
| Ferramenta central | Backlog + reuniões | Quadro visual |

### Preparação do ambiente

Crie um projeto no GitHub Projects com a visão Board, seguindo a documentação oficial listada abaixo. Você vai usá-lo no desafio e, depois, na turma.

**Como conferir que deu certo:** O quadro abre na visão Board com colunas de status, e você consegue criar um cartão e arrastá-lo de uma coluna para outra.

### Referências curadas

| Recurso | Tipo | Idioma | Tempo | O que aproveitar |
|---|---|---|---|---|
| [Quickstart for Projects, GitHub Docs](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/quickstart-for-projects) | documentação oficial | en | 20 min | Siga o passo a passo até ter um quadro com cartões; é a sua preparação de ambiente. |
| [Kanban Guide](https://kanbanguides.org/) | documentação oficial | pt / en | 30 min | Leia as práticas centrais do método; confira no próprio site se há versão em português. |
| [O que é Kanban, da Atlassian](https://www.atlassian.com/agile/kanban) | tutorial | en | 15 min | Seção sobre quadros e limites de WIP; use os exemplos como inspiração para o desafio. |

### Autoteste rápido

Tente responder antes de abrir as respostas.

1. **Diagnóstico:** um cartão está há 10 dias parado em “Fazendo”, coluna com WIP limite 2, e já há outros 2 cartões lá. O que provavelmente está errado?

    ??? success "Confira"
        O WIP está sendo ignorado: o time começou mais tarefas do que consegue terminar ao mesmo tempo.

2. **Na prática:** monte um quadro Kanban de 4 colunas para organizar suas tarefas pessoais desta semana. Quais seriam as colunas?

    ??? success "Confira"
        Não existe resposta única; um exemplo comum é A Fazer / Fazendo / Aguardando Aprovação / Feito.

3. **Verdadeiro ou falso:** Scrum e Kanban não podem ser usados juntos.

    ??? success "Confira"
        Falso. A combinação dos dois é chamada de Scrumban.

### Estou pronto para o desafio?

- [ ] Consigo explicar com minhas palavras o que o mapa do conceito descreve.
- [ ] Meu ambiente está funcionando (verificação acima).
- [ ] Sei onde consultar a documentação oficial quando travar.

---

## 3. Desafio aberto

### Contexto

Para a turma do trainee funcionar, cada pessoa precisa conseguir organizar o próprio trabalho em um quadro sem sobrecarregar a si mesma. Antes de usar o quadro da turma, você vai montar e testar o seu.

### Enunciado

Entregue um quadro Kanban no GitHub Projects com as suas tarefas reais da próxima semana, respeitando um limite de WIP declarado, e um registro de pelo menos três momentos de movimentação dos cartões que mostre onde o fluxo trava.

### Requisitos e restrições

- Quadro com pelo menos 4 colunas que representem etapas do fluxo.
- Pelo menos 8 cartões, cada um com título claro e verificável.
- Limite de WIP declarado no quadro. Descubra se a ferramenta o impõe sozinha ou se ele depende de acordo do time, e registre a conclusão.
- Registro (capturas de tela ou tabela) de pelo menos 3 momentos de movimentação, sem estourar o WIP.
- Uma leitura curta de onde apareceu o gargalo ou o cartão parado e por quê.
- Tempo sugerido: 40 a 60 min.

### Pistas

Abra uma pista por vez, só quando estiver realmente travado.

??? tip "Pista 1: por onde começar"

    Antes de desenhar colunas, pergunte: por quais etapas minhas tarefas passam desde o momento em que surgem até serem entregues?

??? tip "Pista 2: uma ferramenta ou conceito útil"

    O conceito central é o WIP: um limite por coluna, e não uma meta de quantas tarefas fazer. Veja como os exemplos de quadro dos materiais o aplicam.

??? tip "Pista 3: um ponto de atenção"

    Colunas representam etapas do fluxo, não pessoas nem prioridades. E um cartão que não anda há dias é sinal a investigar, não decoração.

### Critérios de pronto

O desafio está concluído quando:

- [ ] As colunas têm nomes que representam etapas do fluxo de trabalho.
- [ ] O limite de WIP está declarado e nenhum dos momentos registrados o ultrapassa.
- [ ] Os cartões são tarefas que outra pessoa conseguiria dizer se estão prontas ou não.
- [ ] A leitura do gargalo aponta um cartão ou coluna concretos.
- [ ] O trabalho está em uma branch, com commits seguindo a convenção do time.

**Para quem terminar cedo:** Acrescente uma coluna Bloqueado e uma regra: cartão bloqueado por mais de um dia vira pauta para conversar com o mentor.

---

## 4. Pergunta de pesquisa

### A pergunta

Como se escolhe o limite de WIP de uma coluna, e o que acontece com o fluxo quando ele é alto demais ou baixo demais?

### Por que essa pergunta

Definir o limite certo no quadro da turma e nos projetos evita tanto a sobrecarga quanto o time ocioso esperando uma etapa.

### Por onde começar (opcional)

- Palavras-chave para buscar: Lei de Little, tempo de ciclo, WIP limit

### Como responder

Escreva de 3 a 6 linhas na sua nota (seção 5) contendo:

1. a resposta, com suas palavras;
2. as fontes consultadas (com link);
3. se possível, como você testou a resposta na prática.

---
## 5. Entregável documentado

### O que entregar

1. O resultado do desafio, dentro da subpasta `entregaveis/` (e/ou `src/`, quando houver código).
2. Uma **nota em Markdown** com o modelo abaixo, salva em `docs/nota-m03.md`.

**Onde entregar:** no seu **fork** deste repositório, dentro da pasta exclusiva `entregas/<seu-nome>/semana-01/modulo-03/`, abrindo um **Pull Request** para a `main` com título no padrão `feat(s01-m03): entrega <seu-nome>`.

### Estrutura de arquivos da sua entrega

```text
entregas/<seu-nome>/semana-01/modulo-03/
├── docs/                      # Documentação extra, diagramas, esquemas ou notas
│   └── nota-m03.md            # Nota em Markdown com a reflexão e respostas
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
