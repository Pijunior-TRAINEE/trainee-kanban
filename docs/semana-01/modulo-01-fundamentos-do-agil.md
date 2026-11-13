---
titulo: "Fundamentos do Ágil"
trilha: "fundamentos (transversal às quatro trilhas)"
nivel: "iniciante"
tempo_estimado: "Leitura de 15 a 20 min; desafio: 30 a 45 min"
pre_requisitos: "nenhum para ler e fazer o desafio; para entregar via Pull Request, o básico de Git/GitHub (módulo de versionamento da Semana 1)"
autor: "Diretoria de Projetos — Pi Júnior UFMG"
revisor: "Diretoria de Projetos — Pi Júnior UFMG"
atualizado_em: "13/11/2026"
---

# Fundamentos do Ágil

## Objetivos de aprendizagem

Ao final do módulo, o trainee será capaz de:

- Explicar, com suas palavras, o problema que o Ágil resolve em relação ao modelo cascata.
- Resumir os quatro valores do Manifesto Ágil e a regra de leitura “o lado direito não é descartado”.
- Situar o Scrum como o framework que coloca a filosofia ágil em prática.

---

## 1. Mapa do conceito

### O que é

Ágil é um jeito de conduzir projetos em que você entrega pedaços pequenos e frequentes, recolhe feedback de verdade e ajusta o rumo ao longo do caminho, em vez de planejar tudo de uma vez e só mostrar o resultado no final. É a diferença entre construir uma casa inteira a partir da planta e entregar a chave no último dia, e entregar um cômodo por vez perguntando ao morador se está do jeito que ele imaginou. O modelo tradicional, a **cascata** (*waterfall*), é o primeiro caso.

### Por que importa na Pi Júnior

Os projetos da Pi Júnior (chatbots, dashboards, scraping e agentes de IA) costumam ter clientes que só entendem o que querem quando veem algo funcionando; descobrir isso apenas no final sai caro. Esse modo de pensar é a base do próprio programa de trainee: quadro Kanban semanal na turma e, no Projeto 2 (trilha de chatbots e agentes de IA), uma sprint de uma semana com cliente fictício.

### Como se conecta com o resto

- **Vem antes:** nenhum; este é o primeiro módulo da trilha de metodologia.
- **Vem depois:** [Scrum: papéis, eventos e artefatos](modulo-02-scrum-papeis-eventos-artefatos.md).

### Vocabulário-chave

| Termo | O que significa (em uma linha) |
|---|---|
| Cascata (*waterfall*) | Modelo em que se planeja tudo no início e se executa em fases sequenciais; o cliente só vê o resultado no final. |
| Ágil | Filosofia de entregas pequenas e frequentes, com feedback real e ajuste constante de rumo. |
| Manifesto Ágil | Documento de 2001 que resume a mudança de mentalidade em quatro valores. |
| Feedback | Retorno de quem usa ou paga pelo produto, que orienta o próximo passo. |
| Scrum | Framework mais usado para praticar o Ágil, com ciclos curtos, papéis, reuniões e artefatos. |

---

## 2. Mínimo para começar

### O essencial

- **Cascata:** planeja-se tudo no início, executa-se em fases fixas e o cliente só vê o resultado no final. Funciona quando os requisitos são estáveis; quando mudam no meio do caminho, descobrir isso tarde sai caro.
- **Ágil:** entregas em pedaços pequenos e frequentes, feedback real e ajuste constante de rumo.
- **Manifesto Ágil (2001):** pessoas e interações mais que processos e ferramentas; software funcionando mais que documentação extensa; colaboração com o cliente mais que negociação de contrato; responder a mudanças mais que seguir um plano.
- **Regra de leitura:** o lado direito de cada frase não é descartado; ele só vale menos que o da esquerda quando os dois entram em conflito.
- **Ágil e Scrum:** o Ágil é uma filosofia, um conjunto de valores; o Scrum é um framework para colocá-la em prática (assunto do próximo módulo).

### Preparação do ambiente

Nada a instalar neste módulo. Você só precisa de um editor de texto para escrever em Markdown e de acesso ao seu fork do repositório de entrega.

**Como conferir que deu certo:** Abra o primeiro link da tabela de referências abaixo. O resultado esperado é a página do Manifesto carregando em português, com os quatro valores no topo.

### Referências curadas

