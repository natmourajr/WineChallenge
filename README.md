# WineChallenge
Repositório para a análise de qualidade do Vinho Verde

## Perguntas a serem respondidas

1 - Como foi a definição da sua estratégia de modelagem?

A estratégia de modelagem foi baseada na abordagem clássica de aprendizado de máquina o modelo CRIsP-DM. As estapas principais deste modelo são: entendimento dos dados (EDA), pré-processamento de dados, modelagem de dados e apresentação dos resultados. A etapa de entendimento foi bastante completa durante o briefing recebido por email. O pré-processamento foi baseado em extração de dados espúrios (strings em colunas númericas), que comprometeram a qualidade dos dados disponíveis para a modelagem. A modelagem foi baseada em uma modelagem supervisionada (classificação supervisionada) para mimetizar o comportamento das avaliações humanas a respeito dos vinhos. E a apresentação dos resultados foi baseada na matriz de confusão e acurácia dos modelos avaliados.

2 - Como foi definida a função de custo utilizada?

Durante o processo de EDA, foi observado que os dados não seguem uma distribuição gaussiana (normal). Assim sendo, os modelos lineares, provavelmente, não seriam o suficiente para a modelagem de classificação proposta. Assim sendo, escolhemos funções custo de acordo com a tecnologia de classificação empregada. Para árvores de decisão, a função da pureza do nó foi escolhida (GINI). Para as máquinas de vetor suporte, a norma 2 do vetor de separação (w) foi utilizada. Enquanto que para as redes neurais artificiais (MLP), foi utilizada a entropia cruzada para o treinamento. Outro ponto que pode ser reforçado é que, como os modelos SVM e MLP são não-lineares, e dependem muito da quantidade de eventos disponíveis por classes para serem treinados, um tratamento de treinamento desbalanceados foi realizado.

3 - Qual foi o critério utilizado na seleção do modelo final?

4 - Qual foi o critério utilizado para validação do modelo? Por que escolheu utilizar este método?

5 - Quais evidências você possui de que seu modelo é suficientemente bom?

