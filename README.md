# Simulador - Simulador de Proposta de Financiamento Sicoob Maxicrédito

O front-end e o back-end conversam utilizando basicamente JSON em cima do protocolo HTTP.

#Versionamento
As versões seguem o padrão especificado http://semver.org/lang/pt-BR/, portanto tire um tempo para ler e entender.
Utiliza o GIT(http://git-scm.com/) como sistema de versionamento para o fontes, enquanto as alterações no banco de dados
são gerenciadas pelo liquibase.	A versão deve ser controlada por tags no git, e se houver alterações no banco de dados deve
haver uma descrição das alterações no banco de dados com o liquibase.


Requisitos de Infraestrutura:

The postgresql server needs this configuration in postgresql.conf => max_prepared_transactions = 10
The datasource needs to be xa, because de transaction is distributed