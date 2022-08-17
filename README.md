# Teste-de-Hipoteses

Este repositório tem como objetivo detalhar o conteúdo estatístico de teste de Hipóteses. Teste de Hipóteses é uma matéria um pouco intimidadora para os estudantes de Estatística quando estes o vêem pela primeira vez. Entretanto é extremamente fundamental para amadurecer suas análises.

Sua finalidade como o prórpio nome diz é o de testar hipóteses. Quando queremos provar que a média salarial de um país mudou por exemplo, não podemos perguntar para todos os tantos milhões de habitantes daquele lugar, mas podemos pegar uma amostra e a partir daí criar uma hipótese para a população, e dizer se a média salarial aumentou ou não.

### Bibliotecas

from math import sqrt  
from scipy.stats import norm

### Teste Unicaudal

#### Para Achar o Z Crítico:

z_critico = norm.ppf( 1 - 0.05 ) | Intervalo de 95% de confiança |

#### Para Achar o Z:

Z = (X - μ)/(σ/sqrt(n))

#### Para Achar o Valor P:

##### Z

p_valor = norm.sf(z)

##### -Z

p_valor = 1 - norm.sf(z)

### Teste Bicaudal

#### Para achar o Z crítico

z_critico = norm.ppf( 1 - (0.05/2) ) | Intervalo de 95% de confiança |

#### Para Achar o Z:

Z = (X - μ)/(σ/sqrt(n))

#### Para Achar o Valor P:

##### Z

p_valor = 2 * (norm.sf(z))

##### -Z

p_valor = 2 * (1 - norm.sf(z))
