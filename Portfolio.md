# Documentação de  Análise de requisitos
---
## PROBLEMA DE NEGÓCIO

Após inúmeras compras que foram realizadas na loja virtual serem devolvidas, o Product Owner deseja ter uma maneira de liberar inúmeros pedidos de devolução de uma vez, seguindo um mesmo critério de elegibilidade
Através da solução de liberação desses inúmeros pedidos, os setores financeiros, de engenharia de software e de políticas de crédito reduzirão tanto o tempo médio de retorno ao cliente, como também reduzirão o gasto de tempo para processamento de cada liberação indidualizada.


### Requisitos de sistema 

* Requisito 1 - Liberar devolução em lote
Através do sistema financeiro da empresa deverão estar vísiveis todos os pedidos de devolução realizados por clientes da loja virtual. Através dessa tela de usuário deverá ser disponibilizado o recurso para todos, alguns ou um único pedido, e a consequente liberação dos selecionados(o);

  * Requisito 1.1 -Liberar recurso de seleção
Na interface do P.O deverá aparecer os pedidos de devolução, esses devem ser disponibilizados em um recurso de múltipla seleção;

  * Requisito 1.2 - Autorização
Após a seleção dos pedidos a serem liberados, no sistema deverá aparecer um botão de ação, que confirme a autorização. Ao ocorrer a liberação, o sistema deve verificar se o produto já foi enviado, prosseguindo somente caso a resposta seja positiva;
---
# Documentação Api Blueprint

FORMAT: A1

## API de filmes

Este é um exemplo de API Blueprint que descreve uma API de filmes.

## Group Filmes

Recursos relacionados a filmes na API.

### Filme collection [/movies]

#### List all Movies [GET]

Liste os filmes na ordem inversa da publicação.
~~~
 Response 200 (application/json)

    + Attributes (array[Movie])
~~~

### Estrutura de Dados

#### Filme
~~~
+ id: 810b43d0-fc0d-4199-8a79-25b471c880bf (string, required)
+ title: Avengers: Endgame (string, required)
~~~
+ description (string)
