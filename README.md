# Sistema de Inspeção Visual Automática de Grãos de Café

Projeto de visão computacional para classificação binária de grãos de café em duas classes: **OK** e **defeituoso**.

## Objetivo

Desenvolver um pipeline clássico de visão computacional para segmentar grãos de café, extrair features manuais e treinar classificadores clássicos para identificar grãos fora do padrão.

## Estrutura do projeto

```text
dataset_binario/
  ok/
  defeituoso/

notebooks/
  01_segmentacao.ipynb
  02_features.ipynb
  03_classificacao.ipynb

outputs/
  X.csv
  y.csv
  graficos_features/
  matrizes_confusao/
  metricas/
  erros/
```

## Pipeline

O projeto segue o seguinte fluxo:

```text
Imagem RGB -> Segmentação -> Extração de features -> Classificação -> Avaliação
```

## Features extraídas

Foram utilizadas features manuais de:

* forma;
* cor;
* textura;
* momentos de Hu.

## Modelos avaliados

Foram comparados dois classificadores clássicos:

* Random Forest;
* SVM.

O melhor resultado foi obtido com o **SVM**, que apresentou **96,67% de acurácia** e apenas **1 erro** no conjunto de teste.

## Como executar

Instale as dependências:

```bash
pip install -r requirements.txt
```

Execute os notebooks na ordem:

```text
notebooks/01_segmentacao.ipynb
notebooks/02_features.ipynb
notebooks/03_classificacao.ipynb
```

## Resultados

Os resultados gerados pelo projeto estão salvos na pasta `outputs/`, incluindo tabelas de métricas, matrizes de confusão, gráficos de features e imagens classificadas incorretamente.
