# AtividadeFase3_Cap14

## **Descrição do Projeto**

Este projeto apresenta a aplicação de uma técnica de aprendizado de máquina para classificação de plantações agrícolas. O objetivo foi explorar e pré-processar um dataset, treinar diferentes modelos de machine learning e avaliar o desempenho de cada um.

---

## **Estrutura do Código**

### 1. **Importação de Bibliotecas**
Bibliotecas utilizadas:
- `pandas`, `seaborn`, `matplotlib` para manipulação e visualização de dados.
- Modelos e utilitários de machine learning da `sklearn`.

### 2. **Carregamento e Exploração do Dataset**
- O dataset carregado é sobre plantações agrícolas.
- Realizadas análises como:
  - Verificação de duplicatas.
  - Identificação de outliers (Boxplot).
  - Visualização da distribuição dos rótulos (labels).
 
  Podemos verificar a partir dos dados observados alguns padrões mesmo com tipos de culturas diferentes:
  - temperatura: 25°C
  - Umidade: 80%
  - Nível de nitrogênio: 35
  - Nível de fósforo: 50
  - Nível de potássio: 30

### 3. **Limpeza de Dados**
Por conta da falta de métodos de limpeza de dados no conteúdo da aula, precisei realizar algumas soluções comuns na tratativa de dados. A solução encontrada para este tipo de situação foi o IQR(Intervalo Interquartil) como métrica para substituir as outliers com a mediana da classe. Este metodo me apresentou bastante interesse por realizar alterações somente nas outliers e permanecendo os dados mais críticos.

### 5. **Treinamento de Modelos**
Modelos treinados:
- Regressão Logística
- K-Nearest Neighbors (KNN)
- Suporte a Vetores Máquinas (SVM) com diferentes kernels (RBF, Polinomial e Linear)
- Árvore de Decisão
- Random Forest

### 6. **Avaliação e Ranking**
- Métricas utilizadas:
  - Acurácia de cada um dos modelos
  - Relatórios detalhados com precisão, recall e F1-score.
- Geração de um ranking dos melhores modelos com base na acurácia.

---

## **Resultados**
- O modelo com melhor desempenho foi `Random Forest` com uma acurácia de `99.32%`.
- Observou-se que modelos como `SVM (RBF)` também apresentaram desempenho competitivo.
- Modelos simples como `KNN` tiveram resultados inferiores, indicando a necessidade de ajustes em hiperparâmetros.
- Apesar da diferença da acurácia existente entre os modelos, todos tiveram resultados acima de 90%, portanto realzando uma análise mais critica pensando no investimento gasto para conceder um modelo adequado e a quantidade de dados sendo utilizada, o modelo de Regressão Logistica atenderia as espectativas.
