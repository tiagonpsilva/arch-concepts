# Architecture Decision Records (ADRs)

Este diretório contém os Architecture Decision Records (ADRs) do projeto, que documentam decisões arquiteturais importantes.

## Estrutura do Diretório

- `README.md` - Este arquivo
- `template.md` - Template para novos ADRs
- `adr-001-typescript-frontend.md` - Adoção de TypeScript para Frontend
- `adr-002-react-query.md` - Uso do React Query para Gerenciamento de Estado
- `adr-003-microservices.md` - Migração para Arquitetura de Microsserviços
- `adr-004-cqrs.md` - Adoção do Padrão CQRS
- `adr-005-oauth-openid.md` - Implementação de OAuth 2.0 e OpenID Connect
- `adr-006-mongodb-profiles.md` - Adoção de MongoDB para Dados de Perfil
- `adr-007-graphql-api.md` - Adoção de GraphQL para APIs Públicas
- `adr-008-cd-canary.md` - Implantação Contínua com Canary Releases
- `adr-009-git-flow.md` - Estratégia Git Flow e Branching
- `adr-010-cloud-aws.md` - Adoção da AWS como Plataforma Cloud

## Como usar este diretório

1. Para criar um novo ADR, use o arquivo `template.md` como base
2. Nomeie o novo arquivo seguindo o padrão `adr-NNN-titulo-descritivo.md`
3. Atualize este README.md adicionando o novo ADR à lista acima
4. Submeta o ADR para revisão através de um pull request

## Melhores Práticas

- Mantenha os ADRs concisos e diretos
- Use linguagem clara e evite jargões desnecessários
- Referencie outros ADRs quando relevante
- Mantenha o status do ADR atualizado
- Discuta os ADRs em reuniões de arquitetura antes da aprovação final 