# Extração e Análise de Dados de CNPJs (Cornélio Procópio)

Este repositório contém scripts desenvolvidos para processamento e filtragem de dados públicos de empresas (Receita Federal), com foco na extração de informações societárias e de estabelecimentos da região de Cornélio Procópio e arredores.

> **Nota:** Este trabalho foi desenvolvido como parte das atividades do **Projeto de Extensão Analisia** da UTFPR.

## 🎯 Objetivo

O código tem como objetivo automatizar a leitura de grandes volumes de dados (arquivos CSV de Dados Abertos de CNPJs), filtrar empresas ativas baseadas em códigos de municípios específicos e consolidar as informações dos sócios dessas empresas em arquivos prontos para análise.

## 🛠️ Tecnologias Utilizadas

* **Python 3**
* **Pandas:** Para manipulação e análise de dados (DataFrames).
* **Jupyter Notebook:** Ambiente de desenvolvimento interativo.

## 📂 Estrutura do Código

O script `CódigoAnalisiaExtracaodeCornelio.ipynb` realiza as seguintes etapas:

1.  **Carregamento de Dados:** Leitura da base de municípios para identificar os códigos IBGE da região de interesse.
2.  **Filtragem de Estabelecimentos:** Processamento dos arquivos de estabelecimentos para encontrar CNPJs ativos na localidade alvo.
3.  **Cruzamento de Dados (Join):** Utilização dos CNPJs filtrados para buscar os respectivos sócios na base de dados de Sócios.
4.  **Consolidação:** Os dados processados são salvos em arquivos parciais (`Socio_resultadoX.csv`) e posteriormente unificados em um único dataset final (`Socios_resultado_combinado.csv`).

## 🚀 Como Executar

1.  Certifique-se de ter o Python e a biblioteca Pandas instalados:
    ```bash
    pip install pandas
    ```
2.  Organize os arquivos de dados brutos nas pastas `Municipios/`, `Estabelecimentos/` e `Socios/` conforme referenciado no script.
3.  Execute o notebook célula por célula para gerar os arquivos de saída.

## 👨‍💻 Autor

Desenvolvido por **[Seu Nome]**
*Estudante de Engenharia de Computação - UTFPR*

---
*Projeto Analisia - UTFPR Cornélio Procópio*
