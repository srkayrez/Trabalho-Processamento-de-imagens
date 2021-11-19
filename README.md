# DESENVOLVIMENTO DE UM SISTEMA BIOMÉTRICO CAPAZ DE
IDENTIFICAR ESPÉCIES DE PLANTAS A PARTIR DE SUAS FOLHAS

## Atividades práticas supervisionadas – APS VI – Trabalho apresentado como exigência para a avaliação do curso de Ciências da Computação da Universidade Paulista sob orientação de professores do semestre.

### Integrantes
GABRIEL EDUARDO JOIOSO
JOÃO VICTOR CAIRES
PAULO ADAM DA SILVA SANTANA
WELLINGTON JUNIOR CHELES

### Orientador
- Prof. Karem Daiane Marcomini

### Objetivo
  O objetivo do trabalho em grupo é estudar o conceito e o processo da engenharia de requisitos de software, e o impacto dessa atividade na qualidade do produto, pois os requisitos de software, as restrições estabelecidas pelos clientes e usuários do sistema definem os atributos de software desses requisitos. a fim de compreender corretamente e extrair as funções do sistema, ele deve Descrição detalhada.

### Introdução
  Iremos utilizar em nosso trabalho um método de aprendizado de máquina ou machine learning que é um subcampo da engenharia e ciência da computação que evoluiu do estudo de reconhecimentos de padrões, através de algoritmos que operam construindo um modelo a partir de inputs de amostras podendo fazer previsões ou decisões guiadas pelos dados ao invés de simplesmente seguir inflexíveis estáticas instruções programadas.

### Metodos utilizados
- KNN (K-Nearest Neighbors)
- Neural Network
- SVM (Support Vector Machine)

### KNN (K-Nearest Neighbors)
  O método para classificação por KNN consiste em atribuir uma classe a um elemento desconhecido usando a classe da maioria de seus k vizinhos mais próximos, segundo uma determinada distância (no espaço de atributos). Dada determinada amostra de uma classe desconhecida, calcula-se a sua distância diante de todas as amostras da base de conhecimento, selecionando as amostras k mais próximas. Dentre essas amostras, escolhemos a classe que é a maioria entre elas. Se tiver empate, utilizamos a classe mais próxima das maiorias empatadas. 
  Essa técnica tem um custo computacional elevado para bases de conhecimento com um grande número de amostras. Isso acontece por conta da necessidade do cálculo da função de distância da amostra desconhecida para todas as amostras contidas na base de conhecimento. 
  A métrica pode ser:
  Euclidiana: (“Linha reta”, distância entre dois pontos);
  Manhattan: (Soma das diferenças absolutas de todos os atributos);
  Máxima: (Maior das diferenças absolutas entre atributos);
  Mahalanobis (Distância entre o ponto e distribuição).
  Os pesos que você pode usar são:
  Uniforme: Todos os pontos em cada bairro são ponderados igualmente.
  Distância: Os vizinhos mais próximos de um ponto de consulta têm uma influência maior do que os vizinhos mais distantes.

