## Convenções para nomeação de itens em bancos de dados relacionais

Neste texto apresento algumas sugestões para a nomeação de objetos em bancos de dados relacionais como MySQL, PostgreSQL e SQLite.

### Nomes de objetos em geral
1. Usar apenas **letras minúsculas**, números e sublinhado (\_) para nomes em geral;
2. Evitar caracteres acentuados, espaços, hifens e caracteres especiais em nomes de tabelas, colunas e views;
3. Evitar o uso de PascalCase e camelCase. Por exemplo, é preferível usar 'data_nascimento' ou 'datanascimento' do que 'DataNascimento' ou 'dataNascimento';
4. Evitar o uso de abreviações;
5. Evitar o uso de palavras reservadas do SQL, como insert, delete, union, etc;
6. Evitar, se possível, o uso de preposições e outras partículas que podem ser facilmente deduzidas;
7. Usar verbos apenas para nomes de rotinas armazenadas (*stored procedures* ou SP).

### Nomes de Tabelas
1. Os nomes de tabelas devem estar em letras minúsculas somente, evitando números e sublinhados (\_) no início do nome;
2. Os nomes de tabelas devem estar no **singular**. Por exemplo: pessoa, contato, grupo;
3. Evitar o uso de prefixos como tbl_ ou tab_;
4. Evitar o uso de sublinhado em tabelas com nomes compostos, preferindo a justaposição das palavras. Por exemplo: contabancaria;
5. Para nomes de tabelas que representam relacionamentos 'um-para-muitos', usar o sublinhado como separador ou \_X_ ou apenas X. Por exemplo: usuario_emprestimo ou usuario_X_emprestimo ou usuarioXemprestimo;
7. O nome de uma tabela não deve ser coincidir com o nome de uma de suas colunas.

### Nomes de Colunas
1. O nome de uma coluna não deve ter o mesmo nome da tabela que a contém;
2. Para evitar redundância, os nomes das colunas não devem ter o nome da tabela por "prefixo". Por exemplo: é suficiente nomear apenas com 'datanascimento' em vez de 'pessoa_datanascimento'; 
3. Os nomes de colunas devem estar sempre no **singular**;
4. Os nomes de colunas devem estar em letras minúsculas somente, exceto para siglas conhecidas ou nomes que requerem o uso de alguma letra maiúscula. Por exemplo: codigoISSN;
5. Pode-se usar o sublinhado para melhorar a leitura do elemento. Por exemplo: data_nascimento;
6. Alguns sufixos como \_status, \_seq, etc. podem ser usados para relembrar o tipo da coluna. Por exemplo: devolucao_status, senha_seq.

### Nomes de Chaves Primárias
1. Evitar o uso de prefixos como pk_ e fk_ para chaves primárias e estrangeiras;
2. O nome da uma chave primária da tabela deve ser somente 'id';
3. A chave primária deve ser a primeira coluna da tabela;

### Nomes de Chaves Estrangeiras
1. O nome de uma chave estrangeira deve ser o nome da tabela estrangeira sufixado com \_id. Por exemplo: pessoa_id;

### Nomes de Colunas Booleanas
1. O nome de colunas booleanas (verdadeiro ou falso) deve ser, se possível, um adjetivo, ou um verbo no particípio. Por exemplo: ativado, inativo;
2. É possível o uso dos prefixos tem_ e com_. Por exemplo: tem_habilitacao, com_carencia;

## Referências
1. https://github.com/RootSoft/Database-Naming-Convention
2. https://stackoverflow.com/questions/7662/database-table-and-column-naming-conventions
3. https://www.sqlstyle.guide
4. https://imasters.com.br/data/convencoes-de-nomeacao-de-sql-schema
5. https://pt.stackoverflow.com/questions/138452/nomenclatura-de-tabela-e-coluna
6. https://www.devmedia.com.br/padronizacao-de-nomenclatura-revista-sql-magazine-100/24710
7. https://gist.github.com/twolfson/dbf5dbb673cbac88836d
