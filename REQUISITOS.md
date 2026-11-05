# Requisitos e escopo — Oficina Mecânica

## 1. Objetivo

Organizar o atendimento e o acompanhamento de serviços de uma oficina mecânica, mantendo os dados de clientes e veículos relacionados às ordens de serviço e aos serviços executados.

## 2. Usuários e necessidades

| Usuário | Necessidade principal |
|---|---|
| Clientes (donos dos veículos) | Acompanhar os serviços realizados em seus veículos. |
| Recepcionistas/atendentes | Cadastrar o atendimento e repassar informações sobre o serviço. |
| Mecânicos | Consultar as ordens e registrar os serviços executados. |
| Gestores/donos da oficina | Acompanhar a operação e gerenciar o negócio. |

## 3. Escopo da primeira versão

### Incluído

- Cadastro de clientes.
- Cadastro de veículos vinculados aos clientes.
- Abertura de ordens de serviço para registrar um atendimento.
- Acompanhamento do andamento das ordens de serviço.
- Registro dos serviços executados em cada ordem.

### Não definido para a primeira versão

O controle de estoque e peças, pagamentos, emissão fiscal, agendamento, notificações ao cliente, relatórios financeiros e integrações externas não foram especificados e ficam fora do escopo inicial até validação com a equipe.

## 4. Requisitos funcionais

- **RF-01 — Clientes:** o sistema deve permitir cadastrar e consultar clientes.
- **RF-02 — Veículos:** o sistema deve permitir cadastrar veículos e associá-los a um cliente.
- **RF-03 — Ordens de serviço:** o sistema deve permitir abrir uma ordem de serviço para um veículo cadastrado.
- **RF-04 — Acompanhamento:** o sistema deve permitir consultar o andamento das ordens de serviço.
- **RF-05 — Serviços executados:** o sistema deve permitir registrar os serviços realizados em uma ordem de serviço.

## 5. Requisitos não funcionais

- **RNF-01 — Usabilidade:** as operações de cadastro e consulta devem ser claras para os diferentes perfis de usuário.
- **RNF-02 — Integridade:** os veículos devem permanecer associados aos seus clientes e os serviços às respectivas ordens.
- **RNF-03 — Privacidade:** os dados de clientes devem ser acessíveis apenas a usuários autorizados.

## 6. Premissas e pendências

- Os nomes dos integrantes da equipe ainda não foram informados.
- Os estados e regras detalhadas para acompanhamento das ordens precisam ser definidos pela equipe.
- Campos obrigatórios, perfis de acesso e tecnologias de implementação serão detalhados antes do desenvolvimento.
