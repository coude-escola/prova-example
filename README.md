# DESAFIO TÉCNICO – PDV SIMPLES

## Contexto Geral

O objetivo deste desafio é o desenvolvimento de um sistema simples de Ponto de Venda (PDV), contemplando as principais funcionalidades como o cadastro de produtos, realização de pedidos e gestão de usuários (administrativos e clientes). O desafio está estruturado por níveis de complexidade, considerando os conteúdos previamente estudados por vocês.

O desafio é progressivo, para comtemplar cada estudante, independente da etapa do curso na qual estiver, de modo que, se o estudante está no nível 2, ele realizara o nível 1 + o nível 2, se ele está no nível 3, ele realizará o que é solicitado nos níveis 1, 2 e 3, e assim por diante.

---
### ENTREGA: 26/05/2025
---

## Nível 1 – PHP e SQL

### Requisitos

* Criação de banco de dados com as tabelas:

  * `usuarios` (id, nome, email, tipo)
  * `produtos` (id, nome, preco)
  * `pedidos` (id, id\_usuario, data, status \[pendente, pago, enviado, concluído])
  * `itens_pedido` (id, id\_pedido, id\_produto, quantidade)

### Funcionalidades

* Inserção de dados via scripts PHP, recebendo os dados via formulários (usuários, produtos, pedidos).
* Exibição dos pedidos e respectivos itens.

---

## Nível 2 – PHP, SQL, HTML e CSS

### Requisitos adicionais

* Criação de interfaces HTML com estilização básica via CSS:

  * Listagem de produtos
  * Adicione, na listagem, cores de fundo diferentes para o registro a depender do seu status

    * pendente - laranja
    * pago - amarelo
    * enviado - azul
    * concluído - verde

### Funcionalidades

* Exibição mais organizada e **responsiva** dos dados em tela.

---

## Nível 3 – PHP, SQL, HTML, CSS e PHP Orientado a Objetos

### Requisitos adicionais

* Organização do código em classes PHP:

  * `Usuario`, `Produto`, `Pedido`, `ItemPedido`, `Conexao`

### Funcionalidades

* CRUD orientado a objetos para produtos, pedidos e usuários.
* Uso de boas práticas de encapsulamento.
* Modularização com `require_once`/`include`.
* Boa organização das pastas e arquivos.

---

## Nível 4 – PHP, SQL, HTML, CSS, PHP POO e JavaScript

### Requisitos adicionais

* Otimizar a experiência do usuário através do JavaScript:

  * Atualização automática da listagem de pedidos a cada segundo, sem a necessidade de recarregar manualmente a página

    * Ao adicionar um novo pedido a listagem, deve haver algum feedback visual, como uma animação de alerta, a troca de cor, alguma coisa que dure por 3 segundos.
  * Adicionar os pedidos mais recentes no topo da listagem

### Funcionalidades

* Manipulação de DOM e eventos

---

## Nível 5 – PHP, SQL, HTML, CSS, PHP POO, JavaScript e Laravel

### Requisitos adicionais

* Utilização do framework Laravel com estrutura completa:

  * `Models`, `Controllers`, `Routes`, `Views`, `Migrations`, `Middlewares`

### Funcionalidades

* Autenticação com separação entre perfis (administrativo e cliente)
* Dashboard administrativo com listagem de pedidos
* Tela do cliente com histórico de pedidos
* Persistência com Eloquent ORM

---

## Considerações adicionais (para todos os níveis)

* Uso das `$_SESSION` para simulação de login
* Validação de campos obrigatórios
* Cálculo automático do total do pedido
* Armazenamento de data e hora do pedido no banco de dados
