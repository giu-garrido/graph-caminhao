# Caminhão

Este projeto resolve o problema de transporte de cargas pesadas entre ilhas conectadas por pontes, respeitando o limite de peso de cada ponte. Foi baseado em um problema da Maratona de Programação da SBC (beecrowd | 1476). **Este projeto é apenas para fins educacionais.**

## Descrição

A Sociedade de Balões Coloridos (SBC) precisa transportar balões entre depósitos e sedes regionais em um arquipélago.
As ilhas são ligadas por pontes com capacidade máxima de peso.

O sistema:

- Modela o arquipélago como um grafo ponderado.
- Calcula a Árvore Geradora Máxima (AGM) para maximizar a capacidade de carga.
- Encontra o maior peso bruto que pode ser transportado em cada trajeto depósito-sede.
- Plota visualmente os grafos e caminhos no Colab usando widgets interativos.

## Bibliotecas usadas

- Numpy 
- NetworkX
- MatplotLib
- ipywidgets

## Como funciona o algoritmo

- Lê o número de ilhas, pontes e sedes a partir do arquivo de entrada.
- Cria o grafo inicial com as ilhas e pontes.
- Gera a Árvore Geradora Máxima (AGM) para aproveitar as pontes mais fortes.
- Calcula o caminho entre depósito e sede com o maior peso possível (baseado no gargalo do caminho).
- Exibe o resultado de forma interativa e gráfica para o usuário.
