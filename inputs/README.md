Projeto de Machine Learning: 
Previsão de Ausência de Funcionários

Este projeto foi minha primeira experiência prática com Machine Learning e teve como objetivo criar um modelo capaz de prever a ausência de funcionários em uma empresa, 
com base em variáveis como:

-Dia da semana

-Proximidade de feriados ou férias

-Estação do ano


Entre outras variáveis relevantes para o contexto empresarial

Etapas do Projeto
1. Geração dos dados
Com a ajuda do ChatGPT, construí uma base de dados fictícia com 300 funcionários, simulando diferentes cenários de presença e ausência.
A ideia foi criar dados realistas o suficiente para treinar o modelo e entender os padrões de comportamento ao longo do tempo.

2. Pré-processamento e estruturação da pipeline
Neste passo, foi criada uma pipeline de Machine Learning que organiza as etapas de preparação e modelagem.
Os principais campos utilizados na pipeline foram:

-dia_da_semana (ex: segunda, terça...)

-feriado_proximo (booleano: sim/não)

-ferias_agendadas

-estacao_ano

-departamento

-presenca (variável alvo: presente/ausente)
![5](https://github.com/user-attachments/assets/3ac98269-adf5-45b5-b67b-8fa1a8f57602)



3. Treinamento do modelo
O modelo utilizado foi o Two-Class Logistic Regression, uma técnica de classificação binária que tenta prever a probabilidade de um funcionário faltar ou não no dia seguinte.
![3](https://github.com/user-attachments/assets/b99a3a2f-c5bb-4211-a90d-0265132a9daa)


4. Avaliação do Modelo
Após o treinamento, o modelo foi avaliado utilizando as seguintes métricas:

-Acurácia: O modelo obteve uma acurácia de 75%, o que significa que ele acertou 75% das previsões, considerando todos os casos.

-AUC (Área sob a Curva): A AUC foi de 0.5675, indicando que o modelo tem uma capacidade moderada de distinguir entre as classes "falta" e "não falta".

-F1-score: O F1-score foi 0.189, indicando que o equilíbrio entre precisão e recall está abaixo do ideal, possivelmente devido ao desbalanceamento entre as classes.

-Precisão: A precisão foi 0.2917, o que significa que, quando o modelo previu uma ausência, ele estava correto aproximadamente 29% das vezes.

-Recall: O recall foi 0.14, o que sugere que o modelo conseguiu identificar apenas 14% das ausências reais, deixando muitas faltas passarem despercebidas.
![4](https://github.com/user-attachments/assets/50afab0d-9120-4c33-8619-69894e316d29)



Durante o desafio, aprendi que quanto mais dados o sistema possuir, mais acertivo pode ser o resultado.

Apresar de a taxa de acerto não ter sido tão boa, certamento o aprendizado foi gigante, e pretendo continuar trabalhando neste projeto para aperfeiçoa-lo ainda mais.
