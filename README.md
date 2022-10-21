# analise-descritiva-risco_credito

Projeto de análise descritiva de risco de crédito. Este projeto faz parte da lista de exercícios da trilha de Big Data Science oferecido pela SEMANTIX.


![Badge ongoing](http://img.shields.io/static/v1?label=STATUS&message=ONGOING&color=YELLOW&style=for-the-badge)

## O problema proposto é dado por:

``Um grande banco tem o objetivo de desenvolver um modelo para identificar maior probabilidade de default. Sua tarefa será realizar uma análise descritiva e tratamento dos dados para entender o perfil dos clientes e quais fatores podem influenciar no risco de crédito.``

## A base de dados

 A base de dados contou com um total de 10 variáveis (features), sendo elas dadas por:

 - ``default``
 	* Essa variável indica se o cliente é (True) um bom pagador ou não (False)
 - ``t_risco``
 	* Essa é taxa de risco do emprestimo, valor que varia de 0 a 1	
 - ``valor_emprestimo``
 	* indica o valor do emprestimo
 - ``prazo_pagamento``	
 	* prazo para o pagamento do emprestimo, dado em meses
 - ``limite_credito``	
 - ``renda``	
 - ``signo``	
 - ``genero``	
 	* se o cliente é homem (m) ou mulher (f)
 - ``perfil_facebook``	
 	* se o cliente possui perfil no facebook (True) ou não (False)
 - ``n_emprestimos_inadiplentes``
 	* número de emprestimos inadiplentes, isto é, quando há o descumprimento do pagamento.

## Resultados da Análise:

A base de dados consta com 64592 linhas e com 10 colunas, deletando a coluna ``signos`` e a partir destes números, há a seguinte contagem de valores nulos referente a cada feature:

- default:                        4626
- t_risco:                         785
- valor_emprestimo:                785
- prazo_pagamento:                 785
- limite_credito:                19753
- renda:                           785
- genero:                         7186
- perfil_facebook:                6407
- n_emprestimos_inadiplentes:      803

Essa contagem pode ser melhor observada no gráfico de barras abaixo:

<br>
<p align="center">
  <img src="https://github.com/ramosrafaela/analise-descritiva-risco_credito/blob/main/figures/contagem.png" width="600" />
</p>


A análise consistiu em calcular os valores estatísticos relacionados a cada feature e preeencher os dados nulos pela média ou mediana. Para features que possuiam maior dispersão foi escolhido usar a mediana. Para features categóricas foi utilizado a moda. 

Uma análise descritiva bivariada foi feita de forma a observar se caracteristicas como genero e perfil no facebook influênciavam no risco de crédito. Os gráficos abaixo demonstram que esses dois fatores não influenciam se o cliente irá ou não pagar o emprestimo.


<br>
<p align="center">
  <img src="https://github.com/ramosrafaela/analise-descritiva-risco_credito/blob/main/figures/hist_f_m_genero.png" width="600" />
</p>

A análise também permitiu observar que não há nenhuma correlação forte entre as features, de forma que numa modelagem para realizar previsões essas features poderiam ser utilizadas.

<br>
<p align="center">
  <img src="https://github.com/ramosrafaela/analise-descritiva-risco_credito/blob/main/figures/correlacao.png" width="600" />
</p>

Também foi possível observar, utilizando o paiplot, se há alguma relação entre as variáveis, isto é, se de alguma forma teria alguma tendencia entre os comportamentos das features do problema. O que se conclui é há apenas comportamentos aleatórios, não há a presença de nenhum padrão significativo. 

<br>
<p align="center">
  <img src="https://github.com/ramosrafaela/analise-descritiva-risco_credito/blob/main/figures/correlacao_graficos.png" width="600" />
</p>
