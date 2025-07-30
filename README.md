# Análise e Precificação Inteligente de Imóveis para Hospedagem

Este projeto foi desenvolvido como parte do curso **"Pandas: Transformação e Manipulação de Dados"** da Alura, com o objetivo de realizar a limpeza, tratamento e manipulação de um conjunto de dados para precificação inteligente no setor de hospedagem de imóveis.
 
## Descrição do Projeto

O objetivo principal deste projeto é preparar um conjunto de dados brutos, oriundo de informações de hospedagem, para que possa ser utilizado em modelos de *Machine Learning* para precificação inteligente. O notebook `precificacao_imoveis.ipynb` (ou o script Python correspondente) detalha todas as etapas do processo de **ETL (Extract, Transform, Load)**.

## O que foi aprendido e aplicado

O desenvolvimento deste projeto me permitiu aplicar e consolidar diversas técnicas de manipulação de dados com a biblioteca **Pandas**:

* **Normalização de Dados:** Utilização do método `json_normalize` para converter dados semi-estruturados em um DataFrame tabular.
* **Limpeza e Transformação:**
    * Tratamento de dados aninhados em listas utilizando o método `explode`.
    * Conversão de tipos de dados (`astype`) para garantir a integridade numérica de colunas como `max_hospedes`, `quantidade_banheiros` e `preco`.
    * Limpeza de valores monetários e conversão para o tipo `float64` utilizando `apply` e `applymap`, lidando com caracteres especiais como `$` e `,`.
* **Manipulação de Textos:**
    * Conversão de textos para minúsculas (`str.lower`).
    * Utilização de **expressões regulares (regex)** para remover caracteres indesejados e tratar hífens.
    * Processo de **tokenização** de *strings* para preparar dados textuais para análises posteriores.
* **Tratamento de Dados de Tempo (Datetime):**
    * Identificação e conversão de colunas para o tipo `datetime` com o método `pd.to_datetime`.
    * Extração e manipulação de componentes de data, como ano e mês, para agregações de dados.

## Tecnologias Utilizadas

* **Python**
* **Pandas**
* **Numpy**

## Repositório

O projeto completo está disponível neste repositório. O arquivo principal é `precificacao_imoveis.ipynb`.
