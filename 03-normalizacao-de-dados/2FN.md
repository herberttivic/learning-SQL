## Segunda forma normal

- Uma entidade estará na segunda forma normal se ele atender as regras da 1FN
- E se todos os atributos não-chave forem dependentes da chave primária
- Ex: 
  - ERRADO => pedido (cod_pedido, cod_produto, nome_produto, preco_produto, qtd, subtotal)
  - CORRETO => pedido (cod_pedido, cod_produto, qtd, subtotal)
  - Obs: o nome_ produto e preco_produto não são dependentes da chave primária cod_pedido, mas sim da chave estrangeira cod_produto. então ela não deve estar na tabela