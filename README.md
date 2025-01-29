# Banco de Dados para Mercado de Bairro

Este repositório contém a modelagem de um banco de dados para um mercado de bairro, incluindo diagrama e scripts SQL.

## 🛠 Tecnologias Utilizadas

- **MySQL** - Banco de dados relacional utilizado para armazenar as informações.
- **Workbench** - Ferramenta para modelagem e gerenciamento do banco de dados.

## 📌 Estrutura do Projeto

- `MER.png` - Contém o diagrama ER do banco de dados.
- `create.sql` - Inclui o script SQL para criação das tabelas
- `index.sql` - Inclui o script SQL para criação dos índices
- `insert.sql` - Inclui o script SQL para inserção de dados
- `procedure.sql` - Inclui o script SQL para criação das *procedures*
- `select.sql` - Inclui o scripts SQL para as consultas do dados
- `trigger.sql` - Inclui o scripts SQL para criação das *triggers*
- `view.sql` - Inclui o scripts SQL para criação das *views*

## 📌 Estrutura do Banco de Dados

O banco de dados **HortFruit** contém as seguintes tabelas principais:

### 🎯 Tabelas Principais

- **cliente**: Contém informações sobre os clientes, incluindo CPF, nome, endereço, telefone e pontos de fidelidade.
- **categoria**: Classifica os produtos vendidos no mercado.
- **produto**: Armazena os produtos disponíveis, vinculados a uma categoria, quantidade e preço unitário.
- **historico_preco**: Registra o histórico de alterações de preços dos produtos.
- **colaborador**: Armazena os dados dos funcionários, incluindo CPF, nome e status de atividade.
- **gerente**: Relação entre colaboradores que ocupam o cargo de gerência.
- **subordinado**: Relaciona os colaboradores aos seus respectivos gerentes.
- **venda**: Registra as vendas realizadas, associando cliente, colaborador e valor total.
- **venda_produto**: Relaciona produtos vendidos a cada venda realizada.
- **fornecedor**: Contém informações sobre os fornecedores dos produtos.
- **lista**: Criada por gerentes para organizar pedidos.
- **lista_produto**: Relaciona produtos a uma lista.
- **lista_fornecedor**: Relaciona fornecedores a uma lista.
- **orcamento**: Registra orçamentos solicitados a fornecedores.
- **orcamento_produto**: Relaciona produtos a orçamentos.
- **lista_orcamento**: Vincula listas a orçamentos aprovados.

## 🚀 Como Usar

1. Clone o repositório:

   ```bash
   git clone https://github.com/vini-pinheiro/banco-de-dados-mercado.git
   ```
3. Importe o script SQL na sua instância do MySQL.
4. Execute os arquivos na seguinte ordem: **create.sql** -> **procedure.sql** -> **trigger.sql** -> **insert.sql**
5. Utilize as consultas fornecidas para analisar os dados.
6. Utilize os índices para melhorar o desempenho das consultas
7. Utilize as visões para simplificar as consultas criadas

## 📄 Licença

Este projeto está sob a licença MIT. Sinta-se à vontade para utilizá-lo e contribuir!

---

Desenvolvido por [Vinicius Pinheiro](https://github.com/vini-pinheiro)
