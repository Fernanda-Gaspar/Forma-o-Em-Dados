<h1 align="center"> 🚀 Desafio Cientista de dados da INDICIUM para o Processo Seletivo - Lighthouse Programa De Formação Em Dados 🚀 </h1>

## 💻 Sobre o projeto

Seu objetivo é identificar quais máquinas apresentam potencial de falha tendo como base dados extraídos através de sensores durante o processo de manufatura. 

Para realizar a tarefa, respondi as seguintes perguntas: 
1. Quais variáveis e/ou suas transformações você utilizou e por quê? 

  Utilizei a coluna failure_type como variável de destino e realizei as transformações a partir dela. Além disso, no mapa de calor, você pode observar    rapidamente quais variáveis estão positivamente ou negativamente correlacionadas umas com as outras e em que grau. Isso pode ser útil para identificar quais recursos podem ser mais úteis para construir um modelo preditivo.
  
3. Qual tipo de problema estamos resolvendo (regressão, classificação)? 

  Estamos resolvendo um problema de classificação (multiclassificação baseado em árvore).
  
5. Qual modelo melhor se aproxima dos dados e quais seus prós e contras?

  Existem vários modelos para implementar uma solução de manutenção preditiva, dependendo do tipo de equipamento que está sendo monitorado e dos recursos disponíveis. Temos por exemplo, três modelos de previsão: 
  
  - Monitoramento baseado em condição: envolve o monitoramento contínuo da condição do equipamento usando sensores. Quando determinados limites ou condições são atendidos, um alerta é acionado ou medidas corretivas são lançadas. O objetivo é reduzir o risco de falha. Por exemplo, se a temperatura de um motor exceder um determinado nível, isso pode indicar que o motor está prestes a falhar.
  - Modelagem preditiva: essa abordagem envolve o uso de algoritmos de aprendizado de máquina para analisar dados históricos de tempo de vida sobre o equipamento para identificar padrões que podem indicar uma falha iminente. Isso pode ser feito usando dados de sensores, bem como dados operacionais e registros de manutenção. Quando os dados históricos ou de falha não estiverem disponíveis, um modelo de degradação pode ser criado para estimar os tempos de falha com base em um valor limite. Essa abordagem é frequentemente usada quando há dados limitados disponíveis. 
  - Algoritmos de prognóstico: usando dados de sensores e outras fontes, os algoritmos de prognóstico podem prever a vida útil restante de um equipamento. Essas informações podem ajudar as organizações a determinar a probabilidade de uma avaria e planejar substituições ou atividades de manutenção. Ao entender melhor o equipamento, as organizações podem potencialmente estender os ciclos de manutenção, o que pode reduzir os custos de substituições e manutenção. E este modelo foi o escolhido para fazer a multiclassificação.

7. Qual medida de performance do modelo foi escolhida e por quê?

 Para avaliar o desempenho do modelo utilizei três etapas: 
 - Pontuação do modelo
 - Validação cruzada
 - Matriz de multiclasse

## 🎲 Obtenção de dados
Utilizei dois tipos de dados para uma melhor previsão e comparação:

São fornecidos dois datasets: um dataset chamado desafio_manutencao_preditiva_treino composto por 6667 linhas, 9 colunas de informação (features) e a variável a ser prevista (“failure_type”). O segundo dataset chamado de desafio_manutencao_preditiva_teste possui 3333 linhas e 8 colunas e não possui a coluna “failure_type”. O objetivo é prever essa coluna a partir dos dados enviados.

## 🛠 Tecnologias

As seguintes ferramentas foram usadas na construção do projeto:

- [Python](https://www.python.org)
- [Jupyer Notebook](https://jupyter.org)

## 🚀 Como executar o projeto

1. Crie e ative um ambiente virtual
2. Clone este repositório https://github.com/Fernanda-Gaspar/Previsao_de_Falha
3. Acesse a pasta do projeto no terminal/cmd
4. Execute o arquivo requirements.txt
5. Instale um jupyter kernel para esse ambiente virtual:
## ipython kernel install --user --name=nome_do_ambiente_virtual
5. Selecione o kernel instalado quando estiver usando o jupyter notebook no ambiente virtual
6. No jupyter notebook execute todas as células a partir do menu

- [Previsão](https://github.com/Fernanda-Gaspar/Previsao_de_Falha/blob/main/previsao.ipynb)

Feito com ❤️ por Fernanda Gaspar 👋🏽
