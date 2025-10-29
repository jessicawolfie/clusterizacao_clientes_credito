# Segmentação de Clientes para Análise de Crédito

![Python](https://img.shields.io/badge/Python-3.12-blue.svg )
![Libraries](https://img.shields.io/badge/Libraries-Pandas%20%7C%20Scikit--learn-orange.svg )
![Status](https://img.shields.io/badge/Status-Concluído-success.svg )

## 1. Descrição do Projeto

Esse projeto utiliza técnicas de Machine Learning não supervisionado para segmentar clientes de uma instituição financeira com base em seus dados demográficos e de crédito.
O objetivo é identificar perfis de clientes distintos (clusters) para permitir que a empresa direcione estratégias de marketing, gestão de risco e desenvolvimento de produtos de forma mais eficaz.

O dataset utilizado é uma versão do "German Credit Data", disponível publicamente.

## 2. Contexto do problema de negócio

Em um mercado competitivo, entender quem são seus clientes é fundamental. Uma abordagem "tamanho único" para produtos de crédito e marketing é ineficiente e custosa. Ao segmentar os clientes em grupos com características semelhantes, uma instituição financeira pode:

*   **Personalizar ofertas:** Desenvolver campanhas de marketing específicas que se conectem com as necessidades de cada tipo de público.
*   **Otimizar a gestão de risco:** Entender os perfis que tendem a solicitar maiores valores de crédito e ajustar as políticas de análise.
*   **Aumentar a retenção:** Desenvolver produtos e serviços que atendam às expectativas de cada segmento, aumentando a satisfação e a lealdade do cliente.

Esse projeto trata desse problema usando o algoritmo K-Means, que ajuda a identificar e analisar esses grupos de forma automática com base nos dados.

## 3. Tecnologias utilizadas

*   **Linguagem:** Python 3
*   **Bibliotecas de Análise de Dados:**
    *   `pandas` para manipulação e limpeza dos dados.
    *   `numpy` para operações numéricas.
*   **Bibliotecas de Visualização:**
    *   `matplotlib` e `seaborn` para a criação de gráficos exploratórios e de resultados.
*   **Biblioteca de Machine Learning:**
    *   `scikit-learn` para o pré-processamento (StandardScaler) e a modelagem (KMeans).
*   **Ambiente de Desenvolvimento:**
    *   Jupyter Notebook (via VS Code) para análise interativa.
    *   Git e GitHub para versionamento de código.

## 4. Como Executar o Projeto

Para executar o projeto em sua máquina local, siga os passos abaixo:

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/jessicawolfie/cluterizacao_clientes_credito.git
    cd cluterizacao_clientes_credito
    ```

2.  **Crie e ative um ambiente virtual:**
    ```bash
    # Crie o ambiente
    python3 -m venv .venv

    # Ative o ambiente (macOS/Linux )
    source .venv/bin/activate
    # ou (Windows - PowerShell)
    # .\.venv\Scripts\Activate
    ```

3.  **Instale as dependências:**
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn jupyter
    ```

4.  **Execute o Jupyter Notebook:**
    Abra o projeto no VS Code. O notebook principal, `notebooks/1.0-eda.ipynb`, contém todo o processo de análise, desde o carregamento dos dados até a interpretação final dos clusters. Execute as células em ordem para reproduzir a análise.

## 5. Resumo dos perfis de clientes encontrados

A análise revelou 4 segmentos de clientes principais:

*   **Cluster 0: O Assalariado Padrão:** Homens de meia-idade, com casa própria e emprego estável, que buscam crédito de baixo valor para bens de consumo.
*   **Cluster 1: O Empreendedor de Alto Valor:** Homens mais velhos e com alta qualificação, que buscam os maiores valores de crédito, principalmente para a compra de carros.
*   **Cluster 2: A Jovem Inquilina:** Mulheres jovens, morando de aluguel, que buscam crédito para a compra de seu primeiro carro.
*   **Cluster 3: A Chefe de Família:** Mulheres de meia-idade, com casa própria, que buscam crédito de baixo valor para bens de consumo.

As implicações de negócio e as visualizações detalhadas para cada um desses perfis estão documentadas no notebook do projeto.

