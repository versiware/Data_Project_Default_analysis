# Análise Descritiva de Clientes com Cartão de Crédito

Este projeto tem como objetivo identificar padrões e subgrupos de clientes altamente endividados a partir de dados de cartão de crédito, utilizando a técnica de **Subgroup Discovery**, utilizando o Beam Search.
Desenvolvido por VersiWare – Projeto de aprendizado em análise de dados com foco em segmentação de clientes e inteligência de negócios.

---

## Objetivo

Realizar uma análise exploratória e descritiva para identificar **comportamentos comuns entre os clientes mais endividados**, com base em características como:

- Limite de crédito
- Pagamento mínimo
- Frequência de uso
- Saques em dinheiro (cash advance)
- Tempo de relacionamento com o cartão

---

## Metodologia

Foi utilizada a biblioteca `pysubgroup` com o algoritmo **Beam Search** para encontrar subgrupos que apresentem a **maior média de saldo devedor (BALANCE)**. Os subgrupos são definidos por combinações de regras sobre os atributos do cliente.

A métrica usada foi a **diferença da média do subgrupo para a média global** (`mean_sg - mean_dataset`), priorizando subgrupos com comportamento acima da média.

---

## Principais Insights

- **Pagamentos Mínimos Elevados**: A variável `MINIMUM_PAYMENTS >= 994.39` aparece em quase todos os subgrupos com saldo alto.
- **Limite de Crédito Alto**: Clientes com `CREDIT_LIMIT >= 7000` concentram parte significativa das dívidas.
- **Uso Rotativo do Cartão**: A baixa taxa de pagamento total da fatura (`PRC_FULL_PAYMENT < 8%`) indica clientes que carregam dívidas mês a mês.
- **Clientes Antigos e Ativos**: Aqueles com `TENURE >= 12` e `BALANCE_FREQUENCY >= 1.0` apresentam comportamento de endividamento contínuo.
- **Uso de Cash Advance**: Clientes que realizam saques em dinheiro (`CASH_ADVANCE >= 1576.49`) são os que possuem **maior média de saldo devedor (R$ 6.715,71)**.
