# Dicionário de Dados

## Visão Geral

O dataset utilizado neste projeto é o **Instacart Market Basket Analysis**, disponibilizado pelo Kaggle. Ele representa o histórico de compras de uma empresa fictícia de supermercado online e será utilizado para identificar oportunidades de cross-sell por meio da análise de cesta de compras.

---

# Tabelas

## orders.csv

Armazena informações sobre os pedidos realizados pelos clientes.

**Grão da tabela:**
Um registro representa um pedido.

**Campos principais:**

- order_id
- user_id
- eval_set
- order_number
- order_dow
- order_hour_of_day
- days_since_prior_order

---

## order_products__prior.csv

Relaciona cada pedido aos produtos comprados.

**Grão da tabela:**
Um registro representa um produto dentro de um pedido.

**Campos principais:**

- order_id
- product_id
- add_to_cart_order
- reordered

---

## products.csv

Cadastro dos produtos.

**Grão da tabela:**
Um registro representa um produto.

**Campos principais:**

- product_id
- product_name
- aisle_id
- department_id

---

## aisles.csv

Cadastro dos corredores (Aisles).

**Grão da tabela:**
Um registro representa um corredor.

**Campos principais:**

- aisle_id
- aisle

---

## departments.csv

Cadastro dos departamentos.

**Grão da tabela:**
Um registro representa um departamento.

**Campos principais:**

- department_id
- department

---

# Relacionamentos

departments (1) → (N) products

aisles (1) → (N) products

products (1) → (N) order_products__prior

orders (1) → (N) order_products__prior