![image](https://user-images.githubusercontent.com/78885438/142518097-ad921d82-25db-4923-ad3d-04d146664f4a.png)

O kNN usa o pré-processamento padrão quando nenhum outro pré-processador é fornecido. Ele os executa na seguinte ordem:
•	Remove instâncias com valores de destino desconhecidos;
•	Continua variáveis categóricas (com codificação one-hot);
•	Remove colunas vazias;
•	Imputa valores ausentes com valores médios;
•	Normaliza os dados centralizando a média e escalando para o desvio padrão de 1.

### Neural Network
  As redes neurais artificiais são um método para solucionar problemas através da simulação do cérebro humano, inclusive em seu comportamento, ou seja, aprendendo, errando e fazendo descobertas. São técnicas computacionais que apresentam um modelo inspirado na estrutura neural de organismos inteligentes e que adquirem conhecimento através da experiência.
  Elas possuem nós ou unidades de processamento. Cada unidade tem ligações para outras unidades, nas quais recebem e enviam sinais. Cada unidade pode ter uma memória local. Essas unidades são a simulação dos neurônios, recebendo e retransmitindo informações. Somando-se as entradas e retornando uma saída, caso esta seja maior que o valor da soma.
  Uma rede neural pode possuir uma ou mais camadas. Exemplificando com três camadas, poderíamos ter a camada de entrada, em que as unidades recebem os padrões; a camada intermediária, onde é feito o processamento e a retirada de características; e a camada de saída, que conclui e apresenta o resultado final. Quanto maior o número de camadas, melhor a capacidade de aprendizado.
  A camada de entrada tem que ter uma unidade especial conhecida como bias, usada para aumentar os graus de liberdade, permitindo assim uma melhor adaptação por parte da rede neural, ao conhecimento a ela fornecido.
  Em termos mais técnicos, o número de camadas define a capacidade de representação das relações entre o espaço de entrada e o de saída. A inexistência da camada intermediária, característica do modelo perceptron, condiciona-o a representar bem somente relações linearmente independentes. A existência de camadas intermediárias, característica do modelo perceptron de múltipla camada (PMC), retira tal limitação. Se tiver apenas uma camada intermediária, o PMC pode representar (com qualquer grau de aproximação, por menor que seja) qualquer função contínua. Duas ou mais camadas ampliam o universo de representação a qualquer função, contínua ou não.
  As redes neurais artificiais, seguindo a tradição americana, estão muito associadas à adaptação de conexões (sinapses) entre neurônios, o conexionismo. Cabe registrar a existência de modelos nos quais as conexões não são adaptadas, mas apenas transmitem estimulação entre neurônios. Tais modelos são chamados redes neurais sem pesos (do inglês, weightless neural networks). Para completar, existem modelos em que as sinapses não são adaptadas, mas sim calculadas previamente, geralmente servindo a tarefas de otimização.
	A Rede Neural usa o pré-processamento padrão quando nenhum outro pré-processador é fornecido. Ele os executa na seguinte ordem:
•	Remove instâncias com valores de destino desconhecidos;
•	Continua variáveis categóricas (com codificação one-hot);
•	Remove colunas vazias;
•	Imputa valores ausentes com valores médios;
•	Normaliza os dados centralizando a média e escalando para o desvio padrão de 1.

![image](https://user-images.githubusercontent.com/78885438/142518229-abb0dc40-24c6-404c-a1e7-c6f06e3abf95.png)

### SVM (Support Vector Machine)
  SVM desenvolvido por Vapnik em 2013, é um método de aprendizagem de máquina no qual propõe a criação de um hiperplano como superfície de decisão. 
  Esse hiperplano tem que apresentar a separação ideal entre duas classes, maximizando a distância entre os pontos mais próximos entre a classe e o hiperplano. Esses pontos são chamados de elementos de borda e os vetores de suporte são as distâncias entre os elementos de borda e o hiperplano.
  Baseando-se na Teoria de Aprendizagem Estatística como sua estratégia de treinamento e na Teoria de Otimização para encontrar o hiperplano. Tem como vantagem de ser capaz de trabalhar com um grande volume de amostras e rapidez na classificação, porem o tempo de treinamento pode apresentar custo computacional considerável para bases com um grande número de amostras.
  As máquinas de vetor de suporte mapeiam entradas para espaços de recursos de dimensões superiores.
  Entradas:
•	Dados: Conjunto de dados de entrada;
•	Pré-processador: Método (s) de pré-processamento.
Saídas:
•	Aluno: Algoritmo de aprendizagem de regressão linear;
•	Modelo: Modelo treinado;
•	Vetores de suporte: Instâncias usadas como vetores de suporte.

  Máquina de vetores de suporte (SVM) é uma técnica de aprendizado de máquina que separa o espaço de atributos com um hiperplano, maximizando assim a margem entre as instâncias de diferentes classes ou valores de classe.
  A técnica geralmente produz resultados de desempenho preditivos supremos. Orange incorpora uma implementação popular de SVM do pacote LIBSVM. Este widget é sua interface gráfica com o usuário.
  Para tarefas de regressão, o SVM executa a regressão linear em um espaço de recursos de alta dimensão usando uma perda insensível a ε. A precisão de sua estimativa depende de um bom ajuste dos parâmetros C, ε e kernel. O widget gera previsões de classe com base em uma regressão SVM.

![image](https://user-images.githubusercontent.com/78885438/142518276-eba65eb1-506a-4f5a-84df-14347151f28e.png)

O SVM usa o pré-processamento padrão quando nenhum outro pré-processador é fornecido. Ele os executa na seguinte ordem:
•	Remove instâncias com valores de destino desconhecidos;
•	Continua variáveis categóricas (com codificação one-hot);
•	Remove colunas vazias;
•	Imputa valores ausentes com valores médios;
•	Para classificação, o SVM também normaliza dados densos e dimensiona dados esparsos.
 
### TESTE E PONTUAÇÃO
  Testa algoritmos de aprendizagem em dados.
  Entradas:
•	Dados: Conjunto de dados de entrada;
•	Dados de teste: Dados separados para teste;
•	Aprendiz: Algoritmo (s) de aprendizagem.
  Saídas:
  Resultados dos algoritmos de classificação de teste:
  O widget testa algoritmos de aprendizagem. Diferentes esquemas de amostragem estão disponíveis, incluindo o uso de dados de teste separados. O widget faz duas coisas.
  Primeiro, ele mostra uma tabela com diferentes medidas de desempenho do classificador, como precisão de classificação e área sob a curva. Em segundo lugar, ele produz resultados de avaliação, que podem ser usados por outros widgets para analisar o desempenho de classificadores, como ROC Analysis ou Confusion Matrix.
  O sinal de aprendizado tem uma propriedade incomum: pode ser conectado a mais de um widget para testar vários alunos com os mesmos procedimentos.

![image](https://user-images.githubusercontent.com/78885438/142518430-6522954f-1080-4dbf-9d52-a1ef0e97e5c8.png)

  O widget oferece suporte a vários métodos de amostragem.

###Validação cruzada
  Divide os dados em um determinado número de dobras (geralmente 5 ou 10). O algoritmo é testado apresentando exemplos de uma dobra de cada vez; o modelo é induzido a partir de outras dobras e os exemplos da dobra estendida são classificados. Isso é repetido para todas as dobras.

### A validação cruzada por recurso
  Realiza validação cruzada, mas as dobras são definidas pelo recurso categórico selecionado de meta-recursos.

### Amostragem aleatória:
  Divide aleatoriamente os dados no conjunto de treinamento e teste na proporção dada (por exemplo, 70:30); todo o procedimento é repetido por um determinado número de vezes.

###Deixar um de fora
  É semelhante, mas mantém uma instância de cada vez, induzindo o modelo de todas as outras e, em seguida, classificando as instâncias suspensas. Este método é obviamente muito estável, confiável e muito lento.

### O teste em dados
  De trem usa todo o conjunto de dados para treinamento e, em seguida, para teste. Esse método quase sempre dá resultados errados.

### Teste em dados de teste
  Os métodos acima usam os dados do sinal de dados apenas. Para inserir outro conjunto de dados com exemplos de teste (por exemplo, de outro arquivo ou alguns dados selecionados em outro widget), selecionamos o sinal Separate Test Data no canal de comunicação e selecione Test on test data.
  Para classificação, a classe de destino pode ser selecionada na parte inferior do widget. Quando a classe de destino é (média sobre as classes), os métodos retornam pontuações que são médias ponderadas de todas as classes. Por exemplo, no caso do classificador com 3 classes, as pontuações são calculadas para a classe 1 como classe de destino, a classe 2 como classe de destino e a classe 3 como classe de destino. Essas pontuações são calculadas em média com pesos com base no tamanho da classe para recuperar a pontuação final.
  O widget calculará várias estatísticas de desempenho. Alguns são mostrados por padrão.
  Para classificação, a classe de destino pode ser selecionada na parte inferior do widget. Quando a classe de destino é (média sobre as classes), os métodos retornam pontuações que são médias ponderadas de todas as classes. Por exemplo, no caso do classificador com 3 classes, as pontuações são calculadas para a classe 1 como classe de destino, a classe 2 como classe de destino e a classe 3 como classe de destino. Essas pontuações são calculadas em média com pesos com base no tamanho da classe para recuperar a pontuação final.
  O widget calculará várias estatísticas de desempenho. Alguns são mostrados por padrão. Para ver mais, basta clicar com o botão direito no cabeçalho e selecionar a estatística desejada.

![image](https://user-images.githubusercontent.com/78885438/142518589-ee466413-76af-451f-b739-cf39941684c3.png)

  A área sob ROC - É a área sob a curva de operação do receptor.
  A precisão da classificação - É a proporção de exemplos classificados corretamente.
  F-1 - É uma média harmônica ponderada de precisão e recall.
  A precisão - É a proporção de verdadeiros positivos entre as ocorrências classificadas como positivas.
  O recall - É a proporção de verdadeiros positivos entre todas as instâncias positivas nos dados.
  A especificidade - É a proporção de verdadeiros negativos entre todas as instâncias negativas.
  LogLoss – É a perda de entropia cruzada, leva em consideração a incerteza de sua previsão com base em quanto ela varia do rótulo real.
  Tempo de treinamento - Tempo cumulativo em segundos usado para modelos de treinamento.
  Tempo de teste - Tempo cumulativo em segundos usado para modelos de teste.

### MATRIZ DE CONFUSÃO
  Mostra proporções entre a classe prevista e a real.
  Entradas: Resultados da avaliação: resultados dos algoritmos de classificação de teste.
  Saídas: Dados selecionados: subconjunto de dados selecionado da matriz de confusão.
  Dados: Dados com as informações adicionais sobre se uma instância de dados foi selecionada.
  A Matriz de confusão fornece o número/proporção de instâncias entre a classe prevista e a real. A seleção dos elementos na matriz alimenta as instâncias correspondentes no sinal de saída. Dessa forma, pode-se observar quais instâncias específicas foram erroneamente classificadas e como.

![image](https://user-images.githubusercontent.com/78885438/142518626-14c3865c-62ff-44ae-abf2-ace7fa8a7b35.png)
![image](https://user-images.githubusercontent.com/78885438/142518640-e096aba9-7a99-4769-b024-909ab72d3e25.png)
![image](https://user-images.githubusercontent.com/78885438/142518649-a48a8d92-07b4-4bb3-9097-c7ee03ba2e80.png)

  Quando os resultados da avaliação contêm dados sobre vários algoritmos de aprendizagem, temos que escolher um na caixa de aprendizado. O instantâneo mostra a matriz de confusão para os modelos SVM, Neural Network e kNN treinados e testados nos dados das folhas.
  Cada linha corresponde a uma classe correta, enquanto as colunas representam as classes previstas.  Em Mostrar, selecionamos quais dados gostaríamos de ver na matriz. O número de instâncias mostra as instâncias classificadas de forma correta e incorreta numericamente.
  Em Selecionar, você pode escolher a saída desejada.
  Correto: Envia todas as instâncias classificadas corretamente para a saída selecionando a diagonal da matriz.
  Misclassified: Seleciona as instâncias mal classificadas.
  Nenhum: Anula a seleção. Como mencionado antes, também se pode selecionar células individuais da tabela para selecionar tipos específicos de ocorrências classificadas incorretamente (por exemplo, as versicolors classificadas como virginicae).
  Ao enviar instâncias selecionadas, o widget pode adicionar novos atributos, como classes preditas ou suas probabilidades, se as opções correspondentes Predições e / ou Probabilidades estiverem marcadas.

  O widget exibe todas as alterações se Enviar automaticamente estiver marcado. Caso contrário, o usuário precisará clicar em Enviar selecionados para confirmar as alterações.
  Test & Score obtém os dados de File e três algoritmos de aprendizagem SVM, Neural Network, kNN. Ele executa validação cruzada ou alguns outros procedimentos de treinamento e teste para obter previsões de classe por ambos os algoritmos para todas (ou algumas) instâncias de dados. Os resultados do teste são alimentados na Matriz de confusão, onde podemos observar quantas instâncias foram classificadas incorretamente e de que maneira.
  Na saída, usamos Data Table para mostrar as instâncias que selecionamos na matriz de confusão. Se, por exemplo, clicarmos em Misclassified, a tabela conterá todas as instâncias que foram mal classificadas pelo método selecionado.
  O gráfico de dispersão obtém dois conjuntos de dados. A partir do widget Arquivo, ele obtém os dados completos, enquanto a matriz de confusão envia apenas os dados selecionados, classificações erradas, por exemplo. O gráfico de dispersão mostrará todos os dados, com símbolos em negrito representando os dados selecionados.

### Distribuições
  Exibe distribuições de valor para um único atributo. 
  Entradas: Dados: conjunto de dados de entrada.
  Saídas: Dados selecionados: instâncias selecionadas do gráfico Dados: dados com uma coluna adicional que mostra se uma instância está selecionada Dados do histograma: bins e contagens de instâncias do histograma O widget Distribuições exibe a distribuição de valor de atributos discretos ou contínuos. Se os dados contiverem uma variável de classe, as distribuições podem ser condicionadas à classe. 
  O gráfico mostra quantas vezes (por exemplo, em quantas instâncias) cada valor de atributo aparece nos dados. Se os dados contiverem uma variável de classe, as distribuições de classe para cada um dos valores de atributo serão exibidas (como no instantâneo abaixo). Para criar este gráfico, usamos o conjunto de dados Zoo.

![image](https://user-images.githubusercontent.com/78885438/142518704-8da0ea85-8816-4f39-9265-66bb7597c28b.png)

  Uma lista de variáveis para exibição. Classifique as categorias por frequência, ordena os valores exibidos por frequência.
  Defina a largura da bandeja com o controle deslizante. A escala de precisão é definida para intervalos sensíveis. A distribuição ajustada ajusta a distribuição selecionada ao gráfico. As opções são: Normal, Beta, Gama, Rayleigh, Pareto, Exponencial, Densidade do kernel.
  Colunas:
  Dividido por exibe distribuições de valor para instâncias de uma determinada classe.
  As colunas da pilha exibem uma coluna por compartimento, colorida por proporções de valores de classe.
  Mostrar probabilidades mostra probabilidades de valores de classe na variável selecionada.
  Mostrar distribuição cumulativa empilha frequências cumulativas

### Gráfico de calibração (Calibration Plot)
  Mostra a correspondência entre as previsões de probabilidade dos classificadores e as probabilidades reais da classe.
  Entradas:
  Resultados da avaliação: resultados dos algoritmos de classificação de teste
  Os gráficos de calibração representam as probabilidades da classe em relação àquelas previstas pelo (s) classificador (es).
  No momento, o único widget que fornece o tipo certo de sinal necessário para o gráfico de calibração é o Teste e pontuação. O Gráfico de Calibração, portanto, sempre seguirá Teste e Pontuação e, como não tem saídas, nenhum outro widget o segue.
  Aqui está um exemplo típico, onde comparamos três classificadores (a saber, SVM, Neural Network e kNN) e os inserimos em Teste e Pontuação. Usamos o conjunto de dados do     Titanic. Teste e pontuação exibe os resultados da avaliação para cada classificador. Em seguida, desenhamos os widgets Calibration Plot e ROC Analysis de Test & Score para analisar melhor o desempenho dos classificadores. O gráfico de calibração permite que você veja a precisão da previsão das probabilidades de classe em um gráfico.

![image](https://user-images.githubusercontent.com/78885438/142518739-033ebda8-9ef4-4907-b694-e163875b4b7a.png)
![image](https://user-images.githubusercontent.com/78885438/142518750-b33ae6d3-7d4f-416b-915e-7ff3871ae64b.png)
![image](https://user-images.githubusercontent.com/78885438/142518763-8eda1dd9-73f0-4e38-913f-b0a5f65ef222.png)

### previsões (predictions)
  Mostra as previsões dos modelos sobre os dados.
  Entradas:
  Dados: Conjunto de dados de entrada.
  Preditores: Preditores a serem usados nos dados.
  Saídas:
  Previsões: Dados com previsões adicionadas.
  Resultados da avaliação: resultados dos algoritmos de classificação de teste
  O widget recebe um conjunto de dados e um ou mais preditores (modelos preditivos, não algoritmos de aprendizagem - veja o exemplo abaixo). Ele produz os dados e as previsões.
  O widget mostra as probabilidades e decisões finais dos modelos preditivos. A saída do widget é outro conjunto de dados, onde as previsões são anexadas como novos atributos meta. Você pode selecionar quais recursos deseja produzir (dados originais, previsões, probabilidades).
  O resultado pode ser observado em uma Tabela de Dados. Se os dados previstos incluem valores de classe verdadeiros, o resultado da previsão também pode ser observado em uma Matriz de confusão.

![image](https://user-images.githubusercontent.com/78885438/142518841-d5cef390-4e42-47ec-ba5d-34b1dcd2f6ff.png)

### Tabela de dados
  Exibe dados de valor de atributo em uma planilha.
  Entradas:
  Dados: Conjunto de dados de entrada.

  Saídas:
  Dados selecionados: Instâncias selecionadas da tabela.
  O widget Tabela de dados recebe um ou mais conjuntos de dados em sua entrada e os apresenta como uma planilha. As instâncias de dados podem ser classificadas por valores de  atributo. O widget também oferece suporte à seleção manual de instâncias de dados.

![image](https://user-images.githubusercontent.com/78885438/142518863-f5582c90-f726-4fb0-b9a8-059ae881a01c.png)

  O nome do conjunto de dados (geralmente o arquivo de dados de entrada). As instâncias de dados estão em linhas e seus valores de atributos em colunas. Neste exemplo, o conjunto de dados é classificado pelo atributo “comprimento da sépala”.
  Informações sobre o tamanho do conjunto de dados atual e número e tipos de atributos.
  Valores de atributos contínuos podem ser visualizados com barras; as cores podem ser atribuídas a diferentes classes.
  As instâncias de dados (linhas) podem ser selecionadas e enviadas para o canal de saída do widget.
  Use o botão Restaurar pedido original para reordenar as instâncias de dados após a classificação baseada em atributo.
  Enquanto o envio automático estiver ativado, todas as alterações serão comunicadas automaticamente a outros widgets. Caso contrário, pressione Enviar Linhas Selecionadas.

### Projeto

![image](https://user-images.githubusercontent.com/78885438/142518898-74a9fc78-f617-4e1c-b922-fd012031f04e.png)

  Primeiramente nós importamos as pastas com as amostras em imagem das plantas que foram utilizadas para realizar o aprendizado de máquina, em seguida o projeto separa as amostrar em dados biométricos.
  Esses dados são enviados para o “Test and Score” para realizar o teste e aprendizado de máquina com o os métodos de classificação (kNN, Neural Network e SVM). Depois é gerada a Matriz de Confusão que é responsável por fornecer o número/proporção de instâncias entre a classe prevista e a real. Será gerado os gráficos de distribuição que mostra quantas vezes (por exemplo, em quantas instâncias) cada valor de atributo aparece nos dados. Se os dados contiverem uma variável de classe, as distribuições de classe para cada um dos valores de atributo serão exibidas.
  Em seguida foi gerado o Calibration Plot que mostra a correspondência entre as previsões de probabilidade dos classificadores e as probabilidades reais da classe. Após isso geramos as predições que mostra as previsões dos modelos sobre os dados.

### Referencias
GANDHI, Rohith . Support Vector Machine — Introduction to Machine Learning Algorithms: SVM model from scratch. towardsdatascience. 2018. Disponível em: https://towardsdatascience.com/support-vector-machine-introduction-to-machine-learning-algorithms-934a444fca47?gi=10fa8891ff31. Acesso em: 19 out. 2021.
JOSÉ, Italo. NN (K-Nearest Neighbors): Como funciona?. medium. 2018. Disponível em: https://medium.com/brasil-ai/knn-k-nearest-neighbors-1-e140c82e9c4e. Acesso em: 15 out. 2021.
K-NEAREST Neighbor(KNN) Algorithm for Machine Learning. javatpoint. Disponível em: https://www.javatpoint.com/k-nearest-neighbor-algorithm-for-machine-learning . Acesso em: 18 out. 2021.
MATRIZ de confusão. wikipedia. Disponível em: https://pt.wikipedia.org/wiki/Matriz_de_confus%C3%A3o. Acesso em: 19 out. 2021.
MÁQUINA de vetores de suporte. Wikipedia. Disponível em: https://pt.wikipedia.org/wiki/M%C3%A1quina_de_vetores_de_suporte. Acesso em: 19 out. 2021.
NEURAL network. wikipedia. Disponível em: https://en.wikipedia.org/wiki/Neural_network. Acesso em: 18 out. 2021.
ORANGEDATAMINING. Documentation. Disponível em: https://orangedatamining.com/docs/. Acesso em: 22 out. 2021.
PRECISION and recall. wikipedia. Disponível em: https://en.wikipedia.org/wiki/Precision_and_recall. Acesso em: 20 out. 2021.
REDE neural artificial. Rede neural artificial. Disponível em: https://pt.wikipedia.org/wiki/Rede_neural_artificial. Acesso em: 19 out. 2021.
STANKEVIX, Gabriel . Analise exploratória de Dados: Uma aplicação do pensamento estatístico em Python. medium. 2020. Disponível em: https://medium.com/@gabriel.stankevix/analise-explorat%C3%B3ria-de-dados-732007ddbfaf. Acesso em: 20 out. 2021.
VAZ, Arthur Lamblet. Neural Network — Deep Learning — Parte 4: Introdução Teórica. medium. 2019. Disponível em: https://medium.com/data-hackers/neural-network-deep-learning-parte-4-introdu%C3%A7%C3%A3o-te%C3%B3rica-db45ebd77029. Acesso em: 18 out. 2021.
WICKLIN, Rick . Calibration plots in SAS. sas. 2018. Disponível em: https://blogs.sas.com/content/iml/2018/05/14/calibration-plots-in-sas.html. Acesso em: 20 out. 2021.

### Nota: (aguardando)
### Comentário do orientador: (aguardando)

<p align="center"><i>“Não importa o que aconteça, continue a nadar”</i> <br>
(WALTERS; GRAHAM, Procurando Nemo, 2003).</p>

<p align="center">Atividade concluída em 18/11/2021.</p>

