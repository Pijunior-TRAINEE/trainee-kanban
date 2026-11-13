---
titulo: "Exercício final: simulação Pijunópolis"
trilha: "fundamentos (transversal às quatro trilhas)"
nivel: "intermediário"
tempo_estimado: "Leitura de 15 a 20 min; desafio: 60 a 90 min"
pre_requisitos: "Módulos 01 a 05 desta trilha"
autor: "Diretoria de Projetos — Pi Júnior UFMG"
revisor: "Diretoria de Projetos — Pi Júnior UFMG"
atualizado_em: "13/11/2026"
---

# Exercício final: simulação Pijunópolis

## Objetivos de aprendizagem

Ao final do módulo, o trainee será capaz de:

- Extrair User Stories fiéis à fala de um cliente a partir da transcrição de uma reunião.
- Priorizar um backlog justificando a ordem e definir um Sprint Goal.
- Montar o quadro Kanban da primeira sprint e uma Definition of Done para os itens de dashboard.

---

## 1. Mapa do conceito

### O que é

É um ensaio geral. Você recebe a transcrição de uma primeira reunião com uma cliente e percorre todo o caminho, do pedido até a primeira sprint: User Stories, backlog, Sprint Goal, quadro e Definition of Done. Como num ensaio de teatro, os conceitos já foram estudados; aqui é a primeira vez que aparecem juntos, com uma cliente “de mentira”.

### Por que importa na Pi Júnior

No Projeto 2 (trilha de chatbots e agentes de IA), você vai conduzir uma reunião diagnóstica simulada e executar uma sprint com Kanban. O cenário de Pijunópolis, um dashboard de disponibilidade de hotéis alimentado por coleta de dados, também conversa com a trilha de dashboards do Projeto 1.

### Como se conecta com o resto

- **Vem antes:** Todos os módulos anteriores, em especial [Do pedido do cliente ao backlog](modulo-05-do-pedido-ao-backlog.md).
- **Vem depois:** Projetos práticos das semanas 4 e 5.

### Vocabulário-chave

| Termo | O que significa (em uma linha) |
|---|---|
| User Story | Necessidade descrita do ponto de vista de quem usa: Como / Quero / Para. |
| Critério de aceite | Condição verificável que diz quando uma story está satisfeita. |
| Backlog priorizado | Itens ordenados pelo valor que entregam. |
| Sprint Goal | Frase que resume o objetivo da sprint. |
| Quadro Kanban | Colunas por etapa do fluxo, com cartões e limite de WIP. |
| Definition of Done | Padrão de qualidade que todo item do time precisa cumprir. |

---

## 2. Mínimo para começar

### O essencial

- **Stories:** formato Como / Quero / Para, checadas pelo INVEST (módulo 05).
- **Priorização:** o que destrava a decisão de negócio mais cedo vem primeiro, e a ordem deve ser justificada em uma frase.
- **Sprint Goal:** uma frase com o resultado da primeira sprint (módulo 05).
- **Quadro:** colunas por etapa do fluxo, limite de WIP e cartões de exemplo (módulos 03 e 04).
- **Definition of Done:** critérios objetivos e verificáveis; não confunda com critério de aceite (módulo 04).
- **Fonte única:** a transcrição é a sua única fonte de informação sobre a cliente.

### Preparação do ambiente

Crie um projeto vazio no GitHub Projects para montar o quadro da Sprint 1 (veja o módulo 03).

**Como conferir que deu certo:** O projeto abre na visão Board e aceita a criação de um cartão. Se algo falhar, repita a preparação do módulo 03.

### Referências curadas

