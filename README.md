# Projeto - Fundamentos da Descoberta de Dados

Projeto do Módulo 13 com análise estatística e visualização de uma base de produtos de supermercado do Chile.

## Arquivos

- `Profissao_Cientista_de_Dados_M13_Projeto_RESOLVIDO.ipynb` - notebook com todas as respostas.
- `dados_parte_01.csv` a `dados_parte_10.csv` - base utilizada, dividida em partes apenas para publicação. O notebook reúne as partes automaticamente.
- `mapa_interativo_descontos.html` - visualização interativa em treemap.

## Principais resultados

### Preço normal por categoria

| Categoria                  |   Media |   Mediana |   Desvio_Padrao |   Quantidade |   Diferenca_Media_Mediana |
|:---------------------------|--------:|----------:|----------------:|-------------:|--------------------------:|
| lacteos                    | 2385.22 |       989 |         3925.82 |          447 |                   1396.22 |
| belleza-y-cuidado-personal | 1783.56 |      1569 |         2210.04 |          239 |                    214.56 |
| congelados                 | 2108.04 |      1519 |         2111.54 |          235 |                    589.04 |
| comidas-preparadas         | 3095.04 |      3290 |         2019.91 |           46 |                   -194.96 |
| frutas                     | 1724.47 |      1195 |         1639.15 |           19 |                    529.47 |
| instantaneos-y-sopas       |  765.49 |       439 |         1170.23 |           57 |                    326.49 |
| verduras                   | 1343.3  |      1180 |         1012.7  |           64 |                    163.3  |

A categoria com maior desvio padrão é **lacteos**, com desvio de **3925.82**.

Na categoria `lacteos`, a média é **2385.22** e a mediana é **989.00**, mostrando uma distribuição assimétrica e influenciada por valores altos.

O boxplot identifica **43 outliers** pelo critério de 1,5 × IQR.

### Média de desconto

| Categoria                  |   Media_Desconto |
|:---------------------------|-----------------:|
| congelados                 |           154.03 |
| belleza-y-cuidado-personal |           123.08 |
| comidas-preparadas         |            43.48 |
| lacteos                    |            17.41 |
| frutas                     |             0    |
| instantaneos-y-sopas       |             0    |
| verduras                   |             0    |

## Como executar

```bash
pip install pandas matplotlib plotly
```

Abra o notebook em Jupyter Notebook, JupyterLab ou VS Code e execute as células em ordem.

## Publicação

Para disponibilizar o projeto no GitHub:

1. Crie um repositório.
2. O notebook lê automaticamente todos os arquivos `dados_parte_*.csv`.
3. Use este `README.md` como página inicial do repositório.
4. Para publicar a visualização interativa, habilite o GitHub Pages apontando para a branch `main`.
