Como rodar o Back-End corretamente?
1. Clone este repositório no VSCode e instale as bibliotecas necessários com os seguintes códigos:
- **npm install express cors dotenv uuid**

- **npm install nodemon --save-dev**
2. Coloque o servidor para rodar com o seguinte comando:
**npm run dev**
3. Abra o Postman, crie uma pasta com as seguintes 'requests':
  
![image](https://github.com/user-attachments/assets/743569c2-6163-46da-a257-83872027a9d9)

4. Realizar as rotas:
4.1. Buscar todos os ingressos
Dentro da rota GET adicione a seguinte URL: http://localhost:3000/api/ingressos Após clicar em 'Send', todos os ingressos devem aparecer.

4.2. Buscar um ingresso pelo ID
Dentro da rota GET adicione a seguinte URL: http://localhost:3000/api/ingressos/id (colocar id) Após clicar em 'Send', deve aparecer o ingresso do ID inserido.

4.3. Criar um ingresso
Dentro da rota POST adicione a seguinte URL: http://localhost:3000/api/ingressos E no body adicione as informações de "evento", "local", "data_evento", "categoria", "preco", "quantidade_disponivel". Ficando neste modelo:

![image](https://github.com/user-attachments/assets/57157149-0c53-4d6b-994c-faeeef218923)


Após clicar em 'Send', o ingresso será adicionado.

4.4. Atualizar um ingresso
Dentro da rota PUT adicione a seguinte URL: http://localhost:3000/api/ingressos/id (colocar id) E no body adicione as informações que você deseja atualizar ("evento", "local", "data_evento", "categoria", "preco", "quantidade_disponivel"). *As informações que não desejar alterar também devem ser inseridas. Após clicar em 'Send', o ingresso será atualizado.

4.5. Deletar um ingresso
Dentro da rota DELETE adicione a seguinte URL: http://localhost:3000/api/ingressos/id (colocar id) Após clicar em 'Send', o ingresso será deletado, sendo possível confirmar com a mensagem de confirmação:

![image](https://github.com/user-attachments/assets/77ced433-eca7-4dde-949b-52d9ae67bb23)

4.6. Comprar um ingresso
Dentro da rota POST adicione a seguinte URL: http://localhost:3000/api/venda No body, adicione o id do ingresso que deseja comprar e a quantidade de ingressos, como a imagem a seguir:

![image](https://github.com/user-attachments/assets/eac29679-ca43-405d-ac48-144b77247e18)


Após clicar em 'Send', a seguinte mensagem de confirmação deve aparecer:

![image](https://github.com/user-attachments/assets/24cffc46-ee5f-4d11-b74b-f8248e5573d8)
