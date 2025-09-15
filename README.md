# Hackathon

check access

https://hackathon.bdtech.ai/home

## 🎯 Objetivo

Você deverá desenvolver um **modelo de previsão de vendas (forecast)** para apoiar o varejo na reposição de produtos. A tarefa é prever a quantidade semanal de vendas por **PDV (Ponto de Venda)** / **SKU (Stock Keeping Unit)** para as **cinco semanas de janeiro/2023**, utilizando como base o histórico de vendas de **2022**.

Esse é um problema real, baseado no nosso produto *One-Click Order*.

## 📂 Dados Disponíveis

Você terá acesso a um conjunto de dados:

### Dados de treino (2022)

Este é o conjunto de dados que você e sua equipe irão usar para trabalhar, criar o modelo, fazer testes e desenvolver a solução final.

-   **Transações**: Data, PDV, Produto, Quantidade, Faturamento.
-   **Cadastro de produtos**: Produto, Categoria, Descrição, + até 4 atributos.
-   **Cadastro de PDVs**: PDV, On/Off Prem, Categoria (c-store, g-store, liquor etc.), Zipcode.

### Dados de teste (Jan/2023)

> [!WARNING]
> Não será compartilhado com os participantes.

Esse é o conjunto de dados em que sua solução será avaliada. Vamos comparar a sua previsão com o dado real.

-   Mesma estrutura dos dados de treino.
-   Usado apenas pela Big Data para avaliar as previsões enviadas.

## 📑 Entregáveis

Sua equipe deve submeter:

1.  **Arquivo de previsão** no formato `.csv` ou `.parquet`, com as seguintes colunas:

    | semana | pdv | produto | quantidade |
    | :--- | :--- | :--- | :--- |
    | 1 | 1023 | 123 | 120 |
    | 2 | 1045 | 234 | 85 |
    | 3 | 1023 | 456 | 110 |

    -   No caso do `.csv`, utilize `;` como caractere separador (exemplo: `1;1023;123;120`) e encoding `UTF-8`.
    -   **Colunas:**
        -   `semana` (número inteiro): número da semana (1 a 5 de janeiro/2023)
        -   `pdv` (número inteiro): código do ponto de venda
        -   `produto` (número inteiro): código do SKU
        -   `quantidade` (número inteiro): previsão de vendas

2.  **Repositório público no GitHub** com:
    -   Código completo e documentação da solução.
    -   Instruções claras de execução (`README.md`).