| Recurso | Tipo | Idioma | Tempo | O que aproveitar |
|---|---|---|---|---|
| [Manifesto para o Desenvolvimento Ágil de Software](https://agilemanifesto.org/iso/ptbr/manifesto.html) | documentação oficial | pt | 5 min | Leia só os quatro valores e a frase final; é a base do autoteste e do desafio. |
| [Princípios por trás do Manifesto Ágil](https://agilemanifesto.org/iso/ptbr/principles.html) | documentação oficial | pt | 10 min | Escolha 3 dos 12 princípios que mais se ligam ao desafio. |
| [Manifesto Ágil, da Atlassian](https://www.atlassian.com/br/agile/manifesto) | tutorial | pt | 15 min | Leia a parte sobre os princípios e compare com a sua própria leitura dos valores. |

### Autoteste rápido

Tente responder antes de abrir as respostas.

1. **Verdadeiro ou falso:** no modelo cascata, o cliente só vê o resultado no final do projeto.

    ??? success "Confira"
        Verdadeiro.

2. **Complete a lacuna:** um dos valores do Manifesto Ágil é priorizar ___ funcionando em vez de documentação extensa.

    ??? success "Confira"
        Software.

3. **Reflita:** pense em um projeto que você já viveu (trabalho, faculdade, hobby). Ele seguiu mais a lógica cascata ou ágil? O que mudaria se fosse ao contrário?

    ??? success "Confira"
        Resposta livre. O importante é identificar se houve uma entrega única no final (cascata) ou entregas e ajustes ao longo do caminho (ágil).

### Estou pronto para o desafio?

- [ ] Consigo explicar com minhas palavras o que o mapa do conceito descreve.
- [ ] Meu ambiente está funcionando (verificação acima).
- [ ] Sei onde consultar a documentação oficial quando travar.

---

## 3. Desafio aberto

### Contexto

Na Pi Júnior, antes de aceitar um projeto, o gerente avalia se a forma de trabalhar combina com o pedido do cliente. Para treinar esse olhar, você vai olhar para trás: analisar um projeto que você mesmo viveu, como se fizesse um diagnóstico para um colega.

### Enunciado

Entregue um diagnóstico de uma página sobre um projeto real que você viveu (trabalho, faculdade ou hobby), mostrando se ele foi conduzido mais como cascata ou mais como ágil, e uma versão alternativa do cronograma desse projeto em que o primeiro feedback real chegue mais cedo.

### Requisitos e restrições

- O diagnóstico aponta quando o primeiro feedback real aconteceu e o que ele mudou (ou teria mudado).
- Cita pelo menos duas evidências concretas do projeto, não impressões gerais.
- A versão alternativa tem ao menos duas entregas intermediárias, cada uma seguida de um ponto de feedback.
- Usa pelo menos dois valores do Manifesto Ágil como argumento.
- Apenas texto em Markdown; nenhuma ferramenta específica é obrigatória.
- Tempo sugerido: 30 a 45 min.

### Pistas

Abra uma pista por vez, só quando estiver realmente travado.

??? tip "Pista 1: por onde começar"

    Pergunte-se: quando, pela primeira vez, alguém que usaria o resultado viu algo funcionando? Quanto tempo depois do início do projeto foi isso?

??? tip "Pista 2: uma ferramenta ou conceito útil"

    Use os quatro valores do Manifesto como uma lente: para cada um, procure um fato do projeto que mostre se ele foi respeitado ou ignorado.

??? tip "Pista 3: um ponto de atenção"

    Ágil não significa “sem planejamento” nem “sem documentação”. Releia a regra de leitura do Manifesto antes de justificar suas mudanças.

### Critérios de pronto

O desafio está concluído quando:

- [ ] O diagnóstico diz, com evidências, se o projeto foi mais cascata ou mais ágil.
- [ ] O momento do primeiro feedback real está identificado.
- [ ] A versão alternativa tem pelo menos duas entregas intermediárias, cada uma com ponto de feedback.
- [ ] Nenhum argumento trata planejamento ou documentação como algo a descartar.
- [ ] O trabalho está em uma branch, com commits seguindo a convenção do time.

**Para quem terminar cedo:** Repita o diagnóstico para um projeto de um colega da turma e compare as conclusões.

---

## 4. Pergunta de pesquisa

### A pergunta

Em que situações o modelo cascata ainda é uma escolha defensável, e que sinais indicam que um projeto precisa de uma abordagem ágil?

### Por que essa pergunta

Ao receber um pedido de cliente, é preciso decidir como conduzir o projeto; a resposta ajuda a defender essa decisão com argumentos, e não por hábito.

### Por onde começar (opcional)

- Palavras-chave para buscar: requisitos estáveis, custo de mudança, incerteza em projetos

### Como responder

Escreva de 3 a 6 linhas na sua nota (seção 5) contendo:

1. a resposta, com suas palavras;
2. as fontes consultadas (com link);
3. se possível, como você testou a resposta na prática.

---
## 5. Entregável documentado

### O que entregar

1. O resultado do desafio, dentro da subpasta `entregaveis/` (e/ou `src/`, quando houver código).
2. Uma **nota em Markdown** com o modelo abaixo, salva em `docs/nota-m01.md`.

**Onde entregar:** no seu **fork** deste repositório, dentro da pasta exclusiva `entregas/<seu-nome>/semana-01/modulo-01/`, abrindo um **Pull Request** para a `main` com título no padrão `feat(s01-m01): entrega <seu-nome>`.

### Estrutura de arquivos da sua entrega

```text
entregas/<seu-nome>/semana-01/modulo-01/
├── docs/                      # Documentação extra, diagramas, esquemas ou notas
│   └── nota-m01.md            # Nota em Markdown com a reflexão e respostas
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
