# trainee-kanban

Material didático (MkDocs, tema Material) e repositório de entregas do Programa de Trainee da diretoria de Projetos da **Pi Júnior UFMG**.

Acesse o conteúdo formatado online: **[trainee-kanban](https://pijunior-trainee.github.io/trainee-kanban/).**

---

## Como entregar suas atividades (Fluxo de Fork + Pull Request)

Você **não** deve alterar os arquivos dentro de `docs/` (que contêm o material didático). Todas as suas entregas devem ficar isoladas dentro da sua pasta pessoal em `entregas/`.

### Passo a passo

1. **Faça um Fork** deste repositório para a sua conta pessoal do GitHub.
2. **Clone o seu fork** e crie uma branch para o módulo que vai entregar:
```bash
   git clone https://github.com/<seu-usuario>/trainee-kanban.git
   cd trainee-kanban
   git checkout -b feat/s01-m01-<seu-nome>
```
3. **Crie a estrutura da sua entrega** dentro de `entregas/<seu-nome>/semana-01/`:

```
entregas/<seu-nome>/
├── docs/
│   └── nota-m01.md            # Nota em Markdown com reflexão e resposta de pesquisa
├── src/                       # Código-fonte (mantenha a pasta mesmo em desafios sem código)
│   └── .gitkeep
├── entregaveis/               # Artefatos textuais, diagnósticos, prints ou exports
│   └── .gitkeep
└── README.md                  # Apresentação da entrega e passos para reproduzir
```
4. **Commit e Push** seguindo Conventional Commits:
```bash
    git add entregas/<seu-nome>/
    git commit -m "feat(s01-m01): adiciona entrega do módulo 01"
    git push -u origin feat/s01-m01-<seu-nome>
```

5. **Abra um Pull Request** da sua branch para a main do repositório oficial da Pi Júnior preenchendo o template de PR.

### Rodar a documentação localmente (com uv)
Caso queira visualizar o site didático localmente antes de abrir um PR ou ao contribuir com novos módulos:
```bash
    uv sync
    uv run mkdocs serve
```
O site abre em `http://127.0.0.1:8000`. Para validar o build exatamente como a CI faz:
```bash
    uv run mkdocs build --strict
```
### Estrutura do repositório
```
.
├── .github/                  # Workflows de CI/Pages e template de Pull Request
├── docs/                     # Material didático publicado no GitHub Pages (não alterar nas entregas)
│   ├── index.md
│   └── semana-01/            # Metodologia Ágil e Kanban (módulos 01 a 06)
├── entregas/                 # Diretório exclusivo para as entregas dos trainees via Fork + PR
│   └── .gitkeep
├── mkdocs.yml                # Configuração do MkDocs
├── pyproject.toml            # Dependências e configuração do projeto (uv)
├── uv.lock                   # Lockfile determinístico do uv
└── README.md
```