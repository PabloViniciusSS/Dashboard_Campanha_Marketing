
# Dashboard Análise de Campanha de Marketing

 ##  📊 Projeto de Análise de Dados: 
 
### 1. **Compreensão do Negócio (Business Understanding)** 📈

A ideia desse mini projeto, criado a partir do curso de Microsoft Power BI Para Business Intelligence e Data Science da Data Science Academy, é proporcionar uma visão geral sobre as campanhas de marketing de uma empresa. O objetivo é criar dashboards que permitam analisar dados e desenvolver estratégias e campanhas mais eficazes. Para isso, serão analisados quatro campos importantes para o sucesso de uma campanha:
    -  Visão do Cliente
    -  Visão do Comportamento de Compra do Cliente
    -  Visão de Performance das Campanhas de Marketing
    -  Visão dos Padrões de Compra no Ponto de Venda (País)


### 2. **Compreensão dos Dados (Data Understanding) 🧐**

Carregamento dos Dados: Os dados foram carregados no Power BI a partir de um arquivo CSV presente na pasta dataset. Ao carregar os dados, podemos ver as seguintes tabelas:

![geral](https://github.com/user-attachments/assets/7c4bd755-51d1-46c8-882b-75ea6dd4df26)

Para facilitar a análise eu dividir as tabelas em alguns grupos:

**Dados Pessoais do Cliente e Estrutura Familiar**

Dados diretamente relacionados aos clientes, como o identificador (ID), ano de nascimento, estado civil, salário anual, filhos em casa e adolescentes em casa.

![clientes](https://github.com/user-attachments/assets/fae31421-2fab-4483-8685-121be6162e7d)

O ID é único para cada pessoa, sendo o identificador na tabela. As tabelas "Filhos em Casa" e "Adolescentes em Casa" indicam quantos filhos vivem na casa, não se a pessoa tem filhos ou adolescentes. Isso muda a forma de análise.
Essas informações ajudam a segmentar os clientes em grupos, para entender melhor o perfil e suas necessidades.

**Dados de Cadastro e Atividade de Compras**

Dados relacionados à data de cadastro e quantos dias se passaram desde a última compra.

![cadastro_site](https://github.com/user-attachments/assets/4fb5157c-c20a-408e-b17b-e7200d6f8a83)

Ajuda a identificar clientes ativos e inativos, criando estratégias de reativação para os clientes que não compraram há muito tempo.

**Gastos por Categorias de Produtos**

Gastos por produtos esta divididos em 6 tipos: Eletrônicos, Brinquedos, Móveis, Utilidades, Alimentos, Vestuários.

![Gastos](https://github.com/user-attachments/assets/1d715794-8b57-4913-bf34-e3ddbf74858f)

Com esses dados podemos analisar quais categorias de produtos tem maior e menor gastos pelos clientes, por exemplo, se os gastos em Eletrônicos são significativamente maiores do que em Brinquedos, isso pode indicar uma preferência ou necessidade maior por esses itens. Além disso, podemos identificar padrões de compras para entender melhor as  preferências e ajustes de marketing e estoque.

**Informações de Compras com Desconto e Canais de Venda**

Os dados sobre compras com desconto, local da compra (Web, Catálogo ou Loja) e número de visitantes do mês.

![numeros_compras](https://github.com/user-attachments/assets/cf9c981a-9da9-4264-b816-6ae25ba62c32)

Compras com Desconto podemos verificar a eficácia das promoções e descontos, analisando quantas compras foram feitas, ajudando nas estratégias de preço e promoções.
Com esses dados podemos fazer uma análise de onde os clientes estão realizando suas compras, para ver preferências e otimizar as experiências de compras em cada canal.
O número de visitantes ajudar a avaliar o tráfego de interesses dos clientes.

**Companhas no site**

Nessas tabelas temos se o cliente fez compra na campanha 1, 2, 3, 4 ou 5 e se ele já comprou com a loja.

![compras](https://github.com/user-attachments/assets/7a0edd4f-fadf-497f-b775-97bdd2eaf1a2)

Compreender o sucesso das campanhas e criar estratégias baseadas nas que deram certo.

**País de Origem**
Por fim temos o país de origem.

![pais](https://github.com/user-attachments/assets/cee201cb-e01f-49bc-b038-d5c131339ec1)


Com essa informação podemos entender aonde os clientes estão localizados e adaptar as estratégias de marketing e logística para cada um deles.

### 3. **Preparação dos Dados (Data Preparation) 🛠️**

**Limpeza e Transformação:**

Os dados já vieram organizados. A única limpeza necessária foi a remoção de um valor discrepante que causava divergência em uma das tabelas.
Em relação à transformação, algumas colunas continham valores booleanos. Estas colunas foram transformadas para melhorar a compreensão dos dados:

    -   Compra na Campanha 1
    -   Compra na Campanha 2
    -   Compra na Campanha 3
    -   Compra na Campanha 4
    -   Compra na Campanha 5
    -   Comprou

Os valores 0 e 1 foram transformados para "não" e "sim", respectivamente, facilitando a análise e interpretação dos dados.

### 4. **Resultados Finais e Insights 💡**

**Visão do Cliente**

**Cards:**
**Salário Anual Médio:** Entender o poder aquisitivo do público-alvo.
**Total de Compras com Desconto:** Verificar a eficácia das campanhas de marketing.
**Quantidade de Clientes:** Quantificar o total de clientes registrados no site.

**Tabelas de Colunas:**
**Total de Clientes por Escolaridade:** Segmentar o público por nível de escolaridade.
**Total de Clientes por Estado Civil:** Segmentar o público por estado civil.

**Treemap:**
**Total de Compras:** Entender qual plataforma é mais usada para compras, ajudando a criar estratégias de marketing.

**Filtro de Países:**
**Filtro:** Segmentar os clientes por país para uma análise mais dinâmica e menos poluída.

![visao_cliente](https://github.com/user-attachments/assets/086652c4-566a-43f1-bc1e-c48a9bed0d8c)

Objetivo: Entender como são os clientes, criando campanhas e estratégias que impactem diretamente o público-alvo.

**Visão Comportamental**

**Gráfico de Dispersão:**
**Total de Gastos por Salário Anual:** Verificar a correlação entre gastos dos clientes e nível de renda.

**Gráficos de Colunas:**
**Total de Gastos por Adolescentes em Casa:** Verificar se a presença de adolescentes aumenta a necessidade de gastos.
**Total de Gastos por Filhos em Casa:** Verificar se a quantidade de filhos interfere no aumento dos gastos.

**Árvore Hierárquica:**
**Total de Gastos, Estado Civil, Escolaridade:** Analisar segmentos específicos e identificar padrões dentro de diferentes grupos.

![visao_comportamental](https://github.com/user-attachments/assets/c66bea74-d9e5-4533-a2c0-7bf80bb6266f)

Objetivo: Compreender como  é o comportamento de compra dos clientes, identificando tendências e padrões, para futuras decisões estratégicas, campanhas e otimizar a experiência do cliente.

**Visão de Campanha**

**Gráfico de Pizza:**
**Clientes que Compraram:** Verificar a proporção de clientes cadastrados que já fizeram compras.
**Total de Salário Anual dos Clientes que Compraram:** Verificar a correlação entre clientes que compraram e seu poder aquisitivo.

**Gráfico de Colunas:**
Total de Filhos em Casa dos Clientes que Compraram: Verificar a correlação entre a quantidade de filhos e as compras realizadas.

**Tabela Dinâmica:**
**Comprou, Estado Civil, País, Formação:** Análise demográfica detalhada dos clientes.

![visao_campanha](https://github.com/user-attachments/assets/91a9a4b5-60a2-4dc9-8a37-bbfb132f029c)

**Objetivo:** Avaliar a eficácia das campanhas, identificar os grupos demográficos e entender as características dos clientes que realizam compras ou não realizam as compras, para melhorar as estratégias de marketing e aumentar as vendas.

**Visão do Ponto de Vendas**

**Gráfico de Colunas Agrupadas com Linha:**
**Total Gasto por Categoria de Produto e Total de Clientes por País:** Analisar os gastos em cada categoria de produto em relação ao número de clientes, segmentação por país.

**Gráfico de Linhas:**
**Total de Gastos por Ano e País:** Verificar as tendências de vendas ao longo dos anos em diferentes regiões geográficas, ajudando a identificar tendências sazonais e regionais.

![visao_vendas](https://github.com/user-attachments/assets/d0007b3b-045e-479f-8f15-b858f6c36551)

**Objetivo:** Avaliar a performance de vendas em diferentes categorias de produtos e regiões ao longo do tempo, identificar sazonalidades e desenvolver estratégias de marketing e estoques eficazes 

### 5. 📎 Conclusão

Com este projeto de análise de dados oferece uma visão abrangente das campanhas de marketing, facilitando a criação de estratégias mais eficazes.É possível através dos Dashboards obter insights valiosos sobre perfil do cliente, comportamento de compras, eficácias das campanhas de marketing, desempenho dos pontos de vendas, verificar como cada região do planeta está reagindo as estratégias realizadas. Essas informações são cruciais para a tomada de decisões estratégicas, otimizando o impacto das campanhas de marketing e melhorando a experiência do cliente.


## Autores

- [@PabloVinicius](https://www.github.com/PabloViniciusSS)

Meu nome é Pablo Vinícius, venho estudando analise de dados, Ciencia de Dados , Aprendizado de Máquinas e deep learning, para buscar meu objetivo que é entrar na área de dados.
## Stack utilizada

**Análise de Dados:** Power BI

## Licença

[MIT](https://choosealicense.com/licenses/mit/)


## Etiquetas

Adicione etiquetas de algum lugar, como: [shields.io](https://shields.io/)

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)

 
