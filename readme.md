# Technical Assessment: Data Exploration 

## Overview

This technical assessment involves exploring and analyzing data across several CSV files, some of which are compressed in ZIP format. The objective is to extract insights by querying these files using [`chdb`](https://clickhouse.com/chdb), an embeddable ClickHouse database engine.

## Task Requirements
- Clone this repository using Git and [install git lFS](https://git-lfs.com/) then use it to pull large files 
- Parse and explore multiple CSV datasets.
- Handle ZIP-compressed files containing CSVs.
- Use [`chdb`](https://clickhouse.com/chdb) to load and query data efficiently.
- Demonstrate your ability to:
  - Understand data relationships.
  - Perform analytical queries.
  - Extract meaningful insights from raw data.

---
### �� Objective

Using the provided dataset, please explore and generate insights related to **beverage consumption** (e.g. soda, energy drinks, coffee...) across the **French territory**.

You are free to choose any angles of analysis or metrics you find relevant — as long as you can justify your choices afterwards 😉.

---

### �� Dataset Description

#### `stores.csv`

* `id`: Unique identifier of the store
* `codeApe`: Typology of the store (business classification)
* `postalCode`: Location of the store
* `country`: Country where the store is located

#### `items.csv`

* `id`: Unique identifier of the item
* `itemName`: Name of the product
* `amount`: Unit price of the product
* `storeId`: Identifier of the store selling the item

#### `rcp.csv`

* `id`: Unique identifier of the receipt
* `storeId`: Identifier of the store where the transaction occurred
* `date`: Date of the receipt (Unix timestamp format in milliseconds)
* `amount`: Total amount of the transaction

#### `items_receipts.csv`

* `receiptId`: Identifier of the receipt
* `itemId`: Identifier of the purchased item
* `quantity`: Quantity of the item bought in the transaction

---

Have fun, and we're excited to see how you explore the data!