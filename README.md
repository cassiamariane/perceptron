# Perceptron
O algoritmo Perceptron é um algoritmo de aprendizado supervisionado usado para tarefas de classificação binária. Ele faz uma simulação do funcionamento de um único neurônio no cérebro. Dado um conjunto de características de entrada e sua saída alvo correspondente, o algoritmo ajusta os pesos para classificar as entradas em uma de duas categorias.  Nessa implementação, o algoritmo aprende a operação lógica OR com pesos inicializados aleatoriamente.

---

## Algoritmo
1. Inicialização
2. Aprendizado Iterativo:
* Para cada exemplo de treinamento:
  * É calculada a saída prevista com base nos pesos atuais.
  * Os pesos são atualizados se a previsão estiver incorreta.
3. Convergência: O processo de aprendizado é repetido até que um o neurônio aprenda a operação OR (verdadeiro (1) se pelo menos uma das entradas for verdadeira ou falso (0) se todas forem falsas) ou atingir um número máximo de iterações.

---

### Fluxo da implementação + Dicionário de variáveis
* Dados: Os dados de entrada consistem em quatro exemplos representando a tabela verdade da operação OR.
* 
| A | B | A + B |
| - | - | ----- |
| 0 | 0 |   0   |
| 0 | 1 |   1   |
| 1 | 0 |   1   |
| 1 | 1 |   1   |

* Taxa de Aprendizado (lr): Definida para controlar o tamanho do passo durante as atualizações de peso.
* Pesos (w): Inicializados com pequenos valores aleatórios.
* Iterações: O algoritmo itera sobre os dados, ajustando os pesos até convergir ou atingir um número máximo de iterações.
* Atualização de Peso: Os pesos são atualizados com base em erros de previsão usando a regra de aprendizado do Perceptron.
* Visualização: Após cada iteração, a fronteira de decisão é plotada para visualizar a classificação aprendida.
O algoritmo continua iterando até que todas as saídas sejam classificadas corretamente ou até atingir um número máximo de iterações. Se todas as saídas forem classificadas corretamente, o algoritmo para, indicando aprendizado bem-sucedido da função lógica OR.

---

Para mais detalhes sobre a implementação, consulte [Perceptron](https://github.com/cassiamariane/perceptron/perceptron.ipynb)

---
## Tecnologias utilizadas
|                           |                         |                                     |
| ------------------------- | ----------------------- | ----------------------------------- |
| ![Python](img/python.svg) | ![NumPy](img/numpy.png) | ![Matplotlib](img/matplotlib.png) |
