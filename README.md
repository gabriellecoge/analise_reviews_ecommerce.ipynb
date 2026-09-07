# Análise de Avaliações — E-commerce de Moda Feminina

Análise exploratória de 23.486 avaliações de clientes de um e-commerce de roupas femininas, com foco em entender o que separa uma cliente que recomenda o produto de uma que não recomenda — e o que isso indica sobre categorias, faixa etária e qualidade percebida.  

# Sobre os dados

Dataset público de avaliações reais de um varejista de moda feminina (anonimizado — nomes de marca e produto foram removidos pela fonte).

| | |
|---|---|
| Linhas | 23.486 avaliações |
| Produtos distintos | 1.206 |
| Colunas | 10 |
| Período | não informado na fonte |


| Coluna | Descrição |
|---|---|
| `Clothing ID` | Identificador do produto avaliado |
| `Age` | Idade da autora da avaliação (18 a 99 anos) |
| `Title` | Título da avaliação |
| `Review Text` | Texto livre da avaliação |
| `Rating` | Nota de 1 a 5 dada pela cliente |
| `Recommended IND` | 1 = recomenda o produto, 0 = não recomenda |
| `Positive Feedback Count` | Quantas pessoas acharam a avaliação útil |
| `Division Name` | Divisão do catálogo (General, General Petite, Initmates) |
| `Department Name` | Departamento (Tops, Dresses, Bottoms, Intimate, Jackets, Trend) |
| `Class Name` | Classe do produto (20 categorias: Dresses, Knits, Blouses…) |

### Panorama inicial

As notas são fortemente enviesadas para cima:
| Nota | Avaliações | % |
|---|---|---|
| 5 ★ | 13.131 | 55,9% |
| 4 ★ | 5.077 | 21,6% |
| 3 ★ | 2.871 | 12,2% |
| 2 ★ | 1.565 | 6,7% |
| 1 ★ | 842 | 3,6% |
82,2% das clientes recomendam o produto avaliado. Idade média de 43,2 anos

### Nota média por departamento:

| Departamento | Nota média | Avaliações |
|---|---|---|
| Bottoms | 4,29 | 3.799 |
| Intimate | 4,28 | 1.735 |
| Jackets | 4,26 | 1.032 |
| Tops | 4,17 | 10.468 |
| Dresses | 4,15 | 6.319 |
| Trend | 3,82 | 119 |

Tops e Dresses concentram 71% do volume de avaliações; Trend é a única categoria com nota média abaixo de 4,0 — e a de menor volume.

### Ferramentas

Python · pandas · numpy · matplotlib · seaborn · Google Colab

### Fonte dos dados

Women's E-Commerce Clothing Reviews — dataset público disponível no Kaggle, publicado por Nicapotato sob licença CC0 (domínio público). Os dados são reais e foram anonimizados pela fonte.
