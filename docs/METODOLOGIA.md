# Metodologia descrita no TCC

## 1. Dados
HTTP Dataset CSIC 2010. O texto registra **61.065 observações, 17 colunas**, com alvo binário `classification` (normal = 0, anômalo = 1).

## 2. Exploração e preparação
- Análise de valores ausentes, colunas e distribuição das classes.
- Limpeza e normalização de requisições HTTP.
- Pré-processamento textual: tokenização, stemming e TF-IDF, conforme capítulos metodológicos.
- Tratamento de atributos categóricos e construção de atributos derivados de URL e conteúdo.
- Redução de dimensionalidade com PCA, conforme descrito no TCC.

**Nota:** a seção de resultados relata **57 atributos** (20 de URL, 30 de conteúdo e 7 derivados); outra parte discute PCA aplicado às características TF-IDF. Sem código-fonte não presumimos a ordem exata ou execução simultânea das variantes.

## 3. Modelagem e avaliação
O texto descreve divisão treino/teste **80/20**, validação cruzada e busca de hiperparâmetros. Menciona Random Forest, SVM, XGBoost, Gradient Boosting, Logistic Regression e Naive Bayes.

Métricas: acurácia, precisão, recall, F1-score, AUC-ROC, matrizes de confusão e curvas ROC/Precision-Recall.

## 4. Ambiente reportado
Ubuntu 22.04; Python 3.11; scikit-learn, XGBoost, NLTK, pandas, NumPy, Matplotlib e Seaborn.

## 5. Limitações
Esta é uma adaptação documental. Nenhum experimento foi executado nesta publicação. Para reprodução, são necessários scripts originais, obtenção permitida dos dados, versões de dependências e confirmação dos procedimentos de avaliação.
