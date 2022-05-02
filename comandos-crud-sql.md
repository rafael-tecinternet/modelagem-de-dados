# Comandos SQL para CRUD - Refêrencia

## Resumo
- C -> Create (inserir dados)
- R -> Read (ler dados)
- U -> Update (atualizar dados)
- D -> Delete (excluir dados)

## Insert
```sql
INSERT INTO fabricantes (nome) VALUES ('Asus');
INSERT INTO fabricantes (nome) VALUES ('Dell');
INSERT INTO fabricantes (nome)  
VALUES ('Apple'), ('LG'), ('Samsung'), ('Brastemp');
```
### Produtos
```sql
INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id) VALUES (
    'Ultrabook', 'Ultrabook Asus com processador Intel Core i12, memória RAM de 16GB e Windows 11', 6500.99, 7, 1
);
INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id) VALUES (
    'Tablet Android', 'Tablet com a versão 12 do sistema operacional da Google, possui tela de 10 polegadas e armazenamento de 64GB', 4999, 3, 5
);
INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id) VALUES ('Geladeira', 'Refrigerador Frost-free com acesso à internet das Coisas e bla bla bla', 1500, 10, 6),('Iphone 13 Pro Max', 'Alta Durabilidade, processador Bionic 14, 128GB, 6GB de RAM', 6999.99, 3, 3),('Ipad Mini', 'Tablet com tela retina display de 4k, memória interna de 64GB, acesso gratuito à icloud', 5000, 8, 3);
INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id) VALUES ('Xbox', 'Console de última geração com acesso aos melhores jogos', 2500, 6, 8),('Ultrabook', 'Equipamento com processador AMD Ryzen5, 12GB RAM, placa de vídeo RTX', 4500.68, 12, 7);
```