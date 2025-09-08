# Desafio de Engenharia de Analytics - Análise de Dados para o Banco Vitória (BanVic)

## Introdução
Este projeto é uma simulação de um desafio de Engenharia de Analytics e Análise de Dados, com o objetivo de demonstrar o valor que a cultura e o uso de dados podem trazer para uma instituição financeira. A análise tem como foco principal a performance de crédito e a otimização de processos, visando impulsionar a tomada de decisões estratégicas.

## Contexto do Desafio
O Banco Vitória (BanVic) busca amadurecer sua cultura de dados para impulsionar a excelência em seus serviços. O projeto piloto foi proposto para analisar dados de crédito e operações, com o intuito de gerar valor para áreas críticas do banco e convencer stakeholders, como a diretora comercial Camila Diniz, de que o uso de dados é fundamental para a tomada de decisão estratégica.

---

## Metodologia e Ferramentas
A análise foi conduzida em um Jupyter Notebook e seguiu as seguintes etapas:
* **Análise Exploratória de Dados (EDA):** Verificação de tipos de dados, valores nulos e a estrutura dos DataFrames.
* **Limpeza e Transformação:** Conversão da coluna de datas para o formato `datetime`, remoção de valores inconsistentes e criação de novas features como 'dia da semana' e 'mês par'.
* **Junção de Dados:** Combinação de múltiplas tabelas (`transacoes`, `contas` e `agencias`) para permitir análises mais robustas e a criação de rankings de desempenho.
* **Visualização e KPIs:** Construção de dashboards e gráficos para resumir as principais descobertas em KPIs claros e acionáveis.

**Ferramentas Utilizadas:**
* Python
* Pandas (manipulação e análise de dados)
* Matplotlib e Seaborn (visualização de dados)
* Jupyter Notebook / VS Code (ambiente de desenvolvimento)

---

## Análises e Resultados Detalhados
O projeto atendeu a todas as solicitações do desafio, gerando insights importantes para a tomada de decisão.

### 1. Análise de Sazonalidade das Transações
A análise temporal revelou padrões claros de comportamento dos clientes.
- **Padrão Semanal:** O volume médio de transações é significativamente maior nos **finais de semana**, com picos de atividade aos sábados e domingos.
- **Comparação Mensal:** A afirmação de que o volume médio de transações seria maior em meses pares foi **refutada**, pois não houve diferença significativa entre os volumes médios de transações em meses pares e ímpares.

### 2. Ranking de Agências e Performance
O ranking de desempenho de agências, crucial para a CEO Sofia, revelou uma grande variação na performance.
- **Agências de Destaque:** A **Agência Digital** se destacou como a líder absoluta, com um volume de transações muito superior à média. A **Agência Matriz** e a **Agência Tatuapé** também tiveram performances sólidas.
- **Agências de Menor Desempenho:** A **Agência Recife** e a **Agência Jardins** apresentaram os menores volumes de transações, indicando a necessidade de direcionar esforços de melhoria.

**Resultados Numéricos do Ranking:**
Ranking das 3 melhores agências:
nome  total_transacoes
1  Agência Digital             33167
4   Agência Matriz              8610
9  Agência Tatuapé              7156

Ranking das 3 piores agências:
nome  total_transacoes
2  Agência Florianópolis              2133
3        Agência Jardins              2109
7         Agência Recife               374


### 3. Proposta de Expansão e Dados Externos
Para enriquecer a análise, foram propostas fontes de dados públicas, como as do **Banco Central (BACEN)** e **IBGE**. A integração desses dados permitiria ao BanVic:
- **Analisar o Risco:** Correlacionar a taxa de juros (Selic) e a inflação (IPCA) com a inadimplência de crédito.
- **Segmentar Clientes:** Usar dados demográficos para entender melhor o perfil dos clientes em diferentes regiões e direcionar campanhas de marketing de forma mais eficaz.
- **Gestão de Tesouraria:** Correlacionar a taxa de câmbio (dólar) com o volume de transações internacionais para otimizar operações.

---

## Conclusão Geral
O projeto demonstrou que a visualização de dados pode gerar **insights imediatos e acionáveis**, como a identificação de picos de demanda e a avaliação de desempenho de unidades de negócio. A análise de dados não apenas respondeu às perguntas iniciais, mas também abriu a porta para o futuro da cultura de Business Intelligence no BanVic.

---

## Como Executar o Projeto
Para reproduzir a análise, siga as instruções abaixo:
1.  **Clone o Repositório:**
    `git clone https://github.com/Cor4l92/Desafio-BanVic.git`
2.  **Abra o Projeto no VS Code:**
    `code Desafio-BanVic`
3.  **Estrutura da Pasta:** Certifique-se de que a pasta `banvic_data/` está no mesmo diretório do notebook (`analise_banvic.ipynb`).
4.  **Execute o Notebook:** Abra o arquivo `analise_banvic.ipynb` no VS Code ou Jupyter 
