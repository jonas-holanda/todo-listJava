<div align="center">

# To-do List criada no Curso Gratuito de Java da rocketseat
</div>

- **Configurações iniciais: [Acessar link](https://efficient-sloth-d85.notion.site/Curso-de-Java-2408d11bfc3447e980fe9460b6293976)**

- **Para executar a aplicação, use esse comando `java -jar target/todolist-1.0.0.jar` no terminal, dentro do diretório da aplicação.**
## Cadastro de Usuários

- **POST** - `http://localhost:8080/users/`
- **BODY** -
```json
{
    "name": "User Example",
    "username": "user-example",
    "password": "12345"
}
```
## Cadastro de Tarefas

- **AUTH/AUTHORIZATION (Basic Auth)** - Username: `user-example` , Password: `12345`
- **POST** - `http://localhost:8080/tasks/`
- **BODY** -
```json
{
    "description": "Tarefa para gravar tasks",
    "title": "Tarefa de teste",
    "priority": "ALTA",
    "startAt": "2024-10-14T12:20:00",
    "endAt": "2024-10-18T12:33:00"
}
```
## Lista de Tarefas

- **AUTH/AUTHORIZATION (Basic Auth)** - Username: `user-example` , Password: `12345`
- **GET** - `http://localhost:8080/tasks/`

## Atualização de Tarefas

- **AUTH/AUTHORIZATION (Basic Auth)** - Username: `user-example` , Password: `12345`
- **PUT** - `http://localhost:8080/tasks/idTask` exemplo: `http://localhost:8080/tasks/829c6c99-58b4-41e8-a599-4ee2a4c27529`
- **BODY** -
```json
{
    "priority": "BAIXA",
    "title": "Atualizando a Tarefa",
    "description": "Nova descrição da tarefa"
}
```
