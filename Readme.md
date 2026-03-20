#  Restaurant Order Management System (SQL)

Este projeto apresenta a modelagem de um banco de dados relacional para o gerenciamento de pedidos em um restaurante, cobrindo desde o cadastro de clientes até o detalhamento do consumo.

##  Arquitetura da Solução
A estrutura foi desenhada para garantir rapidez no atendimento e precisão no fechamento de contas:
- **Clientes:** Cadastro básico para fidelização e contato.
- **Cardápio (Pratos):** Gestão de itens disponíveis e seus respectivos preços.
- **Pedidos:** Registro cronológico das solicitações vinculadas aos clientes.
- **Detalhamento de Itens:** Estrutura que permite múltiplos pratos em um único pedido (relação N:M resolvida com tabela de junção).

##  Tecnologias
- **MySQL / MariaDB**

##  Diferenciais Técnicos
- **Integridade de Dados:** O uso de chaves estrangeiras impede que um pedido seja registrado sem um cliente ou que itens inexistentes sejam adicionados.
- **Precisão Financeira:** Uso do tipo `DECIMAL` para evitar erros de arredondamento comuns em sistemas financeiros.
- **Histórico Automático:** Implementação de `DEFAULT CURRENT_TIMESTAMP` para registro automático do horário do pedido.
