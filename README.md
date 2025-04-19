# Conceitos de Arquitetura

## Objetivo

Este projeto reúne conceitos, técnicas e ferramentas relacionados à arquitetura de solução, arquitetura de software e tecnologia em geral. O propósito é documentar e visualizar padrões arquiteturais, decisões de design e modelos conceituais para facilitar o entendimento e a comunicação entre equipes técnicas.

## Estrutura

### Architecture Decision Records (ADRs)

Localização: `/000-architecture-decison-records`

Documentação de decisões arquiteturais importantes:

#### Padrões Arquiteturais e Design
- [ADR-011](000-architecture-decison-records/adr-011-ddd-hexagonal.md): DDD e Arquitetura Hexagonal
- [ADR-012](000-architecture-decison-records/adr-012-data-modeling.md): Estratégia de Modelagem de Dados
- [ADR-013](000-architecture-decison-records/adr-013-openapi-standard.md): Padronização de APIs com OpenAPI
- [ADR-019](000-architecture-decison-records/adr-019-twelve-factor.md): Adoção do Padrão 12-Factor App

#### Tecnologias e Linguagens
- [ADR-017](000-architecture-decison-records/adr-017-golang-adoption.md): Adoção de Go para Microsserviços
- [ADR-018](000-architecture-decison-records/adr-018-python-adoption.md): Adoção de Python para Serviços de Dados e ML

#### Segurança e Autenticação
- [ADR-014](000-architecture-decison-records/adr-014-sso-implementation.md): Implementação de SSO com OAuth2/OpenID

#### Comunicação e Integração
- [ADR-016](000-architecture-decison-records/adr-016-messaging-patterns.md): Padrões de Mensageria com RabbitMQ
- [ADR-020](000-architecture-decison-records/adr-020-websocket.md): WebSocket para Comunicação Real-time

#### Qualidade e Testes
- [ADR-015](000-architecture-decison-records/adr-015-test-patterns.md): Padrões de Testes

### Design

#### Arquitetura
- **Padrões Arquiteturais**: Documentação de padrões como MVC, MVVM, Hexagonal, Microserviços, etc.
- **Estilos Arquiteturais**: Representações de arquiteturas em camadas, orientada a eventos, baseada em componentes, etc.
- **Decisões Arquiteturais**: Registro de decisões tomadas e seus fundamentos

#### Design de Código
- **Padrões de Design**: Implementações e exemplos de padrões GoF (Factory, Singleton, Observer, etc.)
- **Princípios SOLID**: Diagramas explicativos dos princípios de design orientado a objetos
- **Clean Code**: Ilustrações de boas práticas de codificação

## Implementação

### Ferramentas de Diagramação

#### PlantUML
- Diagramas de Classe
- Diagramas de Sequência
- Diagramas de Componentes
- Diagramas de Estado

#### Mermaid
- Alternativa para diagramas via Markdown

#### Draw.io/diagrams.net
- Diagramas mais complexos e personalizados

## Como Usar

1. Clone este repositório
2. Instale as dependências necessárias para visualizar os diagramas (ver seção Configuração)
3. Navegue pelos diretórios para encontrar conceitos específicos
4. Utilize os diagramas como referência para seus próprios projetos
5. Gere imagens PNG a partir dos diagramas PlantUML usando o script fornecido

## Configuração

### PlantUML
```bash
# Instalar PlantUML (via homebrew no macOS)
brew install plantuml

# Ou usando Java
java -jar plantuml.jar [arquivo]
```

### Script Gerador de PNG

Este projeto inclui um script utilitário `generate-plantuml-png.sh` que facilita a geração de arquivos PNG a partir de diagramas PlantUML (.wsd).

#### Características do Script:
- Converte arquivos PlantUML (.wsd) em imagens PNG
- Processa títulos de diagramas corretamente
- Salva a imagem resultante no mesmo diretório do arquivo fonte
- Fornece feedback detalhado sobre o processo

#### Utilização:
```bash
# Conceda permissão de execução (somente uma vez)
chmod +x generate-plantuml-png.sh

# Execute o script informando o caminho para o arquivo .wsd
./generate-plantuml-png.sh caminho/para/seu-diagrama.wsd

# Exemplo:
./generate-plantuml-png.sh arch-concepts/000-maquina-estado/000-maquina-estado.wsd
```

O script automaticamente baixará o PlantUML.jar se necessário e colocará a imagem PNG resultante no mesmo diretório do arquivo de origem.

## Licença

Este projeto está licenciado sob a licença MIT.