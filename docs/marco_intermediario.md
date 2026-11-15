# Marco Intermediário — Oficina Mecânica

**Projeto:** Sistema de gestão para oficina mecânica
**Instituição:** Centro Universitário UFBRA
**Curso:** Análise e Desenvolvimento de Sistemas (ADS)
**Disciplina:** Projeto de Software
**Equipe:** Franciscana Ribeiro Cintra e Maria Heloísa Macedo
**Data do marco:** 14/11/2026

## Objetivo do marco

Apresentar o modelo orientado a objetos, a arquitetura do primeiro incremento, uma aplicação demonstrável para o fluxo de ordens de serviço, instruções para execução e o histórico de alterações versionadas.

## Entregáveis

| Item | Entrega | Evidência no projeto |
|---|---|---|
| 1. Classes centrais | Seis classes conceituais: `Cliente`, `Veiculo`, `Mecanico`, `OrdemServico`, `ItemServico` e `HistoricoStatus`. O incremento ainda não implementa todas elas no código. | [Modelo OO e UML](uml.md), seções “Classes centrais” e “Correspondência com o incremento implementado”. |
| 2. Atributos, operações e relacionamentos | Tabela de atributos e operações, responsabilidades e regras de associação/composição. | [Modelo OO e UML](uml.md). |
| 3. Diagrama de classes | Diagrama UML em Mermaid, incluindo as classes e enumeração `StatusOS`. | [Modelo OO e UML](uml.md), seção “Diagrama de classes”. |
| 4. Mudança futura e manutenção | Enviar automaticamente atualizações de status pela API oficial do WhatsApp; classificada como manutenção evolutiva. | [Modelo OO e UML](uml.md) e [Arquitetura](arquitetura.md). |
| 5. Primeiro incremento funcional | Cadastro de cliente/veículo, abertura e consulta de OS, lançamento de mão de obra, cálculo do total e mensagens simuladas no histórico de status. | [Aplicação](../index.html), [JavaScript](../app.js) e critérios em [requisitos](requisitos.md). |
| 6. Instruções para executar | Servidor estático local, sem instalação de dependências. | [Arquitetura](arquitetura.md), seção “Como executar o incremento”. |
| 7. Histórico Git | Commits separados para documentação, funcionalidade e ajustes posteriores. | Histórico listado abaixo; consultar também `git log --oneline`. |
| 8. Preparação do marco | Este documento reúne escopo, evidências, limites e roteiro de demonstração. | Este arquivo e links para os documentos detalhados. |

## Primeiro incremento

O incremento implementa o fluxo de atendimento em uma aplicação web estática:

1. Cadastrar cliente e veículo, validando CPF/CNPJ, placa e duplicidade local.
2. Abrir uma OS numerada para um veículo existente.
3. Adicionar serviços de mão de obra com mecânico responsável e valor.
4. Consultar o total calculado e atualizar o status conforme as transições permitidas.
5. Consultar a ordem por número ou placa e visualizar o resumo operacional.

Os dados são salvos no `localStorage` do navegador. Esta versão é uma prova de conceito: não possui autenticação, autorização por perfil, sincronização entre dispositivos ou backup. Deve ser demonstrada apenas com dados fictícios.

## Como executar

Na raiz do projeto, execute:

```sh
python3 -m http.server 8000
```

Depois, abra `http://localhost:8000`. Não é necessário instalar dependências. Para detalhes e limitações, consulte [arquitetura.md](arquitetura.md).

## Roteiro de demonstração

1. Iniciar a aplicação e mostrar o painel vazio.
2. Cadastrar um cliente fictício e seu veículo.
3. Abrir uma ordem e apontar o número e status inicial na fila.
4. Lançar um serviço e mostrar o valor total atualizado.
5. Avançar o status e consultar a OS por número ou placa.
6. Abrir [uml.md](uml.md) para apresentar as classes, relações e a integração futura com WhatsApp classificada como manutenção evolutiva.

## Histórico de commits

| Commit | Alteração |
|---|---|
| `32a57ed` | Preparar documentação do marco e diagramas. |
| `29cc749` | Implementar painel local de ordens de serviço. |
| `54d3653` | Destacar mudança futura e manutenção no documento UML. |
| `c4668c7` | Destacar instruções para executar o incremento. |
| `e6a9e0e` | Registrar mensagens simuladas no histórico de status da OS. |
| `7f73f4f` | Classificar integração futura com WhatsApp como manutenção evolutiva. |

## Documentação relacionada

- [Requisitos do incremento](requisitos.md)
- [Arquitetura e execução](arquitetura.md)
- [Modelo orientado a objetos e UML](uml.md)
- [Requisitos completos do projeto](../REQUISITOS.md)