# Padrões de Acidentes de Trânsito no Brasil

Este trabalho apresenta uma análise abrangente de padrões de acidentes de trânsito nas rodovias federais brasileiras, utilizando dados abertos da Polícia Rodoviária Federal (PRF) referentes aos anos de 2023, 2024 e 2025. O projeto compreende cinco etapas principais: coleta de dados, pré-processamento, análise exploratória, aplicação de algoritmos de clusterização não supervisionada (K-Means, Hierárquico e DBSCAN) e interpretação dos resultados. O conjunto de dados consolidado abrange 213.418 registros de acidentes com 30 variáveis, apresentando alta qualidade (>99,9% completude nas colunas críticas). A análise exploratória inicial revela que colisões traseiras (19,3%) e saídas de pista (14,6%) são os tipos mais frequentes, com concentração significativa nos finais de semana (32,3% do total). Os horários de pico ocorrem às 18h, com 16.018 acidentes, enquanto a menor incidência é às 2h (3.478 acidentes). Acidentes fatais representam 7,2% do total, resultando em 17.828 mortos e 246.493 feridos ao longo do período. As rodovias BR-101 e BR-116 concentram 33,1% de todos os acidentes.

Palavras-chave: Ciência de Dados. Acidentes de Trânsito. Polícia Rodoviária Federal. Análise Exploratória. Clusterização. Padrões Espaciais. Aprendizado Não Supervisionado.

## Estrutura do Projeto

```bash
├── index.ipynb                         # Notebook principal
└── datatran/
    └── datatran_2023_2024_2025.csv     # Base de dados (necessária para execução)
```

## Pré-requisitos

Python 3.8+

Jupyter Notebook ou JupyterLab

## Instalação das dependências

```bash
pip install pandas numpy matplotlib seaborn scikit-learn scipy
```

## Como Reproduzir

### Obter os dados

Os dados utilizados são provenientes do portal de dados abertos da PRF (Polícia Rodoviária Federal), disponíveis em: https://www.gov.br/prf/pt-br/acesso-a-informacao/dados-abertos/dados-abertos-da-prf

O projeto já possui uma pasta .zip com os dados e outra datatran/ com os arquivos descompactados e concatenados em um único arquivo datatran_2023_2024_2025.csv

### Executar o notebook

Execute as células em ordem sequencial. O notebook está organizado nas seguintes seções:

| Seção | Descrição |
|---|---|
| Bibliotecas | Bibliotecas utilizadas ao longo do projeto |
| Pré-processamento | Limpeza, transformação e encoding dos dados |
| Análise Exploratória | Histogramas, boxplots, correlações e análise de outliers |
| Análise dos Objetivos | Respostas às hipóteses levantadas sobre os dados |
| K-Means | Aplicação do algoritmo com seleção de K via cotovelo, Silhouette e ARI |
| Hierárquico Max | Aplicação do algoritmo com abordagens de severidade e comportamental |

## Autores

- Hanny Araujo Borges
- Igor Melo Mesquita
- Maria Eduarda Dutra Silva