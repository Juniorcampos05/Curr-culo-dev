Resumo do Código Front-end
Tem uma página HTML com um botão.

Quando o usuário clica no botão, um JavaScript envia uma requisição POST com dados JSON (nome, idade, profissão) para o servidor backend.

Usa a função fetch para fazer essa requisição para uma URL http://localhost:3000/api/requisicao.

Quando recebe uma resposta JSON do backend, exibe essa resposta na tela dentro de um elemento <pre>.

Também faz tratamento básico de erro, mostrando uma mensagem caso a requisição falhe.

Resumo do Código Back-end
Use o framework Node.js chamado Express para criar um servidor web que atende na porta 3000.

Usa o middleware express.json()para interpretar dados JSON que chegam no corpo das requisições.

Usa o middleware cors()para permitir que o front-end (que pode estar em outra origem) faça requisições sem ser bloqueado pelo navegador.

Defina um endpoint POST em /api/requisicaoque:

Recebe os dados enviados pelo front-end.

Exibe os dados recebidos no console.

Retorna uma resposta JSON com uma mensagem de sucesso, os dados recebidos e um timestamp.
