# 📊 Análise de Carteira de Crédito — Power BI

Dashboard interativo para acompanhar a saúde de uma carteira de crédito: volume emprestado, perfil de risco, inadimplência e distribuição por região e tipo de produto.

Este projeto é a evolução do [Projeto_Victor](LINK_DO_REPO_OU_PASTA_ANTIGA) — a primeira versão foi feita em Excel (tabelas dinâmicas), e esta é a versão em Power BI, com modelagem de dados e visualização interativa.

## 🎯 Pergunta de negócio

Como está o desempenho da carteira de crédito hoje: qual o volume total, quem são os clientes, e onde estão concentrados os maiores riscos e a maior inadimplência?

## 🖼️ Preview

<img width="1093" height="607" alt="power bl" src="https://github.com/user-attachments/assets/236f8273-98a9-4c35-9f83-d0a825dd380b" />


`![Dashboard](caminho/para/a/imagem.png)`

## 📌 O que o dashboard responde

- Qual o valor total emprestado e quantos clientes ativos na carteira
- Qual tipo de crédito (pessoal, cartão, veículo, consignado, imobiliário) mais representa o volume emprestado
- Como o valor emprestado se distribui por região
- Como a carteira evoluiu mês a mês ao longo do tempo
- Qual a exposição por nível de risco (alto, médio, baixo)
- Quantos clientes estão em dia, em atraso (30/60 dias) ou inadimplentes

## 🗂️ Dados e modelagem

- Fonte: base própria simulando uma carteira de crédito (250 clientes, ~23 milhões em valor emprestado)
- Colunas principais: `ID CLIENTE`, `VALOR EMPRESTADO`, `TIPO DE CRÉDITO`, `REGIÃO`, `RISCO`, `STATUS`, `DATA CONTRATO`
- Tratamento feito no Power Query: PREENCHER_COM_O_QUE_VOCÊ_FEZ (ex: correção de tipos de dado, remoção de duplicados, padronização de texto)

> **Próximo passo de modelagem:** os dados hoje estão em uma única tabela. Uma evolução planejada é separar em modelo estrela (tabela fato de contratos + dimensões de cliente, produto e uma tabela calendário), o que deixa o modelo mais rápido e mais alinhado ao que se espera em ambiente profissional.

## 📐 Métricas do dashboard

- Valor Emprestado (total)
- Quantidade de Clientes
- Valor Emprestado por Tipo de Crédito
- Valor Emprestado por Região
- Valor Emprestado por Ano e Mês
- Valor Emprestado por Risco
- Clientes por Status de Pagamento (Em Dia, Atraso 30d, Atraso 60d, Inadimplente)

## 🛠️ Ferramentas usadas

- Power BI Desktop (Power Query, modelagem, DAX, visualização)
- Excel (base de dados original)




