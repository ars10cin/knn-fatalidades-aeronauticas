# Predição de fatalidades em acidentes aeronáuticos com kNN

Projeto de CIN0208 – Ciência de Dados 2026.2 (CIN-UFPE)
Autores: Artur Regis, Mateus Costa, Lucas Miranda e Tiago Sales.

## O que é
Avalia o kNN (hiperparâmetros padrão) na predição de fatalidades em 14.822 aeronaves do CENIPA, variando o pré-processamento em 384 configurações (360 distintas) com validação cruzada estratificada de 10 folds, sem vazamento de dados.

## Arquivos
- colab ciencia de dados atualizado.ipynb: código completo e saídas
- aeronave.csv: base do CENIPA (dados abertos)
- tabela_experimentos_completa.csv: 360 configurações distintas da grade
- resultados_experimentos_knn.csv: resultados da grade (384 configurações)
- testes_estatisticos.csv: comparações entre técnicas de balanceamento
- ablacao_fase_operacao.csv: modelo sem a fase da operação
- vazamento_nivel_dano.csv: efeito da variável nível de dano
- modelos_referencia.csv: comparação com sorteio e regressão logística
- teste_pca.csv: teste complementar com PCA
- entregaveis_projeto.zip: figuras geradas pelo notebook (também aparecem nas saídas do notebook)

## Como reproduzir
1. Abrir o notebook "colab ciencia de dados atualizado.ipynb" no Google Colab.
2. Enviar o arquivo aeronave.csv para o ambiente do Colab (painel de arquivos).
3. Executar tudo (Ambiente de execução > Executar tudo). A grade de 3.840 ajustes leva alguns minutos.
4. Os arquivos CSV e as figuras são gerados no próprio ambiente do Colab.

## Ambiente
Python 3.13, scikit-learn 1.6.1, imbalanced-learn 0.14.2, pandas 2.2.3, numpy 2.4.6 (Google Colab).

## Fonte dos dados
CENIPA, Portal de Dados Abertos:
https://dados.gov.br/dados/conjuntos-dados/ocorrencias-aeronauticas-da-aviacao-civil-brasileira
