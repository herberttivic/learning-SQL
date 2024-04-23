obs: são pouco usadas

## Quarta forma normal

- Uma entidade estará na 4FN se estiver na 3FN e não conter multiplas entradas multivalorais (valores repetidos em diferentes colunas)
- EX:
  - ERRADO => entiadade1 (id, paciente, plano_de_saude, exame)
  - CORRETO => entidade1(id_plano, paciente, plano_de_saude), entidade2(id_exame, exame, id_plano)

## Quinta forma normal

- Uma entidade estará na 5FN se já estiver na 4FN
- E quando um atributo está em outra tabela sem a necessidade de estar na tabela pesquisada, podendo ser removida sem perda de informação
- EX :
  - ERRADO => aluno(idAluno, nome, idMatricula), boletim(idBoletim, nota, idAluno, idMatricula)
  - CORRETO => aluno(idAluno, nome, idMatricula), boletim(idBoletim, nota, idMatricula)
  - Obs: se já possui a entidade aluno possui o idMatricula, apenas a chave estrangeira do idMatricula já é suficiente para identificar o aluno