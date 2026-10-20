# API REST - Baozi Store

Projeto desenvolvido para a disciplina de **Desenvolvimento Web Back-End** do Curso Análise e Desenvolvimento de Sistemas.

## Estudo de Caso 

A Baozi Store é uma pequena loja especializada na venda de pães chineses cozidos no vapor. Para melhorar a organização do negócio, foi criado um sistema simples em API REST utilizando Java e Spring Boot para controlar clientes, produtos e pedidos.

Um cliente chamado CINTIA4546155 realizou seu cadastro no sistema. O produto vendido pela loja chama-se Huajuan (pão chinês tradicional) e possui o preço unitário de R$ 12,50, estando disponível em estoque.

Em um determinado momento, o cliente CINTIA4546155 realizou um pedido de 5 unida-des do produto Huajuan. O sistema registra o cliente, o produto comprado e a quantidade solicitada, facilitando o controle da loja.

## Tecnologias Utilizadas
- Java 21
- Spring Boot 3
- Spring Data JPA
- Banco de Dados H2 (em memória) / MySQL (Opcional)
- Maven

## Arquitetura
- `com.baozistore.api.model`: Entidades JPA (`Cliente`, `Produto`, `Pedido`)
- `com.baozistore.api.repository`: Interfaces Spring Data JPA (`ClienteRepository`, `ProdutoRepository`, `PedidoRepository`)
- `com.baozistore.api.controller`: Controladores REST (`ClienteController`, `ProdutoController`, `PedidoController`)

## Como Executar
1. Importe o projeto na sua IDE (IntelliJ IDEA, Eclipse ou VS Code) como um projeto **Maven**.
2. Execute a classe `BaoziStoreApiApplication.java`.
3. Por padrão, o projeto já está configurado com o banco **H2 em memória**, portanto subirá imediatamente na porta `8080` sem precisar instalar ou configurar servidor MySQL. (Se desejar usar o MySQL, basta descomentar as linhas do MySQL no arquivo `src/main/resources/application.properties`).
