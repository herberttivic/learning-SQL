## Terceira forma normal

- Eliminar os campos que são resultados de equações de outros campos
- Ex : 
  - ERRADO => boletim(nota1, nota2, nota3, media, somatoria)
  - CORRETOR => boletim(nota1, nota2, nota3)
  - Obs : media e somatoria podem ser obtidos a partir de operações com nota1, nota2 e nota3. Portanto não devem estar no banco de dados.