# Telco-Churn-Customers

A análise foi realizada utilizando a base de clientes da IBM que pode ser acessada no kaggle pelo link https://www.kaggle.com/datasets/blastchar/telco-customer-churn.

A motivação da análise é entender quais fatores levam o cliente ao churn (quando o cliente cancela o serviço em determinado período de tempo). Sabendo quais clientes estão propícios ao churn, a empresa pode destinar ações e oferecer descontos/melhorias para reter o cliente.

Algumas perguntas que tentaremos responder:
* Quantidade de clientes que deixaram o serviço?
* Distribuição por gênero?
* Distribuição por parceiros?
* Clientes possuem telefone? serviço de internet? Streaming de TV? Streaming de Filmes?
* Qual o método de pagamento mais comum entre os clientes?
* Qual o tipo de contrato mais comum entre os clientes? 
* O tipo do pagamento influência em cancelarem o serviço?
* O tipo de contrato influência em cancelarem o serviço?
* Clientes que pagam mais por mês, tem mais chance de cancelaram o serviço? e no total de gastos?
* Clientes que possuem mais tempo de utilização, tem menos chances de cancelar o contrato?

# Conclusão

Realizando a análise da base podemos chegar a algumas conclusões:
* Os genêros estão equilibrados, possuímos cerca de 50,4 % de mulheres e 49,6% de homens.
* Uma pequena maioria não possui parceiros, cerca de 51,7%.
* O perfil mais comum de cliente é ter um telefone, internet por fibra ótica, não possuir streaming de TV e nem de filmes. 
* O método preferido de pagamento é o boleto eletrônico, 33% dos clientes preferem isso.
* O tipo de contrato preferido é o renovado mensalmente, 55% dos clientes preferem utilizar ele, o que mostra uma dificuldade na fidelização do cliente.
* A maioria dos clientes que cancelou o serviço, utilizam o método de pagamento por boleto eletrônico, isso se dá pelo motivo de esse ser o método mais comum entre quem paga mensalmente, sendo mais fácil sair do serviço quando quiser.
* O tipo de contrato mais comum entre os clientes que sairam do serviço, é o contrato mensal conforme esperado. Os clientes que possuem contrato anual, possuem uma taxa baixissíma de cancelamento.
* Os clientes que mais saíram do serviço são aqueles que possuem uma taxa mensal mais alta.
* Em contrapartida, clientes que possuem uma taxa total de pagamento menor deixam mais o serviço. Isso pode indicar que são clientes que não utilizaram por muito tempo o serviço, acabam saindo antes de terem gastado mais dinheiro.
* Clientes tem uma tendência grande de sair do serviço no primeiro mês e isso vai diminuindo com o passar do tempo, ou seja, quanto mais tempo de serviço, menor as chances de saída. Então o ideal seria identificar quais clientes tem essa chance para já oferecer boas condições para o cliente não deixar o serviço após o primeiro mês.

Foi realizada a aplicação dos modelos de machine learning e o que melhor se comportou foi o naive bayes, atigindo 84% de recall com os dados de teste. Com dados desconhecidos atingiu 83% de recall, indicando uma boa acurácia para aquilo que tentamos encontrar. A cada 100 funcionários que poderiam deixar o serviço, ele está conseguindo identificar 84 corretamente e dando uma chance para tentar impedir que esses clientes deixem o serviço.
