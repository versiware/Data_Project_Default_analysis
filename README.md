# SD_MAP
O código SD MAP and Beam Search: Análise de inadimplência de clientes, tem como objetivo identificar perfis de clientes com um alto saldo devedor (balance) na base pública um conjunto de dados de cartão de crédito para agrupamento, onde o conjunto de dados resume o comportamento de uso de cerca de 9.000 titulares ativos de cartão de crédito nos últimos 6 meses. 
O nível do cliente possui 18 variáveis comportamentais.
Entendo os dados de Análise, de onde foram extraídos insights relevantes:
CUST_ID : Identificação do titular do cartão de crédito (categórico)
BALANCE : Valor do saldo restante na conta para fazer compras (
BALANCE_FREQUENCY : Com que frequência o saldo é atualizado, pontuação entre 0 e 1 (1 = atualizado com frequência, 0 = não atualizado com frequência)
PURCHASES : Quantidade de compras feitas da conta
ONEOFF_PURCHASES : Valor máximo de compra feita de uma só vez
INSTALLMENTS_PURCHASES : Quantidade de compra feita em parcelas
CASH_ADVANCE : Dinheiro adiantado dado pelo usuário
PURCHASES_FREQUENCY : Com que frequência as compras estão sendo feitas, pontuação entre 0 e 1 (1 = comprada com frequência, 0 = não comprada com frequência)
ONEOFFPURCHASESFREQUENCY : Com que frequência as compras estão acontecendo de uma só vez (1 = comprada com frequência, 0 = não comprada com frequência)
PURCHASESINSTALLMENTSFREQUENCY : Com que frequência as compras em parcelas estão sendo feitas (1 = feita com frequência, 0 = não feito com frequência)
CASHADVANCEFREQUENCY : Frequência do pagamento adiantado em dinheiro
CASHADVANCETRX : Número de transações feitas com "Dinheiro adiantado"
PURCHASES_TRX : Número de transações de compra feitas
CREDIT_LIMIT : Limite do cartão de crédito para o usuário
PAYMENTS : Valor do pagamento feito pelo usuário
MINIMUM_PAYMENTS : Valor mínimo de pagamentos feitos pelo usuário
PRCFULLPAYMENT : Porcentagem do pagamento integral pago pelo usuário
TENURE : Prazo do serviço de cartão de crédito para o usuário
