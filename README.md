# Sistema Gerenciador de Tarefas

Bem-vindo ao Sistema Gerenciador de Tarefas! Este projeto permite que você organize suas tarefas diárias, oferecendo operações CRUD para criar, recuperar, atualizar e excluir registros de tarefas. Desenvolvido utilizando a trilha .NET da Digital Innovation One (DIO), o projeto inclui uma API ou aplicação MVC, dependendo da sua preferência, e utiliza o Entity Framework para interagir com o banco de dados.

## Diagrama de Classe da Tarefa

O principal componente deste sistema é a classe `Tarefa`, que inclui os seguintes atributos:

- `Id`: Identificador único da tarefa.
- `Titulo`: Título da tarefa.
- `Descricao`: Descrição detalhada da tarefa.
- `Data`: Data de realização da tarefa.
- `Status`: Status atual da tarefa (por exemplo, "Pendente", "Concluída", etc.).

## Endpoints da API

### Obter Tarefa por ID
- **Verbo**: GET
- **Endpoint**: `/Tarefa/{id}`
- **Parâmetro**: `id`
- **Corpo**: N/A

### Atualizar Tarefa
- **Verbo**: PUT
- **Endpoint**: `/Tarefa/{id}`
- **Parâmetro**: `id`
- **Corpo**: Schema da Tarefa

### Deletar Tarefa
- **Verbo**: DELETE
- **Endpoint**: `/Tarefa/{id}`
- **Parâmetro**: `id`
- **Corpo**: N/A

### Obter Todas as Tarefas
- **Verbo**: GET
- **Endpoint**: `/Tarefa/ObterTodos`
- **Parâmetro**: N/A
- **Corpo**: N/A

### Obter Tarefas por Título
- **Verbo**: GET
- **Endpoint**: `/Tarefa/ObterPorTitulo`
- **Parâmetro**: `titulo`
- **Corpo**: N/A

### Obter Tarefas por Data
- **Verbo**: GET
- **Endpoint**: `/Tarefa/ObterPorData`
- **Parâmetro**: `data`
- **Corpo**: N/A

### Obter Tarefas por Status
- **Verbo**: GET
- **Endpoint**: `/Tarefa/ObterPorStatus`
- **Parâmetro**: `status`
- **Corpo**: N/A

### Criar Tarefa
- **Verbo**: POST
- **Endpoint**: `/Tarefa`
- **Parâmetro**: N/A
- **Corpo**: Schema da Tarefa

## Schema da Tarefa

```json
{
  "id": 0,
  "titulo": "string",
  "descricao": "string",
  "data": "2022-06-08T01:31:07.056Z",
  "status": "Pendente"
}
