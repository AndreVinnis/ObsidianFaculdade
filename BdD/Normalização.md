Podemos definir normalização como uma sequência de passos e verificações aplicadas a um banco de dados visando *eliminar, ou pelo menos minimizar, as redundâncias* e inconsistências nos dados. O processo de normalização é aplicado em etapas, conhecidas como *Formais Normais (FN),* que vão garantir que o banco de dados fique bem estruturado. Normalmente após a aplicação das formas normais, algumas tabelas acabam sendo divididas em duas ou mais tabelas, o que no final gera um número maior de tabelas do que o originalmente existente.

## 1º Forma normal
Uma tabela deve possuir *apenas valores atômicos em cada coluna*. Isso significa que cada campo deve conter apenas um valor por registro, evitando grupos repetitivos ou listas dentro de uma mesma célula.

![[Pasted image 20250403141742.png]]

Converte para isso:
![[Pasted image 20250403141846.png]]
## 2º Forma Normal
Aprimora a estrutura do banco de dados *eliminando dependências parciais*. Todos os atributos não chave devem depender exclusivamente da chave primária inteira, e não de apenas uma parte dela.
A resolução da aplicação da segunda forma normal é realizada através da *exclusão dos atributos que não dependem totalmente da chave primária*, da tabela original, e constituindo-se com estes uma nova tabela, que terá como chave primária o atributo participante da chave primária da tabela origem.

![[Pasted image 20250403142924.png]]

 ![[Pasted image 20250403142948.png]]
## 3º Forma Normal
Tem como objetivo eliminar dependências transitivas, garantindo que os atributos dependem unicamente da chave primária e não de outros atributos não chave. A aplicação da terceira forma normal consiste em retirar das estruturas os campos que são funcionalmente dependentes de outros campos que não são chaves.
![[Pasted image 20250403143647.png]]

![[Pasted image 20250403143708.png]]
