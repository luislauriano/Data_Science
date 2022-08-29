[![author](https://img.shields.io/badge/author-LuisVinicius-red.svg)](https://www.linkedin.com/in/luislauriano/) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-365/) [![GPLv3 license](https://img.shields.io/badge/License-GPLv3-blue.svg)](http://perso.crans.org/besson/LICENSE.html) [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/luislauriano/data_science)

# Projeto de machine learning para prever possíveis resultados de jogos da copa do mundo de 2022


Esse é um projeto para fins de curiosidade e estudo de machine learning, com o objetivo de que seja possível desenvolver um modelo capaz de prever possíveis resultados das partidas da copa do mundo de 2022, até chegar no resultado do grande vencedor do campeonato.

De que forma isso foi realizado? A partir da análise dos dados e entendimento do problema, ficou claro que em média o time da casa marca mais gols e o número de gols por partida segue uma distribuição de poisson, seguindo de acordo com a lógica de partidas do futebol. Então, foi pensado em construir um Modelo Linear Generalizado com base na regressão de poisson, tendo em vista, que a regressão de poisson busca prever um valor de contagem e para esse problema pode-se prever a quantidade de gols por partida, para conseguir chegar no possível vencendor da partida e as chances de vitória, empate e derrota.

<p align="center">
  <img src="http://sportinsider.com.br/wp-content/uploads/2022/05/copa-do-mundo-do-catar-2022-1.jpg" width = 100%>
</p>


---

Após o projeto ter sido finalizado, a ideia foi também construir uma aplicação com Streamlit para o modelo e realizar o seu deploy com heroku, para que outras pessoas possam utilizar o modelo construído e obter seus possíveis resultados para qualquer partida do campeonato, além de poder simular como possivelmente ficaria a fase de grupos após os jogos e a fase mata-mata, até chegar na grande seleção vencedora da copa do mundo de 2022..  


* **[Repositório/Código fonte da Aplicação](https://github.com/luislauriano/Aplicacao_CopaDoMundo22-projeto)** 

* **[Aplicação na web](https://possiveis-resultados-qatar2022.herokuapp.com/)** 


<p align="center">
  <img src="https://i.imgur.com/o1YKs9I.png" width = 100%>
</p>

---

## Possíveis resultados finais a partir do modelo

Lembrar que, o resultado da partida é feito a partir da escolha do resultado mais provável, diante da probabilidade de cada resultado possível (vitória, empate e derrota) que foi calculado em uma função com base em todas as probabilidades de resultados possíveis. Por esse motivo, o resultado da partida pode acabar sendo diferente se testado outra vez. Para ficar mais claro, podemos imaginar a cena do doutor estranho no filme guerra infinita onde ele encontra um único resultado positivo para eles vencerem a guerra diante de todos os resultados possiveis finais que a guerra contra thanos poderia ter.

Outra observação, o resultado de gols de uma partida pode acabar se repetindo em muitos casos o placar de 1x0, talvez por o modelo não ter uma precisão para quantificar tão bem saldos maiores, mas o interessante é entender e levar em consideração quem o modelo está prevendo como possível vencedor da partida

### Teste 01
Essa é a principal aposta de resultado final do projeto para os jogos da fase mata-mata da copa do mundo de 2022, seguindo os resultados possíveis que o modelo informou, utilizando dados de partidas internacionais da fifa de 2010 a 2022, na tentativa de encontrar um melhor desempenho para o modelo.
<p align="center">
  <img src="https://i.imgur.com/WxpogGU.png" width = 100%>
</p>







