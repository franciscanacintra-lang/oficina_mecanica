# Changelog

Todas as mudanças relevantes deste projeto serão registradas neste arquivo.

O formato é baseado em Keep a Changelog e usa versionamento semântico.

## [Não publicado]

### Planejado

- Cadastro real da entidade Mecânico.
- Migrar persistência local para API e banco relacional.
- Implementar autenticação e acesso por perfil.
- Integrar envio real de notificações após configuração segura.

## [1.2.0] - 2026-11-22

### Adicionado

- Plano incremental do projeto em `docs/plano_incremental.md`.
- Testes unitários para abertura da OS, histórico e atualizações de status em `tests/test_sistema_oficina.py`.
- Organização das mudanças em releases `v1.0-mvp`, `v1.1.0` e `v1.2.0`.
- Registro de branches por finalidade: `feature/*`, `fix/*`, `docs/*` e `release/*`.

### Corrigido

- Consulta por placa normalizada no painel web para remover caracteres não alfanuméricos antes da busca.
- Documentação corrigida para não afirmar banco relacional, autenticação ou envio real de WhatsApp no MVP atual.
- Centralização dos nomes dos processos no DFD gráfico.
- Remoção de conexões sem destino no DFD e retorno do processo de indicadores ao Gestor.

### Evidências

- Execução do MVP Python pelo terminal.
- Quatro testes unitários aprovados no MVP Python.
- Validação de sintaxe JavaScript e Python.
- Histórico Git com commits significativos e tag de versão.

## [1.1.0] - 2026-11-22

### Adicionado

- Painel web para cadastro, veículos, OS, itens e status.
- Mensagens simuladas no histórico de atualizações.
- Diagrama de contexto, DFD nível 0, dicionário de dados e relatório de ajustes.
- UML conceitual de seis classes.
- SVGs de contexto e DFD para uso no LibreOffice.

### Corrigido

- Separação entre classes conceituais e classes efetivamente implementadas.
- Classificação da integração com WhatsApp como manutenção evolutiva.
- Diferenciação dos estados usados pelo MVP Python e pelo painel web.

## [1.0-mvp] - 2026-11-14

### Adicionado

- Primeiro incremento Python de controle de status.
- Histórico de abertura, diagnóstico/reparo e conclusão.
- Painel textual de consulta da OS.
- Documentação inicial do requisito, arquitetura, README e UML.
