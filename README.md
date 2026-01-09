# Tech Challenge 3 - Análise de Atrasos de Voos nos EUA

## 📋 Descrição do Projeto

Este projeto analisa dados históricos de voos nos Estados Unidos (2015) para identificar padrões de atrasos, construir modelos preditivos e agrupar aeroportos por perfil operacional.

---

## 🎯 Objetivos

- **Análise Exploratória**: Identificar sazonalidade, companhias aéreas mais eficientes e aeroportos com gargalos
- **Modelagem Supervisionada**: Prever atrasos de voos usando classificação (atraso > 15 min)
- **Modelagem Não-Supervisionada**: Clusterizar aeroportos por perfil de atraso e volume

---

## 📊 Dados Utilizados

- `flights.csv`: Dados históricos de voos (tabela fato)
- `airlines.csv`: Informações das companhias aéreas
- `airports.csv`: Dados dos aeroportos (inclui lat/long)

---

## 🚀 Como Executar

### Requisitos

**1. Baixar a base de dados para a pasta `\data`:**

```
https://drive.google.com/drive/folders/1aS7exW5N0qq1uIxvIBcAfc18OHojOMjj
```

**2. Instalar as dependências:**

```bash
pip install -r requirements.txt
```

### Ordem de Execução

**1. EDA (Análise Exploratória):**

```bash
jupyter notebook notebooks/1_EDA.ipynb
```

**2. Modelagem Supervisionada:**

```bash
jupyter notebook notebooks/2_Modelagem_Supervisionada.ipynb
```

**3. Clusterização:**

```bash
jupyter notebook notebooks/3_Clusterizacao.ipynb
```

---

## 📈 Principais Resultados

### Análise Exploratória

- **Sazonalidade**: Maior incidência de atrasos nos meses de verão (junho-agosto)
- **Companhias Aéreas**: Variação significativa na taxa de atrasos entre operadoras
- **Aeroportos**: Grandes hubs apresentam maior volume mas não necessariamente mais atrasos proporcionais

### Modelagem Preditiva

- **Algoritmo 1 (Baseline)**: Regressão Logística
- **Algoritmo 2**: XGBoost
- **Métrica de Avaliação**: ROC-AUC para classificação binária (atraso > 15 min)

### Clusterização

- **Cluster 0**: Aeroportos pequenos, baixo tráfego
- **Cluster 1**: Grandes hubs, alto tráfego, atraso moderado
- **Cluster 2**: Aeroportos problemáticos com alto índice de atrasos

---

## 🛠️ Tecnologias Utilizadas

- Python 3
- Pandas & NumPy (manipulação de dados)
- Scikit-learn (modelagem)
- Matplotlib & Seaborn (visualização)
- Plotly (mapas interativos)

---

## 👥 Autora

**Alice de Amorim Domiciano**

Projeto desenvolvido como parte do Tech Challenge 3 - FIAP

---

## 📝 Licença

Este projeto é de uso educacional.
