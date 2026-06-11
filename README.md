# \# Sistema de Inspeção Visual Automática de Grãos de Café

# 

# Este projeto implementa um pipeline clássico de visão computacional para classificar grãos de café em duas classes: OK e defeituoso.

# 

# \## Estrutura

# 

# \- dataset\_binario/: imagens organizadas por classe

# \- notebooks/: notebooks do pipeline

# \- outputs/: resultados gerados

# \- outputs/X.csv: tabela de features

# \- outputs/y.csv: vetor de classes

# 

# \## Como executar

# 

# 1\. Instalar as dependências:

# 

# pip install -r requirements.txt

# 

# 2\. Executar os notebooks na ordem:

# 

# notebooks/01\_segmentacao.ipynb  

# notebooks/02\_features.ipynb  

# notebooks/03\_classificacao.ipynb

# 

# \## Modelos avaliados

# 

# Foram avaliados dois classificadores clássicos:

# 

# \- Random Forest

# \- SVM

# 

# O melhor modelo foi o SVM, com 96,67% de acurácia e 1 erro no conjunto de teste.

