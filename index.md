## Convenções para nomeação de itens em bancos de dados relacionais

Neste texto apresento algumas sugestões para a nomeação de objetos em bancos de dados relacionais como MySQL, PostgreSQL e SQLite. São convenções coletadas de alguns fontes, adaptadas a minha experiência ou visão pessoal.

Como o contexto de aplicação é em língua portuguesa, pode ser que alguma regra não seja conveniente para uso em outros idiomas.

### Nomes de objetos em geral
1. Evitar caracteres acentuados, espaços, hifens e caracteres especiais em nomes de tabelas e colunas;
2. Evitar o uso de PascalCase e camelCase. Por exemplo, é melhor usar data_nascimento ou datanascimento do que as formas DataNascimento ou dataNascimento;
3. Evitar palavras reservadas do SQL, como insert, delete, union, etc;
4. Evitar, se possível, verbos e preposições.

### Tabelas
1. Os nomes de tabelas devem estar em **letras minúsculas** somente, evitando números e sublinhados no início do nome;
2. Os nomes de tabelas devem estar no **singular**. Por exemplo: pessoa, contato, grupo;
3. Evitar o uso de sublinhado em tabelas com nomes compostos, preferindo a justaposição das palavras. Por exemplo: contabancaria;
4. Para nomes de tabelas que representam relacionamentos 'um-para-muitos', usar o sublinhado como separador ou \_x_. Por exemplo: usuario_emprestimo ou usuario_x_emprestimo;
5. Evitar o uso de prefixos como tbl_ ou tab_;
6. O nome de tabela não deve ser coincidir com o nome de uma de suas colunas.

### Colunas
1. O nome de uma coluna não deve ter o mesmo nome da tabela que a contém;
2. Os nomes das colunas não devem ter o nome da tabela por "prefixo". Por exemplo: usar 'datanascimento' em vez de 'pessoa_datanascimento'; 
3. Os nomes de colunas devem estar sempre no **singular**;
4. Os nomes de colunas devem estar em **letras minúsculas** somente, exceto para siglas conhecidas ou nomes que requerem o uso de alguma letra maiúscula;
5. Pode-se usar sublinhado para melhor leitura do campo. Por exemplo: data_nascimento;
6. Evitar o uso de prefixos como pk_ e fk_ para chaves primárias e estrangeiras;
7. O nome da chave primária da tabela deve ser somente 'id' e deve estar na primeira posição da estrutura da tabela;
8. O nome de chaves estrangeiras devem ser o nome da tabela estrangeira correspondente concatenado com \_id. Por exemplo: pessoa_id;
9. Alguns sufixos como \_status, \_seq, etc. podem ser usados para recordar o tipo da coluna. Por exemplo: devolucao_status, senha_seq.
10. 
