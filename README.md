# 📱 Mobile Market Analysis & Price Prediction (2025)

Análise completa de Ciência de Dados sobre o mercado global de smartphones. O projeto vai desde a limpeza de dados e engenharia de features até a construção de um modelo preditivo de preços com Machine Learning.

## 🎯 O Problema de Negócio
Entender a relação entre as especificações técnicas (RAM, Bateria, Câmera) e o preço final do aparelho, identificando quais marcas entregam o melhor custo-benefício e prevendo valores de mercado.

## 🕵️‍♂️ Principais Insights & Correções de Dados
Durante a Análise Exploratória (EDA), identificamos e corrigimos viéses críticos:
* **Correção de Preço Global:** O dataset original focava apenas em preços dos EUA. Criamos uma métrica `Avg_Price_USD` convertendo moedas globais (Índia, China, Paquistão) para dolarizar e padronizar o valor real dos aparelhos.
* **Contagem de Modelos:** Ajustamos a contagem para considerar "Modelos Base", removendo a distorção causada por variações de armazenamento da Apple.
* **Descoberta:** A correlação mais forte com o preço é a **RAM (0.73)**, enquanto Câmera e Bateria têm pouca influência no valor final de aparelhos premium.

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Pandas, Seaborn, Matplotlib, Scikit-Learn.
* **Techniques:** Data Cleaning, Feature Engineering, Pipeline, Hyperparameter Tuning.

## 🤖 Modelagem Preditiva (Machine Learning)
Testamos 3 algoritmos para prever o preço dos celulares. O **Gradient Boosting** foi o campeão.

| Modelo | RMSE (Erro Médio) | Detalhes |
| :--- | :--- | :--- |
| Regressão Linear | $199.94 | Baseline (Performance baixa) |
| Random Forest | $94.95 | Boa performance com dados não-lineares |
| **Gradient Boosting** | **$91.26** | **Modelo Campeão após Tuning** |

## 🚀 Como Visualizar
Como o GitHub às vezes não renderiza notebooks grandes, recomenda-se usar o nbviewer:
[🔗 Clique aqui para ver o Notebook Completo e os Gráficos](https://colab.research.google.com/drive/1iXwVoY-o6QsOn4jrQ1NI7KacknVI8vpS?usp=sharing) 

---
*Projeto desenvolvido por [José Henrique (Nean)](https://www.linkedin.com/in/jos%C3%A9-henrique-do-esp%C3%ADrito-santo-0465042a6/)*