| Recurso | Tipo | Idioma | Tempo | O que aproveitar |
|---|---|---|---|---|
| [Guia do Scrum 2020 (pt-BR)](https://scrumguides.org/docs/scrumguide/v2020/2020-Scrum-Guide-Portuguese-BR.pdf) | documentação oficial | pt | 15 min | Trechos sobre Product Backlog, Sprint Goal e Definição de Pronto. |
| [User Stories, da Atlassian](https://www.atlassian.com/agile/project-management/user-stories) | tutorial | en | 15 min | Revise o formato e os exemplos antes de escrever as suas. |
| [Quickstart for Projects, GitHub Docs](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/quickstart-for-projects) | documentação oficial | en | 20 min | Como criar e organizar cartões no quadro. |

### Estou pronto para o desafio?

- [ ] Consigo explicar com minhas palavras o que o mapa do conceito descreve.
- [ ] Meu ambiente está funcionando (verificação acima).
- [ ] Sei onde consultar a documentação oficial quando travar.

---

## 3. Desafio aberto

### Contexto

Você é a pessoa mais nova do time. O Gerente de Projetos, Marcos, teve uma primeira reunião com uma nova cliente, Helena, dona de uma agência de turismo receptivo em **Pijunópolis**, uma cidade litorânea fictícia. Nessa reunião, Marcos atuou tanto como Scrum Master quanto como Product Owner. A transcrição abaixo é a sua única fonte de informação.

??? note "Transcrição da reunião (clique para abrir)"

    **Participantes:** Marcos (Gerente de Projetos, atuando como Scrum Master e Product Owner) e Helena (cliente, proprietária de uma agência de turismo receptivo em Pijunópolis)

    **Marcos:** Bom dia, Helena! Obrigado por reservar um tempo. Antes de começarmos a desenhar a solução, eu queria entender melhor o problema que você está tentando resolver. Pode me contar o que motivou esse pedido?

    **Helena:** Bom dia, Marcos! Aqui em Pijunópolis a gente tem mais de 40 hotéis e pousadas, e hoje eu preciso ligar ou mandar mensagem pra cada um pra saber quantos quartos estão disponíveis em determinada época do ano. É um trabalho manual enorme, e muitas vezes a informação já está desatualizada quando eu preciso decidir alguma coisa.

    **Marcos:** Entendi. E o que você faz com essa informação depois que consegue? Qual é a decisão que ela ajuda a tomar?

    **Helena:** Eu uso pra decidir pra quais hotéis eu direciono os grupos de turistas que trago pra cidade, principalmente na alta temporada. Se eu soubesse rápido quais hotéis têm vaga e a que preço, conseguiria negociar melhor e fechar pacotes mais rápido.

    **Marcos:** Perfeito, isso já ajuda bastante. Então o objetivo final não é só “ter os dados dos hotéis” — é conseguir tomar uma decisão de alocação e negociação mais rápido. Você imagina algum painel, alguma tela, onde bateria o olho e já veria isso?

    **Helena:** Isso, exatamente! Um dashboard. Eu queria ver, por exemplo, quantos hotéis têm disponibilidade numa faixa de datas, quais as faixas de preço e, se possível, ver isso organizado por região da cidade — porque a região perto da praia é bem diferente da região mais afastada.

    **Marcos:** Show. E hoje, de onde vem essa informação? Os hotéis têm algum sistema, uma planilha, ou é tudo por telefone mesmo?

    **Helena:** Depende muito. Os hotéis maiores têm sistema próprio, mas a maioria das pousadas menores só responde por WhatsApp ou telefone. Não tem padrão nenhum.

    **Marcos:** Isso é importante — significa que, no começo, provavelmente vamos precisar de uma forma manual ou semi-manual de coletar essa informação. Não dá pra prometer uma integração automática com todos os hotéis logo de cara.

    **Helena:** Faz sentido. Eu só preciso que comece a funcionar o quanto antes, mesmo que não seja perfeito. A temporada de verão começa em dois meses e meio.

    **Marcos:** Combinado. Nosso primeiro objetivo vai ser ter uma versão simples funcionando, e ir evoluindo. Só pra alinhar expectativa: vamos trabalhar em ciclos curtos, chamados sprints, de duas semanas. A cada duas semanas eu te mostro o que foi feito, você me dá feedback, e a gente ajusta o rumo.

    **Helena:** Gostei disso, prefiro ir vendo aos poucos mesmo.

    **Marcos:** Ótimo. Só mais algumas perguntas pra montar o plano de trabalho. Quantas pessoas do seu time vão usar esse dashboard?

    **Helena:** Só eu e minha sócia, por enquanto.

    **Marcos:** E teria algum limite de orçamento além do prazo da alta temporada que eu deveria saber?

    **Helena:** O orçamento é enxuto, então prefiro algo simples que funcione a algo bonito e caro. E o prazo mesmo é a alta temporada — dois meses e meio.

    **Marcos:** Entendido. Última pergunta: como você imagina que os dados de disponibilidade vão chegar até nós no dia a dia? Alguém vai digitar isso em algum lugar?

    **Helena:** Eu tinha pensado que talvez minha assistente pudesse ligar toda semana pros hotéis e preencher uma planilha ou formulário simples, e depois isso alimentasse o painel.

    **Marcos:** Perfeito, isso resolve o problema de coleta pro início do projeto. Vou organizar tudo isso em itens de trabalho. E já te aviso: nas próximas semanas você vai me ver perguntando bastante, porque quanto mais eu entender do seu negócio, melhor vai ficar o painel. Combinado?

    **Helena:** Combinado, pode contar comigo!

### Enunciado

A partir da transcrição, entregue: uma lista de User Stories (Como / Quero / Para); um backlog priorizado, com uma frase justificando a ordem; um Sprint Goal para a primeira sprint; a estrutura de um quadro Kanban para a Sprint 1, com colunas e pelo menos 4 cartões de exemplo distribuídos entre elas; e uma Definition of Done para os itens relacionados ao dashboard.

### Requisitos e restrições

- Todas as User Stories estão no formato Como / Quero / Para e podem ser rastreadas a algo que a cliente disse.
- O backlog tem uma frase justificando a ordem escolhida.
- O quadro tem colunas por etapa do fluxo, limite de WIP e pelo menos 4 cartões distribuídos entre as colunas.
- A Definition of Done tem critérios verificáveis.
- Não existe uma única resposta certa, mas o que está escrito deve refletir o que a cliente disse, e não o que você presumiu.
- Tempo sugerido: 60 a 90 min.

### Pistas

Abra uma pista por vez, só quando estiver realmente travado.

??? tip "Pista 1: por onde começar"

    Releia a transcrição procurando as decisões que Helena precisa tomar e o que hoje a atrapalha.

??? tip "Pista 2: uma ferramenta ou conceito útil"

    Use o INVEST para checar as histórias e lembre que DoD e critério de aceite são coisas diferentes. Para ordenar, pergunte o que destrava o resto.

??? tip "Pista 3: um ponto de atenção"

    Use apenas o que a cliente disse. Releia a parte sobre como os dados chegarão no dia a dia, o orçamento e o prazo antes de ordenar o backlog.

### Critérios de pronto

O desafio está concluído quando:

- [ ] Cada User Story pode ser ligada a um trecho da transcrição.
- [ ] A ordem do backlog está justificada e respeita o pedido explícito da cliente (simples e rápido).
- [ ] O Sprint Goal é uma frase com um resultado verificável.
- [ ] O quadro tem pelo menos 4 colunas e pelo menos 4 cartões.
- [ ] A DoD tem pelo menos 4 critérios que outra pessoa consegue verificar.
- [ ] O trabalho está em uma branch, com commits seguindo a convenção do time.

**Para quem terminar cedo:** Liste três perguntas que você faria a Helena na próxima reunião e que mudariam o backlog.

!!! warning "Gabarito"

    Após abrir o Pull Request com a sua entrega, solicite ao mentor/revisor o gabarito de referência para comparar a sua solução.

---

## 4. Pergunta de pesquisa

### A pergunta

Como priorizar um backlog quando o prazo é fixo e o orçamento é enxuto, e que critérios além do valor ajudam a decidir a ordem?

### Por que essa pergunta

Nos projetos reais da Pi Júnior o prazo e o orçamento costumam ser fixos; escolher bem o que entra primeiro decide se o cliente recebe algo útil a tempo.

### Por onde começar (opcional)

- Palavras-chave para buscar: MoSCoW, MVP, valor versus esforço

### Como responder

Escreva de 3 a 6 linhas na sua nota (seção 5) contendo:

1. a resposta, com suas palavras;
2. as fontes consultadas (com link);
3. se possível, como você testou a resposta na prática.

---
## 5. Entregável documentado

### O que entregar

1. O resultado do desafio, dentro da subpasta `entregaveis/` (e/ou `src/`, quando houver código).
2. Uma **nota em Markdown** com o modelo abaixo, salva em `docs/nota-m06.md`.

**Onde entregar:** no seu **fork** deste repositório, dentro da pasta exclusiva `entregas/<seu-nome>/semana-01/modulo-06/`, abrindo um **Pull Request** para a `main` com título no padrão `feat(s01-m06): entrega <seu-nome>`.

### Estrutura de arquivos da sua entrega

```text
entregas/<seu-nome>/semana-01/modulo-06/
├── docs/                      # Documentação extra, diagramas, esquemas ou notas
│   └── nota-m06.md            # Nota em Markdown com a reflexão e respostas
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