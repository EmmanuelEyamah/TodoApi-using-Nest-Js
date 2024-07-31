Create Todo
mutation CreateTodo($input: CreateTodoInput!) {
createTodo(createTodoInput: $input) {
id
title
}
}

Get All Todo
{todos{id title}}

Get Todo By ID
query Todo($input:Int!){
todo(id: $input){
id title
}
}

Update Todo
mutation UpdateTodo($input: UpdateTodoInput!){
updateTodo(updateTodoInput: $input){
id
title
}
}

Remove Todo
mutation RemoveTodo($input: Int!){
removeTodo(id: $input){id}
}
