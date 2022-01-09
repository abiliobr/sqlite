## Convenções para nomeação de itens em bancos de dados relacionais

Neste texto apresento algumas sugestões para a nomeação de objetos em bancos de dados relacionais como MySQL, PostgreSQL e SQLite. São convenções coletadas de alguns fontes, adaptadas a minha experiência ou visão pessoal.

Como o contexto de aplicação é em língua portuguesa, pode ser que alguma regra não seja conveniente para uso em outros idiomas.

### Nomes de objetos em geral
1. Evitar o uso de caracteres acentuados, espaços, hifens e caracteres especiais em nomes de tabelas e colunas;
3. Evitar nomes reservados do SQL, como insert, delete, union, etc;
4. Evitar, se possível, verbos e preposições.

### Tabelas
1. Os nomes de tabelas devem estar em **letras minúsculas** somente, evitando números e sublinhados no início do nome;
2. Os nomes de tabelas devem estar no **singular**. Por exemplo: pessoa;
3. Evitar o uso de sublinhado em tabelas com nomes compostos, preferindo a justaposição das palavras. Por exemplo: contabancaria;
4. Para nomes de tabelas que representam relacionamentos 'um-para-muitos', usar o sublinhado como separador ou \_x_. Por exemplo: usuario_emprestimo ou usuario_x_emprestimo;
5. Evitar o uso de prefixos. Por exemplo: tbl_pessoa;
6. O nome de tabela não deve ser coincidir com o nome de uma de suas colunas.

### Colunas
1. O nome de uma coluna não deve ter o mesmo nome da tabela que a contém;
2. Os nomes das colunas não devem ter o nome da tabela por 'prefixo'. Por exemplo: pessoa_nome; 
3. Os nomes de colunas devem estar sempre no **singular**;
4. Os nomes de colunas devem estar em **letras minúsculas** somente, exceto para siglas conhecidas ou nomes que requerem o uso de alguma letra maiúscula;
5. Pode-se usar sublinhado para melhor leitura do campo, por exemplo: data_nascimento ou datanascimento;
6. O nome da chave primária da tabela deve ser 'id' apenas e deve estar na primeira posição da estrutura da tabela;
7. O nome de chaves estrangeiras deve ser o nome da tabela estrangeira concatenado com '\_id'. Por exemplo: pessoa_id;
8. Alguns sufixos como \_status, \_seq, etc. (sempre antecedidos de \_) podem ser usados para documentar o tipo da coluna. Por exemplo: devolucao_status, senha_seq.
9. 
