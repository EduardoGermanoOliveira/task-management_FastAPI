# task-management_FastAPI
![image](https://github.com/EduardoGermanoOliveira/task-management_FastAPI/assets/90634869/74af4eb5-9f4d-42e3-a88f-3346ef81482d)


O projeto consiste em criar uma API para gerenciamento de tarefas que permite a criação, leitura, atualização e exclusão de tarefas. Cada tarefa deve ter um título, descrição, status e data de criação.

Sugestão de estrutura:
fastapi-task-management/
├── app/
│   ├── controllers/
│   │   └── task_controller.py
│   ├── services/
│   │   └── task_service.py
│   ├── repositories/
│   │   └── task_repository.py
│   ├── models/
│   │   └── task_model.py
│   ├── main.py
│   └── database.py
└── tests/
    ├── test_controllers.py
    ├── test_services.py
    └── test_repositories.py

Descrição dos Componentes
Controllers: Responsáveis por definir os endpoints da API.
Services: Contêm a lógica de negócios e validações.
Repositories: Gerenciam a interação com o banco de dados.

Requisitos
Python 3.10+
FastAPI
SQLAlchemy
SQLite

1. Modelagem de Dados
Crie um modelo para representar uma tarefa com os seguintes campos:

id (integer, primary key)
title (string)
description (string)
status (string, pode ser "Pendente", "Em Progresso", "Concluída")
created_at (datetime)
2. Repositório de Tarefas
Implemente a camada de repositório para realizar operações CRUD:

Criar uma nova tarefa
Obter uma tarefa pelo ID
Atualizar uma tarefa
Deletar uma tarefa
Listar todas as tarefas
3. Serviço de Tarefas
Implemente a camada de serviço para validar os dados e aplicar a lógica de negócios:

Criar uma nova tarefa
Obter uma tarefa pelo ID
Atualizar uma tarefa
Deletar uma tarefa
Listar todas as tarefas
4. Controlador de Tarefas
Implemente os endpoints da API utilizando FastAPI:

POST /tasks/: Criar uma nova tarefa.
GET /tasks/: Listar todas as tarefas.
GET /tasks/{task_id}: Obter detalhes de uma tarefa específica por ID.
PUT /tasks/{task_id}: Atualizar uma tarefa específica por ID.
DELETE /tasks/{task_id}: Deletar uma tarefa específica por ID.
