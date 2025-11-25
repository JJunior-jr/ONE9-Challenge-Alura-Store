# ONE9-Challenge-Alura-Store

# Análise de Desempenho de Lojas

Este notebook contém uma análise detalhada do desempenho de quatro lojas diferentes, utilizando dados de vendas, faturamento, avaliação de clientes e informações geográficas. O objetivo é extrair insights sobre o comportamento de vendas e identificar pontos fortes e fracos de cada loja.

## Sumário do Conteúdo:

### 1. Análise de Faturamento

Nesta seção, calculamos o faturamento total de cada uma das quatro lojas. Os resultados mostraram:
- Loja 1: R$ 1,534,509.12
- Loja 2: R$ 1,488,459.06
- Loja 3: R$ 1,464,025.03
- Loja 4: R$ 1,384,497.58

### 2. Vendas por Categoria
Foi realizada uma análise da quantidade de produtos vendidos por categoria em cada loja, bem como a participação percentual de cada categoria no total de vendas. Gráficos de barras foram utilizados para visualizar a quantidade de vendas por categoria e a participação percentual, mostrando as categorias mais e menos representativas para cada loja.

### 3. Média de Avaliação das Lojas
Calculamos a média das avaliações de compra para cada loja e a média geral. Os resultados foram:
- Loja 1: 3.98
- Loja 2: 4.04
- Loja 3: 4.05
- Loja 4: 4.00
Um gráfico de barras visualiza essas médias, com uma linha indicando a média geral.

### 4. Produtos Mais e Menos Vendidos
Identificamos os 5 produtos mais vendidos e os 5 menos vendidos para cada loja. Gráficos de barras separados foram gerados para visualizar esses rankings, oferecendo uma visão clara dos itens de maior e menor demanda.

#### Exemplo Top 5 (Loja 4):
| Produto                  | Vendas |
|:-------------------------|-------:|
| Cama box                 |     62 |
| Faqueiro                 |     59 |\n| Dashboards com Power BI  |     56 |
| Cama king                |     56 |
| Carrinho controle remoto |     55 |

#### Exemplo Bottom 5 (Loja 4):
| Produto                     | Vendas |
|:----------------------------|-------:|
| Geladeira                   |     38 |
| Ciência de dados com python |     38 |
| Violão                      |     37 |
| Guarda roupas               |     34 |
| Guitarra                    |     33 |

### 5. Frete Médio por Loja
Analisamos o valor médio do frete para cada loja, bem como a média geral do frete. Os valores encontrados foram:
- Loja 1: R$ 34.69
- Loja 2: R$ 33.62
- Loja 3: R$ 33.07
- Loja 4: R$ 31.28
Um gráfico de barras apresenta esses valores, com uma linha indicando o frete médio geral.

### 6. Análise de Desempenho Geográfico
Utilizando a biblioteca `folium`, foi gerado um mapa interativo para visualizar a localização das compras de cada loja. Cada compra é representada por um círculo colorido, onde a cor indica a loja de origem. Isso permite uma análise visual da distribuição geográfica das vendas.
"""

# Adding image links to the README content

# Section 2. Vendas por Categoria

    "## 2. Vendas por Categoria\n",
    "## 2. Vendas por Categoria\n\n" +
    "![Vendas por Categoria e Loja](vendas_por_categoria_e_loja.png)\n\n" 


# Section 3. Média de Avaliação das Lojas
readme_content = readme_content.replace(
    "Um gráfico de barras visualiza essas médias, com uma linha indicando a média geral.\n",
    "Um gráfico de barras visualiza essas médias, com uma linha indicando a média geral.\n\n" +
    "![Média de Avaliações por Loja](media_avaliacoes_por_loja.png)\n\n"
)

# Section 4. Produtos Mais e Menos Vendidos
readme_content = readme_content.replace(
    "#### Exemplo Top 5 (Loja 4):\n",
    "![Top 5 Produtos Mais Vendidos - Loja 1](top5_mais_vendidos_Loja1.png)\n\n" +
    "![Top 5 Produtos Mais Vendidos - Loja 2](top5_mais_vendidos_Loja2.png)\n\n" +
    "![Top 5 Produtos Mais Vendidos - Loja 3](top5_mais_vendidos_Loja3.png)\n\n" +
    "![Top 5 Produtos Mais Vendidos - Loja 4](top5_mais_vendidos_Loja4.png)\n\n" +
    "#### Exemplo Top 5 (Loja 4):\n"
)

readme_content = readme_content.replace(
    "#### Exemplo Bottom 5 (Loja 4):\n",
    "![Top 5 Produtos Menos Vendidos - Loja 1](top5_menos_vendidos_Loja1.png)\n\n" +
    "![Top 5 Produtos Menos Vendidos - Loja 2](top5_menos_vendidos_Loja2.png)\n\n" +
    "![Top 5 Produtos Menos Vendidos - Loja 3](top5_menos_vendidos_Loja3.png)\n\n" +
    "![Top 5 Produtos Menos Vendidos - Loja 4](top5_menos_vendidos_Loja4.png)\n\n" +
    "#### Exemplo Bottom 5 (Loja 4):\n"
)

# Section 5. Frete Médio por Loja
readme_content = readme_content.replace(
    "Um gráfico de barras apresenta esses valores, com uma linha indicando o frete médio geral.\n",
    "Um gráfico de barras apresenta esses valores, com uma linha indicando o frete médio geral.\n\n" +
    "![Frete Médio por Loja](frete_medio_por_loja.png)\n\n"
)

# Section 6. Análise de Desempenho Geográfico
readme_content = readme_content.replace(
    "Isso permite uma análise visual da distribuição geográfica das vendas.\n",
    "Isso permite uma análise visual da distribuição geográfica das vendas.\n\n" +
    "![Mapa Geográfico](mapa_geografico.png)\n\n"
)

with open('README.md', 'w') as f:
    f.write(readme_content)

print("README.md updated with image links.")

# Display the updated README.md content
!cat README.md
