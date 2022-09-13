#Projeto Conceitual de BD Relacional

Este modelo de Banco de Dados (BD) foi elaborado considerando o contexto de uma **oficina mecânica**.

Para a construção do modelo e entendimento do contexto, foi considerado o cenário de realização do primeiro contato com o cliente, onde é feito o **levantamento de informações** que contribui para a elaboração do primeiro **draft**.

Após o contato com o cliente, o contexto a ser considerado é de uma aplicação de controle e gerenciamento de execução de ordens de serviço (revisão, manutenção, reparo, troca de peças).

No levantamento de requisitos, obtemos a seguinte **narrativa**:

* Clientes levam veículos à oficina mecânica para serem consertados ou para passarem por revisões  periódicas;
* Cada veículo é designado a uma equipe de mecânicos que identifica os serviços a serem executados e preenche uma OS com data de entrega;
* A partir da OS, calcula-se o valor de cada serviço, consultando-se uma tabela de referência de mão-de-obra;
* O valor de cada peça também irá compor a OSO cliente autoriza a execução dos serviços;
* A mesma equipe avalia e executa os serviços;
* Os mecânicos possuem código, nome, endereço e especialidade;
* Cada OS possui: n°, data de emissão, um valor, status e uma data para conclusão dos trabalhos.
  
  

O cliente leva seu veículo até a oficina para uma avaliação; após a avaliação, o orçamento é apresentado ao cliente que aprovando, realiza o pagamento . Após confirmação do pagamento, o orçamento é executado pela área operacional.

Neste primeiro momento, percebemos a relevância das seguintes entidades: 

- cliente;
- veículo;
- ordem de serviço;
- estoque;
- colaboradores;
- fornecedor.



Em reuniões com o cliente, são apresentados os draft's, onde o cliente realiza considerações, o modelo passa por aprimoramentos até sua conclusão. As entidades irão receber atributos, serão estabelecidos relacionamentos entre elas e outras tratativas. Em meio a esses aprimoramentos, partimos de algo simples, para algo mais elaborado, ou seja, um modelo de BD que irá atender ao contexto.

Realizamos o mapeamento de Entidade de Relacionamento **(ER)**, e dele, partimos para o **Diagrama do Modelo Relacional**.

A ferramenta utilizada é o MySQL Workbench.

Após a conclusão, o arquivo é gerado em formato **png**.

###Resumo:###

O **cliente**, que pode ser Pessoa Física ou Pessoa Jurídica, leva o veículo para avaliação.

O primeiro contato é feito pala área de **atendimento**. O recepcionista direciona o veículo para o colaborador responsável pela avaliação.

Após a avaliação, o **orçamento** é apresentado ao cliente para sua aprovação. O orçamento contém a relação do serviço a ser prestado, assim como a relação de peças a serem trocadas. 

Os **fornecedores** abastecem o estoque, que deve ser constantemente acompanhado, garantindo a disponibilização de peças.

Feito o pagamento, a área operacional realiza a execução do serviço. O **pagamento** pode ser realizado com cartão de crédito, dinheiro ou pix.

A área responsável observa a data de entrega para que o veículo seja entregue conforme previsto.


