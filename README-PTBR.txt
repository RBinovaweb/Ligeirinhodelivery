# Ligeirinho ⚡ — Loja + Painel

Arquivos:
- index.html = loja pública
- admin.html = painel administrativo
- firebase-config.js = configuração do Firebase
- seed-products.js = produtos iniciais
- database.rules.json = regras do Realtime Database

## 1. Firebase
Crie/abra um projeto no Firebase.
Adicione um app Web e copie o firebaseConfig para firebase-config.js.
Crie o Realtime Database.
Ative Authentication > Sign-in method > Email/Password.
Crie seu usuário administrativo em Authentication > Users.

## 2. Realtime Database Rules
Cole o conteúdo de database.rules.json nas regras do Realtime Database e publique.

A loja pode ler produtos/configurações.
Somente usuário autenticado pode editar produtos/configurações e ler pedidos.
Clientes podem criar pedidos sem login.

## 3. GitHub Pages
Envie todos os arquivos para o mesmo repositório.
Ative Settings > Pages > Deploy from branch.
Abra:
- /index.html = loja
- /admin.html = painel

## 4. Primeiro acesso
Entre em /admin.html com o e-mail e senha criados no Firebase.
Clique em "Importar produtos iniciais".
Depois edite preços, imagens, categorias e disponibilidade.

## Observação de segurança
O firebaseConfig do app Web não é uma senha. A proteção real dos dados é feita pelas regras do Firebase Authentication + Realtime Database.
