O projeto inteligência artificial e previsões tem como objetivo fazer uma análise de score de clientes de um banco.
Com isso é possível realizar previsões e classificar os clientes como bons ou ruins.
Passo a passo do projeto:

 • Importar a base de dados, realizei a importação da base de dados utilizando a bliblioteca pandas.
 
 • Verificar informações vazias, por padrão, realizei a verificação de valores vazios, com intuito mitigar problemas no decorrer da análise.
 
 • Fazer o tratamento na base de dados, foi necessário realizar o tratamento em algumas colunas com o tipo de informação “object” (texto), antes de prosseguir com a construção do projeto.
   Para isso utilizei o codificador "LabelEncoder" da biblioteca "sklearn", onde o codificador transforma as informações de texto em números para que fosse possível trabalhar com os 
   modelos de classificação, poi eles não funcionam com informações em texto.
   Utillizei cada informação de texto tipo: cientista, professor, mecânico e transformei em números: 0, 1, 2...
   A única coluna de texto que nós não alterei é a coluna de score_credito, pois é a coluna que usei para fazer as previsões. 
   Então transformei todas as outras e por fim basta verifiquei se todas as colunas foram de fato modificadas.
   
 • Selecionar as colunas de treino para o modelo, para selecionar as colunas separei a base de dados em 2, uma base de treino, para treinar o modelo para que ele consiga fazer as 
   previsões. E uma base de teste, que é a base que utilizei para ver como está fazendo essa previsão.
 
 • Treinar 2 modelos, depois de separar a base de dados em treino e teste, importei 2 modelos de classificação para treiná-los e verificar qual deles tem o melhor resultado para esse 
   caso, são eles: Modelo Árvore de Decisão e o Modelo Vizinhos Mais Próximos.
   Depois de importar os modelos, treinei cada uma deles utilizando a base de treino, dessa forma estavam preparados para serem testados com a base de teste e então foi possível comparar 
   o resultado entre os dois modelos. 
   
 • Verificar o melhor modelo, para avaliar a performance do modelo, utilizei a métrica da Acurácia para verificar quantas informações foram classificadas de forma correta.
   para calcular as previsãoes, utilizei os modelos, a árvore de decisão e o KNN, fazendo uso do .predict com cada um dos modelos.
   Feita a previsão, utilei a métrica de acurácia para verificar quanto cada um dos modelos acertou.
   Para a Árvore de Decisão tivemos uma acurácia de 82% enquanto que para o modelo KNN tivemos 73% de acurácia.
   Então para esse projeto em específico entre os dois modelos que nós temos, o modelo Árvore de Decisão teve o melhor resultado.
   Isso significa que o modelo serve para prever o score dos demais clientes.
   
 • Verificar quais as características mais importantes para definir o score do cliente, além de definir qual o modelo é melhor para fazer a classificação, é possível ainda utilizar esse 
   mesmo modelo para verificar quais as características mais importantes para definir o score de crédito.
   É uma forma de  melhorar ainda mais sua análise e mostrar para a empresa as características mais importantes para definir o score do cliente.
   Na base de dados utilizada aqui, por exemplo, as informações de divida_total, mix_credito e juros_empréstimo são características bem importantes.
   Então elas vão ajudar bastante na hora de definir o score do cliente, mais do que as outra características.

Nesse projeto atuei com  importação, tratamento de dados e análise de dados.
Com isso, foi possível treinar dois modelos de classificação para auxiliar na previsão dos dados.
Com isso, foi possível treinar dois modelos de classificação para auxiliar na previsão dos dados. Isso ajudaria a empresa a verificar de acordo com a  acurácia, quais os clientes que possuem um bom score.
Outro ponto, é que foi possível analisar quais as características mais importantes para definir esse score do cliente.
Foi possível perceber com esse projeto o quão importante é a análise de dados para as tomadas de decisões em  uma empresa, independente da área.
  
