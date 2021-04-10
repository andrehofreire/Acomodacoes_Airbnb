# Teste_Cognitivo
Teste Cognitivo Preço de Acomodações Airbnb Rio de Janeiro


## Questões Enviadas

a. Como foi a definição da sua estratégia de modelagem?
- Nas etapas de limpeza e pré-processamento utilizei métodos de normalização de variáveis, remoção de outliers, tratamento de valores nulos e incoerentes.
- Com o objetivo de encontrar quais variáveis são as mais relevantes para o modelo criei um mapa de calor para enxergar as correlações lineares e utilizei o parâmetro "feature_importances" do modelo Random Forest para me dizer quais variáveis são as que mais ajudam a explicar a variável price, ordenando da mais importante para a menos importante.


b. Como foi definida a função de custo utilizada?
- Utilizei a importância Gini, que é a função de custo padrão do RandomForestRegressor do Scikit-learn.


c. Qual foi o critério utilizado na seleção do modelo final?
- Realizei testes com diferentes algoritmos (Regressão linear, ridge, lasso e Svm-Regressor) e o RandomForestRegressor se mostrou o melhor para o problema em questão.


d. Qual foi o critério utilizado para validação do modelo? Por que escolheu utilizar esse método?
- Utilizei o train_test_split para dividir os dados, o algoritmo foi treinado nos dados de treino e testado em dados que ele não havia "visto" previamente. Utilizei esse método para garantir que a avaliação da precisão do modelo nos retorne resultados confiáveis.


e. Quais evidências você possui de que seu modelo é suficientemente bom?
- Conseguimos alcançar um r2 de 0.85, que nos diz que conseguimos explicar 85% da variância da variável price com o nosso modelo.
- Utilizei também alguns métodos visuais, vimos que os resíduos possuem uma distribuição aproximadamente normal, o que nos dá um indicativo de que o modelo não é tendencioso.

