# Guia de domínio para atividades

## Estrutura do README

Cada atividade deve ter um arquivo `README.md` dentro de `assignments/<id>/` e seguir a ordem e os títulos do [`template do projeto`](../../../../templates/assignment-template.md):

- `# 📘 Atividade: [Título da Atividade]`
- `## 🎯 Objetivo`
- `## 📝 Tarefas`
- Para cada tarefa: `### 🛠️ [Título da Tarefa]`, `#### Descrição` e `#### Requisitos`

Mantenha os títulos em português conforme o template. Não remova seções nem acrescente seções extras, a menos que o usuário peça. Escreva para alunos iniciantes, com objetivos concretos e requisitos claros, específicos e verificáveis. Inclua exemplos de entrada e saída em blocos de código quando ajudarem a esclarecer o resultado esperado.

## Arquivos da atividade

Use um identificador curto em `kebab-case` para o diretório e para o `id` no `config.json`. O `README.md` é obrigatório. Os únicos arquivos permitidos pelo hook do projeto dentro de uma atividade são:

- `README.md`
- `starter-code.py`
- `data.csv`

Crie `starter-code.py` ou `data.csv` somente quando forem solicitados ou necessários para cumprir os requisitos. Não crie soluções completas nem arquivos adicionais sem solicitação explícita.

## Registro no portal

Cada item em `config.json` deve usar o formato existente e ter `id`, `title`, `description` e `path`, com `path` igual a `assignments/<id>`. Inclua anexos apenas quando os arquivos existirem no diretório da atividade.

O script [`update-config.js`](../scripts/update-config.js) define automaticamente o prazo para sete dias após a execução. Use-o somente quando esse prazo for confirmado pelo usuário; caso contrário, peça a data desejada antes de registrar a atividade. Para anexar arquivos a uma atividade já registrada, use [`add-attachment.js`](../scripts/add-attachment.js) e os tipos correspondentes (`python` para `starter-code.py`, `csv` para `data.csv`).
