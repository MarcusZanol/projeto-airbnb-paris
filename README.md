# 🏠 Análise Exploratória de Dados - Airbnb Paris

Projeto de análise exploratória de dados (EDA) utilizando o dataset público do [Inside Airbnb](https://insideairbnb.com/) referente a anúncios de hospedagem em **Paris, França**.

## 📊 Sobre o projeto

Este projeto tem como objetivo explorar e entender o comportamento das locações de curto e longo prazo na cidade de Paris, identificando padrões de preço, tipos de imóveis, distribuição geográfica por bairro e perfil de estadia mínima exigida pelos anfitriões.

## 🗂️ Fonte dos dados

Os dados foram obtidos através do portal [Inside Airbnb](https://insideairbnb.com/pt/), que disponibiliza dados públicos e atualizados de anúncios reais do Airbnb em diversas cidades do mundo.

- **Cidade**: Paris, Île-de-France, França
- **Arquivo utilizado**: `listings.csv`
- **Data de extração dos dados**: 16 de junho de 2026

## 🛠️ Ferramentas e bibliotecas utilizadas

- Python
- Pandas
- Matplotlib
- Seaborn

## 🔍 Etapas da análise

1. **Importação e inspeção inicial dos dados**
2. **Tratamento de valores ausentes** (identificação de colunas com dados nulos, como `neighbourhood_group`, `price`, `last_review`, `reviews_per_month` e `license`)
3. **Análise da coluna `minimum_nights`**: identificação de outliers e separação da base em dois grupos:
   - `df_7`: locações com estadia mínima de até 7 dias
   - `df_30`: locações com estadia mínima de 8 a 30 dias
4. **Análise por tipo de imóvel** (`room_type`) em cada grupo
5. **Análise por bairro** (`neighbourhood`): quantidade de locações e valor médio de preço
6. **Visualizações gráficas**: histogramas, boxplots, countplots e gráficos de barras

## 📈 Principais insights

- A maioria dos anúncios exige estadia mínima de **1 a 2 noites**, indicando forte vocação turística de curto prazo.
- Existe um grupo relevante de anúncios com estadia mínima de **30 dias**, sugerindo locações de temporada ou uso residencial.
- Bairros como **Buttes-Montmartre** e **Popincourt** concentram o maior volume de locações de curta duração.
- Os maiores valores médios de locação estão em bairros centrais e nobres, como **Palais-Bourbon** e **Élysée**.

## 📁 Estrutura do repositório

├── listings.csv # Base de dados original
├── notebook.ipynb # Notebook com toda a análise
└── README.md # Este arquivo

## 👤 Autor

**Marcus Penso**
Software Engineer | Python | Data Science | Java | SQL

https://www.linkedin.com/in/marcus-penso-8bb0b2263/
