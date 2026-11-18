# Resultados reportados no TCC

As métricas são extraídas das tabelas e conclusões do texto acadêmico; **não são novas medições** deste repositório.

| Classificador | F1-score CV | Desvio informado | Acurácia de teste |
|---|---:|---:|---:|
| Random Forest | 0,9074 | ±0,0045 | 0,92 |
| XGBoost | 0,9195 | ±0,0091 | 0,93 |
| Gradient Boosting | **0,9257** | ±0,0057 | **0,94** |
| Logistic Regression | 0,7839 | ±0,0109 | 0,83 |
| Naive Bayes | 0,4720 | ±0,0126 | 0,68 |

## Indicadores complementares
- Gradient Boosting: AUC-ROC **0,988** segundo resumo/conclusão.
- XGBoost: recall da classe anômala (`1`) **0,95** na tabela.
- Gradient Boosting: recall da classe anômala **0,90** na tabela.
- Random Forest: recall da classe anômala **0,94** na tabela.

## Interpretação
Gradient Boosting obteve o maior F1-score de validação cruzada e acurácia de teste entre os cinco modelos com tabelas. XGBoost apresentou maior recall da classe anômala, importante para reduzir ataques não detectados.

## Ressalvas
A conclusão textual discute taxas de falsos negativos que não se alinham integralmente aos recalls por classe tabelados. Priorizamos os valores tabulados; não calculamos taxas adicionais nem declaramos reprodução. SVM é citado na metodologia mas sem uma tabela equivalente de resultados.
