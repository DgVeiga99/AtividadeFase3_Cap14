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

### 3. **Limpeza de Dados**
- Remoção iterativa de outliers com base no IQR (Intervalo Interquartil).
- Substituição dos valores extremos pela mediana da respectiva coluna.

### 4. **Pré-processamento**
- Separação de features e rótulos (`label`).
- Codificação dos rótulos com `LabelEncoder`.
- Normalização das features numéricas para o intervalo [0, 1].

### 5. **Treinamento de Modelos**
Modelos treinados:
- Regressão Logística
- K-Nearest Neighbors (KNN)
- Suporte a Vetores Máquinas (SVM) com diferentes kernels (RBF, Polinomial e Linear)
- Árvore de Decisão
- Random Forest

### 6. **Avaliação e Ranking**
- Métricas utilizadas:
  - Acurácia
  - Relatórios detalhados com precisão, recall e F1-score.
- Geração de um ranking dos melhores modelos com base na acurácia.

---

## **Resultados**
- O modelo com melhor desempenho foi `Random Forest` com uma acurácia de `XX.XX%`.
- Observou-se que modelos como `SVM (RBF)` também apresentaram desempenho competitivo.
- Modelos simples como `KNN` tiveram resultados inferiores, indicando a necessidade de ajustes em hiperparâmetros.

---

## **Contribuições Finais**
- O pipeline completo abrangeu desde a análise inicial dos dados até a comparação dos modelos.
- A limpeza de outliers e a normalização foram etapas fundamentais para melhorar o desempenho dos modelos.
- A análise visual e estatística confirmou padrões importantes nos dados, auxiliando na escolha das abordagens de modelagem.

---

## **Como Executar**
1. Clone este repositório.
2. Instale as dependências necessárias:
   ```bash
   pip install -r requirements.txt
