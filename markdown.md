# Requisitos para a Interface de Treinos

## Formulário
- Adicione um formulário para criar e editar treinos.
- O formulário deve conter os seguintes campos:
  - **Título** (obrigatório)
  - **Notas**
  - **Data**
  - **Duração** (em minutos)

## Funcionalidades
- **Criar:** O formulário, quando submetido, deve criar um novo treino enviando uma requisição `POST` para a API.
- **Editar:** Cada item na lista de treinos deve ter um botão "Editar". Ao ser clicado, os dados do treino correspondente devem preencher o formulário, que passará a funcionar em modo de atualização (enviando uma requisição `PUT`).
- **Deletar:** Cada item na lista de treinos deve ter um botão "Deletar". Ao ser clicado, o sistema deve pedir uma confirmação ao usuário antes de remover o item através de uma requisição `DELETE`.

## Interface do Usuário (UI)
- Mantenha a seção existente que exibe o status da "API health".
- Organize a seção de treinos em um layout de duas colunas:
  - **Coluna da Esquerda:** Deve conter o formulário de criação/edição de treinos.
  - **Coluna da Direita:** Deve exibir a lista de treinos cadastrados.

## Melhorias de Experiência
- **Atualização Automática:** Após qualquer operação de criar, editar ou deletar um treino, a lista de treinos exibida na tela deve ser atualizada automaticamente para refletir o estado mais recente dos dados.
