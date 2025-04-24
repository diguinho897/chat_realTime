# Chat-Real-Time

Aplicação de chat em tempo real usando **Node.js**, **Express** e **Socket.io**.

## Descrição

Servidor HTTP em **Express** serve uma SPA (HTML/CSS/JS) que conecta clientes via WebSockets (abstraídos pelo **Socket.io**). Ao enviar uma mensagem, o cliente emite o evento `chat message`; o servidor o recebe e broadcast para todos os sockets conectados, atualizando instantaneamente o DOM.


## Instalação

1. Clone o repositório  
2. `npm install`  
3. `npm run dev` (com Nodemon) ou `npm start`
4. Necessário descompactar a pasta "node_modules"

## Uso

Acesse `http://localhost:3000`, abra múltiplas abas/janelas e troque mensagens em tempo real.

## Scripts

- `npm start` — executa `node server.js`  
- `npm run dev` — executa `nodemon server.js` para reload automático

## Tecnologias

- Node.js & V8 (Event Loop, I/O não bloqueante)  
- Express.js (rotas, arquivos estáticos)  
- Socket.io (WebSockets + fallback)  
- Nodemon (dev)
