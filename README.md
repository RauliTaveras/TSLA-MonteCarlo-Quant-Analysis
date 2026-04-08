# 📊 TSLA Quantitative Analysis & Monte Carlo Simulation
**Autor:** Rauli Enmanuel Taveras Hernández

## Este repositorio está disponible tanto en inglés como en español. 🇩🇴
## This repository is available in both English and Spanish. 🇺🇸
---

## 🇩🇴 Repositorio en Español
Este proyecto presenta un análisis avanzado de Tesla Inc. (TSLA) cubriendo la última década. Se demuestra que las métricas tradicionales son insuficientes para activos de alta volatilidad y se propone un marco de gestión de riesgos basado en simulaciones estocásticas de alto impacto. Cada celda de trabajo en los archivos adjuntos está debidamente definida y explicada para guiar al lector en el proceso analítico.

### Características Clave (Key Features):
* **Curaduría de Datos Multifuente:** Integración de la API `yfinance` con estados financieros 10-K extraídos manualmente para garantizar precisión en el histórico de 10 años.
* **Análisis Estadístico Avanzado (EDA):** Detección de anomalías, leptocurtosis (colas pesadas) y análisis profundo de Drawdown para medir el riesgo tangible del inversor.
* **Motor de Simulación Estocástica:** Ejecución de 1,000,000 de trayectorias posibles para modelar el futuro del activo.
* **Métricas de Riesgo Institucional:** Implementación de Value at Risk (VaR) y Conditional VaR (CVaR) para capturar escenarios de "cisne negro".

### Fundamento Matemático:
Utilizamos el **Movimiento Browniano Geométrico (GBM)**, el estándar de oro en finanzas para modelar precios que no pueden ser negativos:
$$S_t = S_0 \exp\left(\left(\mu - \frac{\sigma^2}{2}\right)t + \sigma W_t\right)$$
* **$\mu$ (Drift):** La tendencia o retorno promedio histórico.
* **$\sigma$ (Volatilidad):** El riesgo o desviación del precio.
* **$W_t$ (Wiener Process):** El choque aleatorio del mercado (azar).

👉 **[Ver Notebook en Español](./TSLA_Analisis_Cuantitativo_ES.ipynb)**

---

## 🇺🇸 Repository in English
This project features an advanced quantitative analysis of Tesla Inc. (TSLA) spanning the last decade. It highlights the limitations of traditional finance for high-volatility assets and proposes a risk management framework based on high-impact stochastic simulations. Every code cell in the provided files is clearly defined and explained to guide the reader through the analytical process.

### Key Features:
* **Multi-source Data Curation:** Merging `yfinance` API with manual 10-K financial statement extraction for a robust 10-year baseline.
* **Advanced Statistical Analysis (EDA):** Detection of anomalies, leptokurtosis (heavy tails), and deep Drawdown analysis to measure tangible investor risk.
* **Stochastic Simulation Engine:** 1,000,000 price trajectory simulations to model the asset's future behavior.
* **Institutional Risk Metrics:** Implementation of Value at Risk (VaR) and Conditional VaR (CVaR) to capture "black swan" scenarios.

### Mathematical Foundation:
We implemented **Geometric Brownian Motion (GBM)**, the gold standard for modeling stock prices that cannot drop below zero:
$$S_t = S_0 \exp\left(\left(\mu - \frac{\sigma^2}{2}\right)t + \sigma W_t\right)$$
* **$\mu$ (Drift):** The historical average return or trend.
* **$\sigma$ (Volatility):** The price deviation or risk.
* **$W_t$ (Wiener Process):** The random market shock.

👉 **[View English Notebook](./TSLA_Quantitative_Analysis_EN.ipynb)**

---

## 📈 Visual Results / Resultados Visuales

![Dashboard](./TSLA_Executive_Dashboard.png)

![Monte Carlo Animation](./TSLA_MonteCarlo_WowFactor.gif)
