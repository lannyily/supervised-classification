# Classificação de Variedades de Sementes de Abóbora com Machine Learning

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn)

Este repositório contém o código fonte e a documentação do projeto **"Análise Comparativa de Algoritmos de Machine Learning na Classificação de Variedades de Sementes de Abóbora"**.

O trabalho realiza uma análise comparativa entre três métodos supervisionados para classificar variedades de sementes (*Çerçevelik* e *Ürgüp Sivrisi*) com base em atributos morfológicos.

## 📄 Sobre o Projeto

A classificação automática de sementes é crucial para a indústria agrícola, garantindo qualidade e pureza varietal. Este projeto utiliza o **Pumpkin Seeds Dataset** para treinar e avaliar três modelos de aprendizado de máquina, visando identificar qual abordagem oferece o melhor desempenho diante de classes morfologicamente semelhantes.

O detalhamento teórico, metodologia completa e discussão dos resultados podem ser encontrados no artigo disponível neste repositório:
> 📄 [Full_Paper__Sistemas_Inteligentes.pdf](Full_Paper__Sistemas_Inteligentes.pdf)

## 🧠 Modelos Implementados

Foram desenvolvidos três notebooks Jupyter, cada um focado em um algoritmo específico:

1.  **K-Nearest Neighbors (KNN)** (`KNN.ipynb`):
    * Algoritmo baseado em instâncias que classifica amostras com base na maioria dos vizinhos mais próximos.
    * Simples e eficaz para padrões locais.

2.  **Naive Bayes** (`Naive_Bayes.ipynb`):
    * Modelo probabilístico baseado no Teorema de Bayes (implementação *Gaussian Naive Bayes*).
    * Assume independência entre os atributos.

3.  **Redes Neurais Artificiais (RNA)** (`RNA.ipynb`):
    * Utiliza um Perceptron Multicamadas (MLP).
    * Capaz de capturar relações não-lineares complexas nos dados.

## 📊 Resultados

Os modelos foram avaliados utilizando métricas de Acurácia, Precisão, Recall e F1-Score. O resumo dos resultados (conforme detalhado no artigo) é:

| Modelo | Acurácia (Melhor Resultado) | Observação |
| :--- | :---: | :--- |
| **Rede Neural (RNA)** | **90.40%** | Melhor desempenho geral, ideal para triagem de alta precisão. |
| **KNN** | ~87.50% | Bom desempenho, mas sensível a ruídos e outliers. |
| **Naive Bayes** | ~87.00% | Rápido e eficiente, mas limitado pela suposição de independência. |

> As Redes Neurais superaram significativamente os demais métodos após a otimização de hiperparâmetros.
