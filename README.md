# Diagramas Conceituais

## Objetivo

Este projeto reúne conceitos, técnicas e ferramentas relacionados à arquitetura de solução, arquitetura de software e tecnologia em geral. O propósito é documentar e visualizar padrões arquiteturais, decisões de design e modelos conceituais para facilitar o entendimento e a comunicação entre equipes técnicas.

## Design

### Arquitetura
- **Padrões Arquiteturais**: Documentação de padrões como MVC, MVVM, Hexagonal, Microserviços, etc.
- **Estilos Arquiteturais**: Representações de arquiteturas em camadas, orientada a eventos, baseada em componentes, etc.
- **Decisões Arquiteturais**: Registro de decisões tomadas e seus fundamentos (ADRs - Architecture Decision Records)

### Design de Código
- **Padrões de Design**: Implementações e exemplos de padrões GoF (Factory, Singleton, Observer, etc.)
- **Princípios SOLID**: Diagramas explicativos dos princípios de design orientado a objetos
- **Clean Code**: Ilustrações de boas práticas de codificação

## Implementação
- **PlantUML**: Utilizado para criar diagramas através de código
  - Diagramas de Classe
  - Diagramas de Sequência
  - Diagramas de Componentes
  - Diagramas de Estado
- **Mermaid**: Alternativa para diagramas via Markdown
- **Draw.io/diagrams.net**: Diagramas mais complexos e personalizados

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


Este projeto está licenciado sob [incluir licença escolhida].