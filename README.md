# Análise preditiva do preço de venda de imóveis em São Paulo
&nbsp;
> Análise Exploratório de Dados e modelo prreditivo de regressão para estimativa de preços de venda de apartamentos na cidade de São Paulo capital - SP, Brasil.

&nbsp;

O preço de compra de um imóvel pode variar conforme muitos fatores: sua localização, . Por isso, buscar por um imóvel que corresponde às necessidade e objetivos do usuário não é uma tarefa trivial. 

Nesse projeto, aprendizagem de máquina foi utilizada para obter um modelo preditivo baseado em dados obtidos por web scrapping de classificados online. Foram treinados modelos de regressão linear aplicando os métodos de regularização Lasso (L1), Ridge (L2), e também modelo sem regularização. Foi feita a tranformação Box-Cox da variável dependente para a normalização da distribuíção dos resíduos. Para o ajuste de himeparâmetros foi aplicada a otimização de hiperparâmetros pelo algoritmo de Descida do Gradiente.

&nbsp;

### **Objetivos principais:**
---
- Obter um modelo preditivo para preços de compra de apartamento na cidade de São Paulo.
- Obter insights explorando as relações entre as variáveis explicativas e a variável resposta.

&nbsp;

### **Descrição do conjunto de dados**
---
O conjunto de dados possui informações de mais de 13000 apartamentos disponíveis para venda ou aluguel na cidade de São Paulo, Brasil. Os dados foram coletados durante abril de 2019 por meio de webscraping de sites de classificados imobiliários.

**Fonte:** Kaggle

**Disponível em:** https://www.kaggle.com/datasets/argonalyst/sao-paulo-real-estate-sale-rent-april-2019?resource=download

&nbsp;

### **Dependências**
---
```sh
import pandas as pd
import numpy as np
import sklearn 
import scipy
import matplotlib.pyplot as plt
import seaborn as sns
```

&nbsp;

### **Principais resultados obtidos em relação às métricas de performance dos modelos**
---
R² de cada um dos modelos de regressão linear em relação ao conjunto de teste:
Método de Regularização | Sem transformação da target | Com transformação Boxcox
:---|:---:|:---:
Nenhum           |          0.799037          |        0.850788
Ridge (L2)       |          0.877548          |        0.880910
Lasso (L1)       |          0.869770          |        0.883898





