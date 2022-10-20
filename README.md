# analise-descritiva-risco_credito

Projeto de análise descritiva de risco de crédito. Este projeto faz parte da lista de exercícios da trilha de Big Data Science oferecido pela SEMANTIX.

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


