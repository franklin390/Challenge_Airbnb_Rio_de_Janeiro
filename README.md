# **Challenge Airbnb - Rio de Janeiro**

*24 de maio, 2021*

## **Descrição geral do problema**

---

![Airbnb](https://marcas-logos.net/wp-content/uploads/2020/03/Airbnb-logo.png)

Airbnb é um serviço online comunitário para as pessoas anunciarem, descobrirem e reservarem acomodações e meios de hospedagem.

Este sistema permite aos indivíduos alugar o todo ou parte de sua própria casa, como uma forma de acomodação extra. O site fornece uma plataforma de busca e reservas entre a pessoa que oferece a acomodação e o turista que busca pela locação. Abrange mais de 500 mil anúncios em mais de 35.000 cidades e 192 países. Desde sua criação em Novembro de 2008 até Junho de 2012, mais de 10 milhões de reservas foram agendadas via Airbnb.

Os dados por trás do site Inside Airbnb são obtidos de informações publicamente disponíveis no site do Airbnb. Os dados foram analisados, limpos e agregados para facilitar a discussão pública. E nesta análise, este assunto será o tema principal.


**Objetivo:** Utilizar a linguagem **Python**, para **prever o tipo de acomodação escolhido pelos clientes**.

**Perguntas:**

* Como foi a definição da sua estratégia de modelagem?
	> A estratégia usada para avaliar este conjunto de dados pode ser descrita a partir dos seguintes passos:
		1. Análise exploratória do conjunto de dados de forma geral, identificando valores ausentes, variáveis duplicadas, colunas inconsistentes, etc.;
		2. Estudo mais detalhado sobre a distribuição das principais variáveis do conjunto de dados; Detecção de distorções causadas por outliers, valores inconsistentes, etc.;
		3. Remoção dos outliers das principais variáveis numéricas do conjunto de dados; Avaliação da eficácia da remoção dos outliers na distribuição do conjunto de dados;
		4. Transformação do conjunto de dados utilizando diferentes técnicas como: Normalicação, padronização e etc;
		5. Utilização diferentes técnicas para a etapa de Features Selection como: SelectKBest, Information Gain, ANOVA F-value, Forward Selection, Extra Trees Classifier e Random Forest Importance;
		6. Criação de um conjunto de componentes a partir da técnica PCA;
		7. Avaliação preliminar do conjunto de dados em diferentes formatos com diferentes algoritmos preditivos como: LogistRegression, KNN, LDA, AdaBoost, RandomForest, XGBoost e etc;
		8. Seleção e otimização dos algoritmos que apresentaram os melhores resultados na avaliação preliminar;
		9. Avaliação do resultado dos algoritmos otimizados a partir da função Log Loss e;
		10. Seleção do melhor modelo criado.

* Como foi definida a função de custo utilizada?
	> Para a trabalhar com esta análise de classificação, optamos pelo uso da função LogLoss em todas as etapas de criação do modelo para que previsões incorretas de maneira muito acertiva tivessem penalidades maiores.
* Qual foi o critério utilizado na seleção do modelo final?
	> Vários testes foram efetuados, e na grande maioria, o algoritmo XGBoost apresentou a melhor performance na predição feita para o conjunto de dados. Seu score para as métricas de acurácia e LogLoss foram os que apresentaram os melhores resultados.
* Qual foi o critério utilizado para validação do modelo? Por que escolheu utilizar este método?
	O modelo foi treinado utilizando dados de treino, validação e teste. Isso permitiu a criação de um modelo que fosse generalizável e que não sofresse de overfitting. A escolha do XGBoost foi feita devido a boa performance obtida durante as avaliações preliminares dos diferentes algoritmos testados.
	
* Quais evidências você possui de que seu modelo é suficientemente bom?
	> Depende do que "suficientemente bom" significa, já que sua interpretação é subjetiva. Mas, dado os resultados da análise, acredito que o modelo consiga performar muito bem com um resultado satisfatório na maioria dos casos.

Para visualizar a análise completa feita neste projeto, acesse este link:

* https://franklin390.github.io/Challenge_Airbnb_Rio_de_Janeiro/

---
