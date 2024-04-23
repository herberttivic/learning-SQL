## Outros conceitos


### Entidade
- é o objeto ou evento do mundo real que desejamos armazenar no banco dedados
---
### Atributo
- campos que as entidades devem ter (Ex: código, nome)
---
### Atributo chave [Primary key (PK)]
- também chamado de chave primária
- é um identificador único de cada objeto de determinada entidade
- ex: entidade pessoa -> cpf ( PK )
---
### Relacionamentos
- é quando uma entidade tem necessidade compartilhar seus dados com outra
- relacionamentos são geralmente referenciados por uma chave primária
  - ex: 
  ```
  categoria(id, nome)
  produto(id, nome, id_categoria)
  ```
---
### Relacionamento unário
- também chamado de grau 1
- é quando uma entidade se relaciona com ela mesma
- ou seja, um objeto de determinada entidade se relaciona com outro objeto dessa mesma entidade
- ex :
    ```
    pessoa (
      cpf : bigint, 
      nome : string, 
      cpf_pai : bigint (relacionamento com pessoa.cpf), 
      cpf_mae : bigint (relacionamento com pessoa.cpf)
    );
    ```
---
### Relacionamento binário
- também chamado de grau 2
- é uma relação entre objetos de entidades diferentes
- ex: produto -> categoria
---
### Relacionamento ternário
-  também chamado de grau 3
- é quando 3 entidades se ligam através de um mesmo relacionamento
- geralmente a entidade que une as 3 outras é chamada de pivô
- ex:
    ```
    pedido(
      id_cliente : string
      id_produto : string
      id_forma_de_pagamento : string
    );
    ```
---
### Cardialidade (máxima)
- define a quantidade máxima de ocorrência de uma entidade que será relacionada com outra entidade
- tipos de relacionamento (qtd):
  - 1:1 (one to one)
  - 1:n (one to many)
  - n:m (many to many)
- obs : many to many sempre exige uma entidade pivô
- ex : o objeto VENDEDOR só pode conter até 3 PRODUTOS

---
### Cardialidade (mínima)
- define a quantidade mínima de ocorrência de uma entidade que será relacionada com outra entidade
- ex:
  - Escritório 1..1
    - 1 Escritório pode conter 1 vendedor ou nenhum(0) vendedor (min 0, max 1)
  - Vendedor 0..1
    - 1 Vendedor precisa de pelo menos 1 esritório (min 1, max 1)