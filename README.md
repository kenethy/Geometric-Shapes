# Geometric Shapes

## BASE DE DADOS
2D Geometric Shapes

## PRÉ-PROCESSAMENTO
  1. Cada imagem da base de dados deve ser convertida de RGB para níveis de cinza.
  2. Se necessário, um filtro Gaussiano deve ser aplicado para a remoção de ruídos.
  3. As imagens em níveis de cinza devem ser binarizadas.

## EXTRAÇÃO DE CARACTERÍSTICAS
  1. Faz-se uso de vários tipos de características de contorno da forma (shape).
  2. Há justificativas no relatório de experimentos para a escolha das características selecionadas na avaliação.
  3. A justificativa é amparada com a experimentação realizada.

## EXPERIMENTOS
Os experimentos são executados de acordo com o esquema abaixo:
  1.  Executamos 10-fold cross-validation 5 vezes para cada base de dados, com cada uma das cinco execuções partindo de uma distribuição aleatória dos dados entre cada fold, resultando em um total de 50 experimentos por base de dados (10 x 5).
  2. Em cada um dos 50 experimentos, os conjuntos de treinamento e teste são mantidos o mesmo para cada algoritmo a ser testado (mesmo ponto de partida para cada modelo), de modo a obter-se uma avaliação justa dos resultados.  
  3. Os algoritmos que foram testados são: Árvore de Decisão, Naïve Bayes, K-Vizinhos Mais Próximos (K-NN), K-Vizinhos Mais Próximos 
Ponderado (W-K-NN), Máquina de Vetores de Suporte (SVM) e Regressão Logística, Rede Neural Artificial treinada por Backpropagation.
  4. Testamos o K-NN variando-se 3 vezes o número do parâmetro k, assim como o W-K-NN para os mesmos 3 valores de k escolhidos.
  5. A medida de distância adotada tanto no K-NN quanto no W-K-NN é a Distância Euclidiana.
  6. A SVM foi testada com as funções de kernel Linear e RBF.

## ANÁLISE EXPERIMENTAL
  1. A comparação é realizada em relação à Acurácia no Conjunto de Teste.
  2. Calculamos a média, o desvio padrão e a mediana da Acurácia do Conjunto de Testes para os 50 testes realizados para cada algoritmo em cada base de dados.
  3. Também incluímos a média, desvio padrão e mediana para o tempo de execução de cada experimento.
  4. Uma análise comparativa entre os algoritmos utilizados e suas variações é realizada, de modo a identificar qual abordagem pode ser considerada a mais confiável para a resolução dos problemas analisados.
  5. Essa análise é feita de forma empírica (baseado nas medidas obtidas) e através do uso de algum teste de hipóteses estatístico (t de Student, Teste de Friedman, ANOVA, etc.). Os testes de hipóteses são realizados apenas em relação à taxa de Acurácia do Conjunto de Teste.

## MATERIAIS GERADOS
1. Relatório de Experimentos (artigo)
2. Bases de Dados Geradas (imagens em níveis de cinza e binárias)
