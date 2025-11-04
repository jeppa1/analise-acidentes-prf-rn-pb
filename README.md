# Análise de Acidentes (PRF): RN vs. PB (2017-2025)

Análise Exploratória de Dados (EDA) sobre acidentes da PRF (2017-2025) com foco comparativo entre Natal (RN) e João Pessoa (PB).

**Notebook Interativo (Kaggle):** [Clique aqui para acessar o Notebook](https://www.kaggle.com/code/jadsonchagas/analise-acidentes-prf-rn-pb)

---

### 1. Visão Geral do Projeto

Este projeto é uma análise de ponta a ponta dos registros de acidentes de trânsito da Polícia Rodoviária Federal, cobrindo um período de 9 anos (2017-2025). O objetivo foi comparar o perfil dos acidentes nos estados do Rio Grande do Norte e Paraíba, com foco específico nas rodovias federais que atravessam as capitais Natal e João Pessoa.

A análise investiga tendências temporais, causas, tipos de veículos e a gravidade das ocorrências para identificar padrões e fatores de risco.

### 2. Principais Descobertas (Insights)

A análise revelou padrões claros, com destaque para o impacto desproporcional dos acidentes com motocicletas:

* **Tendência Temporal:** O volume de pessoas envolvidas em acidentes nas rodovias de João Pessoa é consistentemente maior que em Natal.
* **Causas Principais:** As causas mais comuns em ambas as capitais são relacionadas à falha humana, como "Falta de Atenção à Condução" e "Não manter distância".
* **O Risco da Motocicleta (Hipótese Confirmada):**
    * "Motocicleta" é o veículo com o maior número de envolvidos em acidentes em ambas as capitais, superando "Automóvel".
    * Isso explica por que "Queda de ocupante" e "Tombamento" são os tipos de acidente mais frequentes.
    * A chance de um motociclista sair **ileso** de um acidente é mínima (**6,1% em JP**, **9,5% em Natal**), em comparação com acidentes gerais (~45%).
* **O Custo Humano:** Os acidentes com motos são o principal motor das estatísticas de gravidade:
    * Em **João Pessoa**, **78,3%** de todas as "Lesões Graves" e **60,5%** de todos os "Óbitos" envolveram motocicletas.
    * Em **Natal**, **70,5%** de todas as "Lesões Graves" vieram de acidentes com motos.

### 3. Visualizações Principais

| Evolução por Estado | Evolução por Capital |
| :---: | :---: |
| ![Evolução por Estado](img/image_aa716c.png) | ![Evolução por Capital](img/image_9f0880.png) |

| Gravidade Geral | Gravidade (Apenas Motos) |
| :---: | :---: |
| ![Gravidade Geral](img/COLE_O_NOME_DA_IMAGEM_DA_CELULA_19.png) | ![Gravidade (Apenas Motos)](img/COLE_O_NOME_DA_IMAGEM_DA_CELULA_21.png) |

### 4. Ferramentas Utilizadas

* **Linguagem:** Python
* **Bibliotecas de Análise:** Pandas
* **Bibliotecas de Visualização:** Matplotlib, Seaborn
* **Ambiente:** Jupyter Notebook (para ETL) e Kaggle Notebooks (para Análise)

### 5. Estrutura do Repositório

* `/data/processed/`: Contém os 4 arquivos CSV consolidados e limpos, prontos para análise.
* `/img/`: Contém as visualizações exportadas do notebook.
* [cite_start]`analise-acidentes-prf-rn-pb.ipynb`: O notebook Jupyter final com a análise exploratória (o mesmo do Kaggle).
* `acidentes_2025_2017.ipynb`: O notebook original usado para o processo de ETL (consolidação dos dados brutos).

### 6. Fonte dos Dados

Os dados brutos foram obtidos no Portal de Dados Abertos da Polícia Rodoviária Federal (PRF), cobrindo o período de 2017 a 2025.
