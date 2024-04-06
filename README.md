<h1>Trabalhando com Machine Learning na Prática no Azure ML</h1>
Desafio sobre aprendizado de máquina: Criar um modelo de previsão com seus devidos pontos de extremidade configurados.

<h2>Workspace</h2>
Para criar o espaço de trabalho, treinar o modelo, avaliar o melhor modelo e testar, basta seguir o passo a passo contido na página abaixo.</br>
https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html

<h2>Modelo de previsão e pontos de extremidade</h2>
Neste trabalho o melhor modelo foi VotingEnsemble coforme mostrado a seguir.

<img src="Imagens/AzureML-1.png">
<img src="Imagens/AzureML-2.png">

O teste do ponto de extremidade utilizado foi o seguinte:
<pre>
   {
   "Inputs": { 
     "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]    
   },   
   "GlobalParameters": 1.0
 }
</pre>

E o resultado foi o seguinte:
<pre>
  {
    "Results": [
      364.78935594629985
    ]
  }
</pre>

<img src="Imagens/AzureML-3.png">
