# Comandos SQL - Referência

## Modelagem Física

### Criar banco de dados
```sql
CREATE DATABASE vendas CHARACTER SET utf8mb4;
```
### Criar a tabela fabricantes

```sql
CREATE TABLE fabricantes (
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL
);
```
### Visualizar detalhes estruturaias da tabela
```sql
DESC fabricantes;
```
```sqL
CREATE TABLE produtos (
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL,
    descricao TEXT(1000) NOT NULL,
    preco DECIMAL(6,2) NOT NULL,
    fabricante_id INT NOT NULL
);
```
### Criação da chave estrangeira (relacionamento entri as tabelas)
```sql
ALTER TABLE produtos
    # CONSTRAINT  é uma restrição definida no relacionameto
    # A chave estrangeira deve fazer referência à chave primária
    ADD CONSTRAINT fk_produtos_fabricantes;
    FOREIGN KEY(fabricante_id) REFERENCES fabricantes(id);
```