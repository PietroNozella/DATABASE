# Banco de dados venda de peças 
CREATE TABLE peca_ (
    preco FLOAT (50),
    descricao VARCHAR (50),
    codigo_peca INT PRIMARY KEY,
    quantidade_estoque INT (50),
    codigo_armazem INT(50)
);

CREATE TABLE armazem_ (
    codigo_armazem INT PRIMARY KEY,
    endereco VARCHAR (50),
    fk_peca__codigo_peca INT
);

CREATE TABLE vendedor_ (
    codigo_vendedor INT PRIMARY KEY,
    nome VARCHAR (50),
    endereco VARCHAR (50),
    comissao FLOAT,
    fk_cliente__pedido_codigo INT,
    fk_cliente__pedido_codigo_ INT,
    fk_cliente__pedido_numero INT
);

CREATE TABLE cliente__pedido (
    codigo INT,
    nome VARCHAR(50),
    endereco VARCHAR (50),
    faturamento FLOAT,
    limite_credito FLOAT,
    fk_codigo_vendedor_codigo_vendedor_PK INT,
    fk_nome_vendedor_nome_vendedor_PK VARCHAR (50),
    quantidade_pecas INT,
    numero INT,
    data DATE,
    codigo INT,
    fk_nome_cliente_nome_cliente_PK VARCHAR (50),
    fk_endereco_cliente_endereco_cliente_PK VARCHAR (50),
    fk_codigo_vendedor_codigo_vendedor_PK_ INT,
    codigo_peca INT,
    preco_cotado FLOAT,
    PRIMARY KEY (codigo, numero)
);

CREATE TABLE nome_cliente (
    nome_cliente_PK VARCHAR (50) PRIMARY KEY,
    nome_cliente VARCHAR (50)
);

CREATE TABLE endereco_cliente (
    endereco_cliente_PK VARCHAR (50)  NOT NULL PRIMARY KEY,
    endereco_cliente VARCHAR (50)
);

CREATE TABLE codigo_vendedor (
    codigo_vendedor_PK INT NOT NULL PRIMARY KEY,
    codigo_vendedor INT
);

CREATE TABLE codigo_vendedor (
    codigo_vendedor_PK INT (50) NOT NULL PRIMARY KEY,
    codigo_vendedor INT (50)
);

CREATE TABLE nome_vendedor (
    nome_vendedor_PK VARCHAR (50)  NOT NULL PRIMARY KEY,
    nome_vendedor VARCHAR (50)
);
 
ALTER TABLE armazem_ ADD CONSTRAINT FK_armazem__2
    FOREIGN KEY (fk_peca__codigo_peca)
    REFERENCES peca_ (codigo_peca)
    ON DELETE RESTRICT;
 
ALTER TABLE vendedor_ ADD CONSTRAINT FK_vendedor__2
    FOREIGN KEY (fk_cliente__pedido_codigo, fk_cliente__pedido_codigo_, fk_cliente__pedido_numero)
    REFERENCES cliente__pedido (codigo, codigo, numero)
    ON DELETE RESTRICT;
 
ALTER TABLE cliente__pedido ADD CONSTRAINT FK_cliente__pedido_2
    FOREIGN KEY (fk_codigo_vendedor_codigo_vendedor_PK)
    REFERENCES codigo_vendedor (codigo_vendedor_PK)
    ON DELETE NO ACTION;
 
ALTER TABLE cliente__pedido ADD CONSTRAINT FK_cliente__pedido_3
    FOREIGN KEY (fk_nome_vendedor_nome_vendedor_PK)
    REFERENCES nome_vendedor (nome_vendedor_PK)
    ON DELETE NO ACTION;
 
ALTER TABLE cliente__pedido ADD CONSTRAINT FK_cliente__pedido_4
    FOREIGN KEY (fk_nome_cliente_nome_cliente_PK)
    REFERENCES nome_cliente (nome_cliente_PK);
 
ALTER TABLE cliente__pedido ADD CONSTRAINT FK_cliente__pedido_5
    FOREIGN KEY (fk_endereco_cliente_endereco_cliente_PK)
    REFERENCES endereco_cliente (endereco_cliente_PK);
 
ALTER TABLE cliente__pedido ADD CONSTRAINT FK_cliente__pedido_6
    FOREIGN KEY (fk_codigo_vendedor_codigo_vendedor_PK_)
    REFERENCES codigo_vendedor (codigo_vendedor_PK);
