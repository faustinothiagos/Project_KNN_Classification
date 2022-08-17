# KNN_Classification

<div align="center">
<img src="https://user-images.githubusercontent.com/97195240/185261921-1814e228-71ff-49d7-a789-b764720da0ab.png" width="400px" />
</div>

<a id="section_knn"></a>

## Marco teórico

##  K-Nearest Neighbor Classification

KNN é um dos algoritmos mais simples em aprendizagem de máquina. A famosa frase "diga-me com quem você anda e eu direi quem você é" talvez seja a melhor explicação informal do algoritmo. Basicamente, KNN se encarrega de memorizar a localização de cada amostra do conjunto de treinamento de acordo com os valores de suas características. Ao receber novos dados, ele os coloca na posição do espaço que lhes corresponde de acordo com suas características e encontra os k vizinhos mais próximos (k é um hiperparâmetro do modelo que define quantos vizinhos devem ser considerados ao fazer as previsões) . Esses vizinhos ou pontos próximos são as amostras do conjunto de treinamento que são mais semelhantes à observação que queremos classificar. Uma vez identificados os k vizinhos mais próximos, cada um deles contribui com um "voto" para a classe a que pertence. A previsão é determinada pela classe majoritária entre os k vizinhos mais próximos.

<div id="caja9" style="float:left;width: 100%;">
  
  <div style="float:left;width: 85%;"><label><b>Mais formalmente,o algoritmo KNN se encarrega de calcular uma probabilidade para cada classe <i>c</i>:</b>
      
$$ p(y = c|x, D, k) = \frac{1}{k} \sum_{i \in N_k(x, D)} I(y_i = c) $$
      
onde $x$ é o vetor de features dos dados a serem previstos, $D$ é o conjunto de dados de treinamento, k é o número de vizinhos a serem avaliados em $D$, $N_k (x, D) $são os índices dos k vizinhos mais próximo.
    
A classe com maior probabilidade é aquela que será prevista.
</b><br></label></div>

- [Acessar a documentação do Scikit-learn](https://scikit-learn.org/stable/modules/neighbors.html)
    
Uso do modelo KNN de classificação em Python para analisar um DataSet do molusco abalone.
