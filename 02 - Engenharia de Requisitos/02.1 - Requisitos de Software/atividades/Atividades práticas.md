## Seguradora de Automóveis

Em uma seguradora de automóveis, os corretores pesquisam, mensalmente, os cadastros das apólices e de segurados, visando a renovação dos seguros em vigor. Com base nas informações das apólices e da tabela de preços dos seguros – fornecido pelo Departamento de Operações – preparam e enviam aos segurados, cujo seguro vence no mês seguinte, a nova apólice de seguro.

Quando um novo cliente contrata um seguro, o corretor cadastra esse novo cliente no cadastro de segurados e emite a apólice correspondente. A importância segurada é definida pela Tabela FIPE que está disponível em um site na internet.

O segurado paga a apólice na rede de bancos autorizados. Semanalmente, os bancos informam à seguradora os valores pagos mensalmente; em função das apólices pagas, são calculadas as comissões dos vendedores, os quais são informados ao Departamento Financeiro para pagamento.

As apólices não pagas dentro do prazo de vencimento são automaticamente canceladas, sendo enviado um “Aviso de Cancelamento de Apólice” ao segurado.

Toda vez que um seguro é utilizado, o corretor, após ser informado pelo Departamento de Operações, registra o fato na respectiva apólice.

O corretor gostaria, com a implantação do novo sistema, poder gerar a qualquer momento um relatório com as informações dos clientes que fazem parte da sua carteira. Nesse relatório, aparecem outras informações, além da data de renovação do seguro.

Os segurados já cadastrados podem atualizar seus dados (tais como, placa do veículo, endereço, telefone, etc.) através do “Formulário de Atualização Cadastral”, que pode ser entregue pessoalmente na seguradora, enviado pelo correio ou preenchido e submetido via internet.

**Questão 01** - Considerando o texto sobre a seguradora de automóveis, faça uma lista com  pelo menos 10  requisitos funcionais.

**Requisitos funcionais**

- RF01 O sistema fornece um relatório dos seguros que vencem no mês seguinte ao da pesquisa.
- RF02 O sistema cadastra novo cliente.
- RF03 O sistema cadastra apólice de seguro para um dado cliente.
- RF04 O sistema registra os seguros pagos pelo cliente (enviado pelo banco) mensalmente.
- RF05 O sistema cancela apólice de seguros.
- RF06 O sistema registra na apólice a utilização do seguro.
- RF07 O sistema gera um relatório com informações dos clientes que fazem parte da carteira de um corretor.
- RF08 O sistema atualiza dados dos clientes cadastrados.
- RF09 O sistema envia um “Aviso de Cancelamento de Apólice“ ao segurado.
- RF010 O sistema calcula as comissões dos corretores.

**Questão 02** - Considerando o texto sobre a seguradora de automóveis, faça uma lista com  pelo menos  5 requisitos não funcionais e 3 regras de negócio:

A resposta abaixo é uma possível solução para o problema. Os RNF e RN são pouco abordados no texto acima. Desta forma a solução proposta considera requisitos que fazem sentido com o problema exposto. Num caso real, o analista refinaria a elicitação, pesquisando mais a documentação, entrevistando os envolvidos, etc., para levantar os RNF e RN.

**Requisitos não funcionais**

- RNF01  O sistema deve executar em ambiente Windows 10.
- RNF02  O sistema deve prover senha de acesso para os corretores.
- RNF03 O sistema deve utilizar um banco de dados existente cujo SGBD é o SQL Server .
- RNF04 O corretor poderá acessar o sistema via internet
- RNF05  O “Aviso de Cancelamento de Apólice” deve ser feito via MSM e e-mail.

**Regras de negócio**
- RN01 Se o carro precisar de manutenção a importância segurada é 30% inferior ao especificado na tabela FIPE.
- RN02  O valor a ser pago de comissões é calculado no dia 20 de cada mês ou último dia útil anterior a esta dia e considera as apólices vendidas nos últimos 30 dias anteriores.
- RN03  O cancelamento da apólice ocorre se o cliente atrasar o pagamento por mais de 40 dias.