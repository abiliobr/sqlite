## Convenções para nomeação de itens em bancos de dados relacionais

Neste texto apresento algumas sugestões para a nomeação de objetos em bancos de dados relacionais como MySQL, PostgreSQL e SQLite. São convenções coletadas de alguns fontes, adaptadas a minha experiência ou visão pessoal.

Tabelas:
1. Usar nomes de tabelas em **letras minúsculas** somente, evitanto números e sublinhados \(_) no início do nome;
3. Usar nomes sempre no **singular**. Por exemplo: pessoa;
4. Evitar o uso de sublinhado em tabelas com nomes compostos, preferindo a justaposição das palavras. Por exemplo: contabancaria;
5. Para nomes de tabelas que representam relacionamentos 'um-para-muitos', usar o sublinhado como separador ou \_x_. Por exemplo: usuario_emprestimo ou usuario_x_emprestimo;
6. Não usar prefixos. Por exemplo: tbl_pessoa;
7. Não usar para o nome de tabela o mesmo nome de uma de suas colunas.

Colunas:
1. Não usar para o nome de coluna o nome da tabela que a contém;
2. Usar nomes de colunas sempre no **singular**;
3. Usar nomes de colunas em **letras minúsculas**, exceto para abreviaturas e siglas conhecidas;
4. Pode-se usar sublinhado para melhor leitura do campo: data_nascimento ou datanascimento;
5. O nome da chave primária da tabela deve ser 'id' apenas e deve estar na primeira posição da estrutura da tabela.



## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/abiliobr/dbnc/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/abiliobr/dbnc/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
