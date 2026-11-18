---
name: new-assignment
description: "Use when: creating a new programming assignment, exercise, or task folder in assignments/. Guides the activity README, optional starter files, registration in config.json, and validation against the project template."
---

# Criar uma nova atividade

## Quando usar

Use esta skill para planejar e criar uma atividade de programação no diretório `assignments/` e registrá-la no portal do projeto.

## Procedimento

1. Leia o [guia de domínio](./references/assignment-guide.md), [`templates/assignment-template.md`](../../../templates/assignment-template.md), as instruções aplicáveis em `.github/instructions/assignments.instructions.md`, `config.json` e uma atividade existente semelhante.
2. Identifique o título, os objetivos de aprendizagem, o nível dos alunos e os requisitos de cada tarefa. Não invente prazos, anexos ou requisitos; pergunte ao usuário quando uma informação ausente for necessária para concluir a atividade corretamente.
3. Escolha um identificador curto em `kebab-case` para a pasta, confira se ela já existe e crie `assignments/<id>/README.md`.
4. Estruture o README conforme o template, preservando a ordem e os títulos das seções. Escreva em português claro para alunos iniciantes, com objetivos concretos e requisitos observáveis e verificáveis.
5. Crie `starter-code.py` e/ou `data.csv` somente quando forem solicitados ou necessários para atender aos requisitos. Use apenas os nomes de arquivo permitidos para atividades: `README.md`, `starter-code.py` e `data.csv`.
6. Confirme com o usuário que o prazo automático de sete dias do [script de registro](./scripts/update-config.js) é apropriado e execute-o com o `id`, título e descrição confirmados. Se esse prazo não for apropriado, obtenha a data desejada antes de registrar a atividade.
7. Se houver arquivos para anexar, registre-os depois da atividade usando o [script de anexos](./scripts/add-attachment.js), com o nome de exibição, arquivo e tipo correspondentes.
8. Valide o resultado: confira a estrutura do README, valide a sintaxe JSON de `config.json` e confirme que todos os caminhos de anexos referenciados existem. Não altere atividades ou arquivos fora do escopo.
9. Ao concluir, resuma os arquivos criados ou atualizados e as verificações realizadas.
