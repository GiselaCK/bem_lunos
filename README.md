# bem_lunos
Modelos de aprendizado de máquina para prever as notas finais de alunos baseados em diversos fatores.
Projeto Aprendizado de Maquina
**Nome:** Gisela C. Kassick, Giovani M. Nagano e Rebeka L. Batichotti

## Introdução
O desempenho estudantil é um dos principais indicadores de qualidade educacional e está fortemente associado a fatores sociais, psicológicos e econômicos. O dataset Student Performance Factors, disponível no Kaggle, reúne informações sobre estudantes, incluindo hábitos de estudo, tempo de sono, atividades extracurriculares e suporte familiar, com o objetivo de compreender como esses elementos influenciam o desempenho acadêmico. A análise desse conjunto de dados permite identificar padrões que auxiliam na formulação de estratégias mais eficazes para promover o aprendizado e o sucesso escolar.

Com base nesse conjunto de dados, este projeto aplica técnicas de aprendizado de máquina para prever o desempenho estudantil e compreender quais fatores exercem maior impacto sobre os resultados dos alunos. O código foi desenvolvido englobando as etapas de pré-processamento, análise exploratória, modelagem preditiva e avaliação dos resultados.
Na etapa de modelagem, diferentes algoritmos de aprendizado de máquina são aplicados para comparar sua capacidade de generalização e precisão:

--K-Nearest Neighbors (KNN): método baseado na similaridade entre amostras. A previsão é feita com base nas k observações mais próximas no espaço de características. É simples e eficiente para dados com relações locais bem definidas.
--Random Forest: conjunto de múltiplas árvores de decisão que trabalham em paralelo, reduzindo o risco de sobreajuste (overfitting) e melhorando a precisão das previsões. É robusto e oferece boa interpretabilidade por meio da importância das variáveis.
--Elastic Net: modelo linear que combina as penalizações L1 (Lasso) e L2 (Ridge), controlando a complexidade do modelo e selecionando variáveis relevantes. É útil em situações onde há colinearidade entre os preditores.
--Gradient Boosting Regressor: técnica baseada em aprendizado por reforço sequencial, onde novas árvores são adicionadas para corrigir os erros das anteriores. É um dos métodos mais poderosos para tarefas de regressão tabular.
--Ridge Regression: regressão linear com regularização L2, que reduz a influência de variáveis altamente correlacionadas e melhora a estabilidade do modelo, evitando o sobreajuste
