
# 🚀 Personalização com JavaScript

## 📝 Descrição do Desafio

Sabe quando você se cadastra em um site e, logo ao fazer login, ele já te chama pelo nome? 🤔  
Este desafio propõe criar um **pequeno sistema interativo** que solicita informações do usuário e retorna uma mensagem personalizada!  

A ideia é desenvolver um código que **pergunte ao usuário**:
- 🏷 **Qual o seu nome?**
- 🎂 **Quantos anos você tem?**
- 💻 **Qual linguagem de programação você está estudando?**

Em seguida, o programa exibirá a seguinte mensagem:

Olá [nome], você tem [idade] anos e já está aprendendo [linguagem]!


Além disso, o programa fará uma **pergunta extra** e responderá com base na escolha do usuário.  

---

## 🎯 Objetivo do Projeto

✅ Capturar informações do usuário usando `prompt()`.  
✅ Exibir mensagens dinâmicas no navegador com `alert()`.  
✅ Utilizar **operações condicionais** (`if/else`).  
✅ Desenvolver um **script interativo** que pode ser executado diretamente no navegador.  

---

## 📌 Código-Fonte

```javascript
// Coleta de informações do usuário
let nome = prompt("Qual o seu nome?");
let idade = prompt("Quantos anos você tem?");
let linguagem = prompt("Qual linguagem de programação você está estudando?");

// Exibe a mensagem personalizada
alert(`Olá ${nome}, você tem ${idade} anos e já está aprendendo ${linguagem}!`);

// Pergunta extra ao usuário
let resposta = prompt(`Você gosta de estudar ${linguagem}? Responda com o número 1 para SIM ou 2 para NÃO.`);

// Exibe a resposta personalizada
if (resposta == 1) {
    alert("Muito bom! Continue estudando e você terá muito sucesso. 🚀");
} else if (resposta == 2) {
    alert("Ahh que pena... Já tentou aprender outras linguagens? 🤔");
} else {
    alert("Resposta inválida. Tente novamente com 1 para SIM ou 2 para NÃO.");
}
🛠 Como Executar o Código?

📌 Opção 1: Rodar no Navegador (Recomendado)
Este código utiliza prompt() e alert(), então o método mais indicado para rodá-lo é no navegador.

1️⃣ Crie um arquivo index.html e cole o seguinte código:


<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interatividade com JavaScript</title>
</head>
<body>
    <script src="script.js"></script>
</body>
</html>
2️⃣ Salve o arquivo no mesmo diretório do script.js.
3️⃣ Abra o arquivo index.html no navegador (Google Chrome, Firefox, Edge, etc.).

Ou, se estiver usando o VS Code, clique com o botão direito no index.html e escolha "Open with Live Server".

📌 Opção 2: Rodar no Terminal com Node.js (⚠️ Sem prompt() e alert())
Caso queira rodar pelo terminal, é necessário remover o prompt() e alert() e utilizar readline-sync:

1️⃣ Instale o Node.js caso ainda não tenha: https://nodejs.org/
2️⃣ Instale o pacote readline-sync:
3️⃣ Altere o código para:



let nome = readline.question("Qual o seu nome? ");
let idade = readline.question("Quantos anos você tem? ");
let linguagem = readline.question("Qual linguagem de programação você está estudando? ");

console.log(`\nOlá ${nome}, você tem ${idade} anos e já está aprendendo ${linguagem}!`);

let resposta = readline.question(`\nVocê gosta de estudar ${linguagem}? (1 para SIM, 2 para NÃO) `);

if (resposta == 1) {
    console.log("Muito bom! Continue estudando e você terá muito sucesso. 🚀");
} else if (resposta == 2) {
    console.log("Ahh que pena... Já tentou aprender outras linguagens? 🤔");
} else {
    console.log("Resposta inválida. Tente novamente com 1 para SIM ou 2 para NÃO.");
}

4️⃣ Agora execute no terminal:


🎨 Melhorias Futuras
🔹 Criar uma versão com HTML + CSS para um layout mais amigável.
🔹 Adicionar um botão para iniciar a interação ao invés de usar prompt().
🔹 Armazenar as respostas em localStorage para personalizar o site em futuras visitas.
🔹 Permitir que o usuário selecione linguagens de programação a partir de uma lista.

🤝 Contribuições
Se quiser contribuir com melhorias ou correções, sinta-se à vontade para abrir um pull request ou sugerir uma issue.

📌 Criado por Luiz André (brodyandre) 🚀
📌 Feito com html e JavaScript.

📜 Licença
Este projeto está sob a licença MIT. Você pode usá-lo, modificá-lo e compartilhá-lo livremente.


