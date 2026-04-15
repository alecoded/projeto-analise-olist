**Análise Exploratória de Vendas - E-commerce Olist (Pandas)**

Este projeto faz parte de um portfólio de análise de dados e foca na extração de insights e manipulação de grandes volumes de dados utilizando a biblioteca Pandas. O objetivo principal é consolidar diferentes fontes de dados para entender o desempenho financeiro e o comportamento de vendas da Olist.

**Objetivos da Análise**
Consolidar múltiplos datasets (pedidos, pagamentos, itens e produtos) em uma única base mestra para análise.

Calcular métricas financeiras chave, como o faturamento total bruto (R$ 16.008.872,12).

Analisar a distribuição da receita por status do pedido para identificar o volume de entregas concluídas.

Identificar tendências temporais de faturamento mensal para detectar períodos de pico e sazonalidade.

Mapear as categorias de produtos que mais contribuem para a receita da plataforma.

Mapear a eficiência logística calculando a distribuição do tempo total de entrega (em dias) desde a compra até a chegada ao cliente.

**Tecnologias e Bibliotecas**
Python 3.x

Pandas: Limpeza, transformação e agregação de dados.

Matplotlib & Seaborn: Criação de visualizações gráficas (gráficos de barras e linhas).

Zipfile: Extração automatizada do dataset.

**Etapas do Projeto**
Extração de Dados: Automatização da extração dos arquivos .csv a partir de um arquivo comprimido (archive.zip).

Limpeza e Consolidação: Junção (merge) das tabelas de pedidos e pagamentos utilizando o order_id como chave, seguida pela integração com itens e produtos para criar uma base rica em detalhes.

**Análise de Receita:**

Cálculo da receita total.

Agrupamento por status (ex: delivered, canceled, shipped) com visualização em gráfico de barras horizontais.

**Série Temporal:** Conversão de strings para formato datetime e criação de colunas de período (Ano-Mês) para plotar a evolução mensal das vendas.

**Análise de Produtos:** Ranking das categorias campeãs em faturamento, identificando setores como "cama_mesa_banho" e "beleza_saude" no topo da lista.

<img width="989" height="493" alt="image" src="https://github.com/user-attachments/assets/5b42c29c-d146-4ea5-9c5d-dbfc367ba3fd" />


**Principais Insights Obtidos**

**Agilidade Logística:** A distribuição do tempo de entrega mostra que a grande maioria dos pedidos é entregue entre 5 e 15 dias, com o pico de frequência (moda) concentrado na faixa de 7 a 8 dias. Isso demonstra uma operação de logística eficiente na maior parte dos casos, embora exista uma "cauda longa" de pedidos que demoram 30 dias ou mais.

<img width="851" height="495" alt="image" src="https://github.com/user-attachments/assets/1ddb32c0-1788-407f-a76e-65bff14fa721" />

*Figura 1: Histograma do Tempo de Entrega. A análise demonstra que a logística da plataforma é eficiente na maioria dos casos, com o maior volume de pedidos sendo entregue entre 5 e 12 dias. Porém, observa-se uma "cauda longa" que indica desafios com entregas mais demoradas (acima de 30 dias).*

**Dominância de Entregas:** A esmagadora maioria da receita provém de pedidos com status "entregue", garantindo a saúde operacional do faturamento.

**Pico Histórico:** Novembro de 2017 foi identificado como o mês de maior faturamento, com mais de R$ 1,58 milhão em vendas.

<img width="860" height="512" alt="image" src="https://github.com/user-attachments/assets/b5892b6d-00da-4740-84ce-78d99a137c09" />

*Figura X: Evolução do faturamento mensal. É possível observar um crescimento consistente ao longo de 2017, com um pico histórico expressivo em novembro (impacto provável da Black Friday). Após o pico, o e-commerce consolida suas vendas em um patamar superior ao longo de 2018.*

<img width="860" height="512" alt="image" src="https://github.com/user-attachments/assets/a19b8d40-aaea-4ddc-aeb9-334e42f647af" />


**Concentração de Receita**: O Top 5 de categorias de produtos representa uma fatia significativa do faturamento total, com destaque para artigos de uso doméstico e bem-estar.

**Nota:** Este notebook foca na abordagem programática e estatística com Pandas. Para uma análise focada em consultas estruturadas de banco de dados, consulte o arquivo 02-analise-avancada-sqlite.ipynb.
