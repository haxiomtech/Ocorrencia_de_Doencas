
# Previsão de Cancer de Mama com Base em Histórico de Pacientes

### Parte dos primeiros dados e colunas

![image](https://user-images.githubusercontent.com/119424591/208986052-7fb85114-55aa-4476-a136-a6a95ae83aeb.png)

### Análise Exploratória

#### Quantidade de diagnósticos

![image](https://user-images.githubusercontent.com/119424591/208977261-53243480-f526-4c5c-b70f-3f4d03a86f25.png)

#### Separação entre dados de treino e dados de teste

1. Os dados de treino são parte dos dados brutos com intuito de treinar o algoritmo.
2. Os dados de teste são outra parte dos dados brutos, diferentes dos dados de treino, com intuito de validar o resultado da previsão.

Para treinar o algoritmo foram utilizados 469 registros. 
Para testar o algoritmo foram utilizados 100 registros.

### Resultado

![image](https://user-images.githubusercontent.com/119424591/208981537-82bd687c-0766-4e79-b416-5743dc996cd7.png)

### Interpretando os Resultados

 A tabela cruzada mostra 4 possíveis valores, que representam os falso/verdadeiro positivo e negativo
 
 Temos duas colunas listando os labels originais nos dados observados
 
 Temos duas linhas listando os labels dos dados de teste

### Temos:

 Cenário 1: Célula Benigno (Observado) x Benigno (Previsto) - 61 casos - true positive 
 
 Cenário 2: Célula Maligno (Observado) x Benigno (Previsto) - 00 casos - false positive (o modelo errou)
 
 Cenário 3: Célula Benigno (Observado) x Maligno (Previsto) - 02 casos - false negative (o modelo errou)
 
 Cenário 4: Célula Maligno (Observado) x Maligno (Previsto) - 37 casos - true negative 

### Lendo a Confusion Matrix (Perspectiva de ter ou não a doença):

 True Negative  = nosso modelo previu que a pessoa NÃO tinha a doença e os dados mostraram que realmente a pessoa NÃO tinha a doença
 
 False Positive = nosso modelo previu que a pessoa tinha a doença e os dados mostraram que NÃO, a pessoa tinha a doença
 
 False Negative = nosso modelo previu que a pessoa NÃO tinha a doença e os dados mostraram que SIM, a pessoa tinha a doença
 
 True Positive = nosso modelo previu que a pessoa tinha a doença e os dados mostraram que SIM, a pessoa tinha a doença

 Falso Positivo - Erro Tipo I
 
 Falso Negativo - Erro Tipo II

### Taxa de acerto do Modelo: 98% (acertou 98 em 100)




