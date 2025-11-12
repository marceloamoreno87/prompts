# Regras e Comandos do Cursor

Este diretório contém regras e comandos personalizados para o Cursor AI.

## Estrutura

```
.cursor/
├── rules/          # Regras de desenvolvimento
│   ├── backend.mdc    # Regras para projetos backend (Go)
│   ├── frontend.mdc   # Regras para projetos frontend (Next.js)
│   ├── infra.mdc      # Regras para infraestrutura (Docker/Containers)
│   └── general.mdc    # Regras gerais compartilhadas
└── commands/       # Comandos personalizados
    ├── tasks.md       # Gerar tarefas estruturadas
    ├── code-review.md # Revisar código
    ├── refactor.md    # Refatorar código
    ├── debug.md       # Debugar problemas
    └── optimize.md    # Otimizar performance
```

## Regras (Rules)

### Backend (`rules/backend.mdc`)
Template completo para gerar setup de backend em Go:
- Go 1.25+
- Gin framework
- PostgreSQL 16 + Redis 7
- Hot reload com air
- Clean Architecture
- Swagger para documentação

### Frontend (`rules/frontend.mdc`)
Template completo para gerar setup de frontend em Next.js:
- Next.js 15+
- Node.js 22+
- Tailwind CSS + shadcn/ui
- Hot reload com Fast Refresh
- Dark/Light mode obrigatório
- App Router

### Infraestrutura (`rules/infra.mdc`)
Template para infraestrutura com containers:
- Docker + Docker Compose
- Ambiente 100% desenvolvimento
- Hot reload configurado
- Variáveis de ambiente em `.env`

### Geral (`rules/general.mdc`)
Regras compartilhadas entre backend e frontend:
- Padrões de nomenclatura
- Gerenciamento de variáveis de ambiente
- Versionamento Git
- Qualidade de código
- Segurança básica

## Comandos (Commands)

### Gerar Tarefas (`commands/tasks.md`)
Gera tarefas estruturadas em arquivos Markdown:
- Timestamp automático
- Formato padronizado
- Status, prioridade, dependências
- Tags opcionais

### Revisão de Código (`commands/code-review.md`)
Revisa código gerado com checklist completo:
- Arquitetura e estrutura
- Performance
- Segurança
- Padrões de código

### Refatoração (`commands/refactor.md`)
Refatora código existente:
- Extração de funções/componentes
- Simplificação de lógica
- Melhoria de nomenclatura
- Otimização de performance

### Debug (`commands/debug.md`)
Ajuda a debugar problemas:
- Análise sistemática
- Identificação de causa raiz
- Soluções específicas

### Otimização (`commands/optimize.md`)
Otimiza código para performance:
- Análise de gargalos
- Otimizações de banco de dados
- Otimizações de renderização
- Implementação de cache

## Princípios Gerais

- **Ambiente 100% Desenvolvimento:** Nenhuma configuração de produção
- **Sem Testes:** Não criar arquivos de teste
- **Sem Documentação Extensa:** Apenas Swagger para backend
- **Sem Comentários:** Código autoexplicativo
- **Sem CI/CD:** Não incluir configurações de CI/CD
- **Variáveis em .env:** Nunca no docker-compose.yml

## Versões Mínimas

- **Go:** 1.25+
- **Node.js:** 22+
- **Next.js:** 15+
- **PostgreSQL:** 16
- **Redis:** 7

## Uso

Para usar as regras, referencie o arquivo `.mdc` apropriado no contexto do Cursor.

Para usar os comandos, referencie o arquivo `.md` apropriado e siga as instruções.

