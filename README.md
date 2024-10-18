# Ensaio de Machine Learning
## Descrição
A empresa fictícia Data Money acredita que a habilidade no treinamento e ajuste fino dos algoritmos de Machine Learning, conduzida pelos Cientistas de Dados da empresa, é o principal motivo pelos excelentes resultados que suas consultorias vêm entregando aos clientes.
## Objetivo
O objetivo deste projeto é realizar uma série de ensaios com algoritmos de Classificação, Regressão e Clusterização, para estudar como a performance desses modelos varia à medida que alteramos os principais parâmetros que controlam overfitting e underfitting.
## Premissas
Este projeto foca exclusivamente em testar e ajustar modelos de Machine Learning. Portanto, etapas como análise exploratória dos dados (EDA), seleção de features e preprocessamento não fazem parte do escopo. Os dados utilizados são gerados especificamente para esta análise.
# Planejamento da Solução
## Produto Final
O produto final será composto por 7 tabelas que apresentarão a performance dos algoritmos, utilizando várias métricas de avaliação, para três conjuntos de dados distintos: treinamento, validação e teste.
## Algoritmos Avaliados
### 1. Classificação:
- Algoritmos: K-Nearest Neighbors (KNN), Decision Tree, Random Forest e Regressão Logística.
- Métricas de Performance: Acurácia (Accuracy), Precisão (Precision), Revocação (Recall) e F1-Score.
### 2. Regressão:
- Algoritmos: Regressão Linear, Decision Tree Regressor, Random Forest Regressor, Regressão Polinomial, Regressão Linear com Lasso, Regressão Linear com Ridge, Elastic Net, e versões polinomiais dos modelos com regularização.
- Métricas de Performance: Coeficiente de Determinação (R²), Erro Quadrático Médio (MSE), Raiz do Erro Quadrático Médio (RMSE), Erro Médio Absoluto (MAE) e Erro Percentual Absoluto Médio (MAPE).
### 3. Clusterização:
- Algoritmos: K-Means e Affinity Propagation.
- Métrica de Performance: Silhouette Score.
## Ferramentas Utilizadas
- Linguagem: Python 3.8
- Biblioteca Principal: Scikit-learn
# Desenvolvimento
## Estratégia de Solução
O objetivo é testar algoritmos de Machine Learning, variando seus parâmetros principais de controle de overfitting e observando as métricas de performance resultantes. A estratégia será identificar os melhores conjuntos de parâmetros e então realizar o treinamento final utilizando essas configurações otimizadas.
## Passo a Passo:
1. Divisão de Dados: Separar os dados em conjuntos de treinamento, validação e teste.
2. Treinamento Inicial: Treinar os algoritmos utilizando os parâmetros default nos dados de treinamento.
3. Avaliação (Treinamento): Medir a performance dos modelos treinados nos dados de treinamento.
4. Avaliação (Validação): Avaliar a performance com os dados de validação usando os parâmetros default.
5. Ajuste de Parâmetros: Alterar os principais parâmetros que controlam o overfitting até identificar os melhores resultados.
6. Retraining com Melhores Parâmetros: Unir os dados de treinamento e validação, e treinar novamente os algoritmos com os parâmetros ajustados.
7. Avaliação Final: Testar o modelo treinado nos dados de teste e medir a performance.
8. Insights Finais: Analisar os resultados e destacar os três principais insights obtidos dos ensaios.
## Principais Insights
### Insight 1:
Os algoritmos baseados em árvores de decisão (Decision Tree e Random Forest) apresentaram as melhores performances em todas as métricas, principalmente no ensaio de Classificação, superando algoritmos lineares.
### Insight 2:
Os resultados da Regressão Polinomial mostraram que, embora seja um modelo poderoso, é altamente sensível ao grau do polinômio, necessitando de um ajuste cuidadoso para evitar overfitting.
### Insight 3:
A performance dos algoritmos de classificação nos dados de validação apresentou resultados consistentes e alinhados com o desempenho obtido nos dados de teste, indicando uma boa generalização dos modelos e ausência de overfitting significativo.
# Resultados
## Ensaio de Classificação
### Performance nos Dados de Treinamento
![imagem](https://github.com/RafaelMacorin/ensaios_machine_learning/blob/main/classification/algorithm_metrics_train.png)
### Performance nos Dados de Validação
![imagem](https://github.com/RafaelMacorin/ensaios_machine_learning/blob/main/classification/algorithm_metrics_val.png)
### Performance nos Dados de Teste
![imagem](https://github.com/RafaelMacorin/ensaios_machine_learning/blob/main/classification/algorithm_metrics_test.png)
## Ensaio de Regressão
### Performance nos Dados de Treinamento
![imagem](https://github.com/RafaelMacorin/ensaios_machine_learning/blob/main/regression/regression_algorithm_metrics_train.png)
### Performance nos Dados de Validação
![imagem](https://github.com/RafaelMacorin/ensaios_machine_learning/blob/main/regression/regression_algorithm_metrics_val.png)
### Performance nos Dados de Teste
![imagem](https://github.com/RafaelMacorin/ensaios_machine_learning/blob/main/regression/regression_algorithm_metrics_test.png)
## Ensaio de Clusterização
### Performance sobre os Dados
![imagem](https://github.com/RafaelMacorin/ensaios_machine_learning/blob/main/cluster/algorithm_metrics_cluster.png)
# Conclusão
Neste ensaio de Machine Learning, foi possível aprofundar o entendimento sobre o comportamento de diferentes algoritmos de Classificação, Regressão e Clusterização. Concluímos que os modelos baseados em árvores se destacam em situações de classificação complexa, especialmente quando há muitos atributos. No entanto, os algoritmos de regressão exigem mais atenção no ajuste de parâmetros, como o grau polinomial, devido à sua sensibilidade ao overfitting. A escolha cuidadosa desses parâmetros é crucial para evitar o overfitting, garantindo que o modelo generalize bem em novos dados.

Essa experiência foi valiosa para entender como diferentes parâmetros influenciam a performance dos algoritmos e como otimizar sua aplicação em problemas reais. Além disso, destaca a importância do aprendizado contínuo, que é fundamental para aprimorar as análises realizadas e desenvolver soluções mais eficazes no campo de Machine Learning.
# Próximos Passos
Os próximos passos incluem a exploração de novos algoritmos e a utilização de diferentes conjuntos de dados para melhorar o conhecimento sobre os limites de performance de cada abordagem. Além disso, uma etapa de análise exploratória e seleção de features será realizada para aumentar ainda mais a qualidade das predições.
