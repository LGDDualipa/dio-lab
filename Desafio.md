# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 10/01/2026
Empresa: Moulin Industries 
Responsável: Arthur Moulin

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Moulin Industries, realizado por Arthur Moulin. O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de realizar diminuição de custos imediatos.

## Descrição do Projeto
O projeto de implementação de ferramentas foi estruturado em 3 etapas estratégicas, cada uma com metas específicas voltadas para a criação de um serviço online de vendas. O foco da Abstergo Industries é disponibilizar uma plataforma digital que conecte farmácias da região a uma distribuidora de medicamentos e utilidades médicas, garantindo eficiência, redução de custos e maior alcance comercial.
Esse desafio envolve não apenas a adoção de serviços AWS para suportar a infraestrutura tecnológica, mas também a integração de processos que permitam escalabilidade, segurança e monitoramento contínuo. A seguir, serão detalhadas as etapas do projeto.

### Etapa 1: Servidor Seguro para APP e Site
O objetivo da Primeira etapa é criar uma infraestrutura segura para o aplicativo e o site garantindo segurança, disponibilidade 24/7 e desempenho.
- Amazon EC2:
Criação de instâncias otimizadas para rodar tanto o APP quanto o Site.
Configuração de Auto Scaling para ajustar automaticamente a capacidade conforme a demanda.
O aplicativo e o site será hospedado dentro da infraestrutura de servidores da Amazon utilizando o Servidores EC2, e rodará em autoscaling para garantir um bom desempenho para todos os clientes.

- Amazon VPC:
Controle de tráfego.
Segurança a Informações.

- Ferramentas Anti-DDOS, Filtro Trafego Malicioso.
Implementação de Ferramentas Anti-Ddos e Filtro de trafico malicioso, não necessariamente utilizando Serviços da Amazon mas Alguma solução da CloudFlare.

### Etapa 2: Banco de Dados para Clientes, Pedidos e Estoque
Garantir armazenamento estruturado e seguro das informações de clientes, pedidos e estoque, além de manter registros imutáveis das transações financeiras e movimentações.
- banco de dados Relacional - Amazon RDS:
Utilizaremos o Um banco de dados Relacional, PostgreSQL para o cadastro de clientes, Cadastro de Mercadorias e etc.
- Banco de Dados Não Mutável - Amazon QLDB:
Registro imutável de todas as transações (pedidos e movimentações).
- Será feito uma integrações entre os bancos de dados para que todas as transações da empresa sejá transparente e confiavel, e o banco de dados relacional trabalha com o cadastro de clientes e produtos, taxas e etc.

### Etapa 3: Monitoramento de custos e desempenho, Integração de ferramentas externas
Garantir que o sistema seja sustentável financeiramente, com desempenho estável e seguro, além de oferecer aos clientes uma experiência completa com pagamentos online e acompanhamento de pedidos.
- Monitoramento de Custos e Desempenho:
Ferramentas da AWS Como: Cost Explorer, CloudWatch, Budgets para acompanhar de perto o uso e desempenho da operação buscando reduzir o custo. 
- Integração com Plataformas de Pagamento:
Conexão com APIs de pagamento externas (ex.: PayPal, Stripe, PagSeguro)
- Monitoramento de Pedidos para Clientes:
Desenvolvimento de um painel integrado ao APP/Site para acompanhamento em tempo real.
Utilização de Amazon DynamoDB para armazenar status de pedidos de forma rápida e escalável.




## Conclusão
A implementação de ferramentas na Moulin Industries tem como objetivo principal disponibilizar um aplicativo e um site, capazes de elevar a eficiência operacional e a produtividade da empresa, além de ampliar o alcance das vendas. Recomenda-se a continuidade do uso das soluções já implantadas e a constante busca por novas tecnologias, que possam aprimorar ainda mais os processos internos e fortalecer a competitividade da organização.


Assinatura do Responsável pelo Projeto:

Arthur Moulin