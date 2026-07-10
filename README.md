# ERP Drakkars Community

Sistema ERP Open Source desenvolvido pela Drakkars Consultoria.

Construído com Django, PostgreSQL e RHEL 10 utilizando exclusivamente tecnologias Open Source.

---

## Status do Projeto

> **Versão Atual:** 0.1.0-alpha

Este projeto encontra-se em desenvolvimento ativo.

O objetivo é construir um ERP moderno, modular, altamente documentado e preparado para ambientes corporativos.

---

# Sobre o Projeto

O **ERP Drakkars Community** é um Enterprise Resource Planning (ERP) Open Source desenvolvido pela **Drakkars Consultoria**.

Nosso objetivo não é apenas desenvolver um ERP.

Queremos construir uma plataforma que também seja uma referência em documentação técnica, arquitetura de software e boas práticas de desenvolvimento.

Todo o projeto será desenvolvido publicamente através do GitHub.

---

# Objetivos

O ERP Drakkars foi criado para atender quatro grandes objetivos.

## 1. Ser totalmente Open Source

Todo o código-fonte será disponibilizado publicamente.

Todo o desenvolvimento acontecerá no GitHub.

Todo o roadmap será público.

---

## 2. Ser fácil de instalar

Qualquer pessoa deverá conseguir instalar o ERP seguindo apenas a documentação oficial.

Nosso foco é que até mesmo profissionais iniciantes consigam colocar o sistema em funcionamento.

---

## 3. Servir como material de estudo

A documentação explicará muito mais do que comandos.

Ela ensinará:

- Linux
- RHEL
- PostgreSQL
- Django
- Python
- Git
- Nginx
- Gunicorn
- Segurança
- Deploy

Nosso objetivo é transformar este projeto em uma excelente fonte de aprendizado.

---

## 4. Ser preparado para produção

O sistema será desenvolvido seguindo padrões utilizados em aplicações corporativas.

Desde o início serão considerados aspectos como:

- Segurança
- Escalabilidade
- Organização
- Modularização
- Testes automatizados
- Documentação
- Monitoramento

---

# Filosofia do Projeto

O ERP Drakkars segue alguns princípios fundamentais.

## Simplicidade

Sempre escolheremos soluções simples antes de soluções complexas.

Código simples é mais fácil de manter.

---

## Legibilidade

Todo código deve ser fácil de ler.

Se um desenvolvedor não conseguir entender uma função rapidamente, ela provavelmente precisa ser melhorada.

---

## Documentação

Nenhuma funcionalidade será entregue sem documentação.

Todo módulo possuirá documentação própria.

---

## Qualidade

Todo código deverá seguir padrões definidos pelo projeto.

Utilizaremos ferramentas automatizadas para validação.

---

## Evolução Contínua

O projeto será desenvolvido em pequenas entregas.

Cada versão será melhor que a anterior.

---

# Arquitetura

```text
                    Usuário

                       │

                       ▼

                  Navegador

                       │

                       ▼

                    Nginx

                       │

                       ▼

                  Gunicorn

                       │

                       ▼

                    Django

                       │

                       ▼

                 PostgreSQL
```

Toda a aplicação será executada sobre RHEL 10.

---

# Stack Tecnológica

| Camada | Tecnologia |
|----------|------------|
| Sistema Operacional | RHEL 10 |
| Linguagem | Python 3.13+ |
| Framework | Django 5 LTS |
| Banco de Dados | PostgreSQL |
| Servidor WSGI | Gunicorn |
| Reverse Proxy | Nginx |
| Front-End | HTML5 |
| CSS | Bootstrap 5 |
| JavaScript | Vanilla JavaScript |
| Versionamento | Git |
| Licença | MIT |

---

# Recursos Planejados

A versão inicial possuirá os seguintes módulos.

- Login
- Dashboard
- Clientes
- Produtos
- Estoque
- Pedidos
- Financeiro
- Compras
- Relatórios
- Usuários
- Permissões
- API REST
- Auditoria
- Backup
- Configurações

Novos módulos serão adicionados conforme o roadmap do projeto.

---

# Estrutura do Repositório

```text
erp_drakkars/

├── apps/
├── config/
├── docs/
├── scripts/
├── database/
├── tests/
├── static/
├── templates/
├── media/
├── requirements/
├── .github/
├── README.md
├── LICENSE
├── CHANGELOG.md
├── CONTRIBUTING.md
├── SECURITY.md
└── pyproject.toml
```

---

# Organização dos Módulos

Cada funcionalidade do ERP será implementada como um aplicativo Django independente.

Exemplo:

apps/

- accounts
- dashboard
- customers
- products
- inventory
- sales
- finance
- reports
- administration

Essa organização facilita manutenção, testes e evolução do sistema.

---

# Público-Alvo

Este projeto é destinado a:

- Desenvolvedores Python
- Administradores Linux
- Empresas
- Consultorias
- Estudantes
- Profissionais de infraestrutura
- Comunidade Open Source

---

# Licença

Este projeto utiliza a licença MIT.

Mais informações podem ser encontradas no arquivo LICENSE.

---
# Roadmap

O desenvolvimento do ERP Drakkars será incremental. Cada versão adicionará novos recursos, mantendo estabilidade, documentação e testes automatizados.

| Versão | Objetivo | Status |
|---------|----------|:------:|
| 0.1.0-alpha | Fundação do projeto | 🚧 Em desenvolvimento |
| 0.2.0-alpha | Ambiente Django + PostgreSQL | ⏳ |
| 0.3.0-alpha | Sistema de autenticação | ⏳ |
| 0.4.0-alpha | Dashboard | ⏳ |
| 0.5.0-alpha | Cadastro de clientes | ⏳ |
| 0.6.0-alpha | Cadastro de produtos | ⏳ |
| 0.7.0-alpha | Controle de estoque | ⏳ |
| 0.8.0-alpha | Pedidos de venda | ⏳ |
| 0.9.0-alpha | Financeiro | ⏳ |
| 1.0.0 | Primeira versão estável | ⏳ |

---

# Princípios de Desenvolvimento

Todo o projeto segue alguns princípios fundamentais.

## Clean Code

Todo código deverá ser:

- Simples
- Organizado
- Reutilizável
- Fácil de manter
- Bem documentado

---

## Clean Architecture

Separaremos responsabilidades entre:

- Interface
- Regras de negócio
- Persistência
- Infraestrutura

Essa divisão reduz o acoplamento entre os módulos.

---

## SOLID

Sempre que fizer sentido, seguiremos os princípios SOLID para tornar o código escalável.

---

## Segurança desde o início

Segurança não será uma etapa final.

Ela fará parte do desenvolvimento desde o primeiro commit.

Entre as medidas adotadas estarão:

- CSRF Protection
- Password Hashing
- ORM (evitando SQL Injection)
- Validação de entrada
- Escape automático de HTML
- Controle de permissões
- Auditoria
- Logs
- HTTPS em produção

---

# Estrutura dos Diretórios

A organização do projeto foi planejada para facilitar crescimento e manutenção.

```text
erp_drakkars/

apps/
│
├── accounts/
├── dashboard/
├── customers/
├── products/
├── inventory/
├── sales/
├── finance/
├── reports/
└── administration/

config/

docs/

database/

scripts/

tests/

templates/

static/

media/

requirements/

.github/
```

Cada diretório possui uma responsabilidade específica.

A documentação completa encontra-se na pasta `docs/`.

---

# Arquitetura da Aplicação

```text
                  Browser

                     │

                     ▼

               Nginx (Reverse Proxy)

                     │

                     ▼

              Gunicorn (WSGI Server)

                     │

                     ▼

             Django Application

                     │

                     ▼

               PostgreSQL Database
```

Essa arquitetura é amplamente utilizada em aplicações corporativas.

---

# Fluxo de uma Requisição

```text
Usuário

↓

Navegador

↓

Nginx

↓

Gunicorn

↓

Django URL

↓

View

↓

Service

↓

Model

↓

PostgreSQL

↓

Resposta

↓

Usuário
```

---

# Organização dos Aplicativos

Cada módulo do ERP será um aplicativo Django independente.

Exemplo:

```text
apps/

accounts/

customers/

products/

inventory/

sales/

finance/

reports/
```

Isso permite evolução independente de cada módulo.

---

# Convenções de Código

Para manter o projeto organizado utilizaremos os seguintes padrões.

## Python

- PEP 8
- Type Hints
- Docstrings
- Ruff
- Black
- isort

---

## Git

Utilizaremos Conventional Commits.

Exemplos:

```text
feat(auth): add login page

fix(database): correct migration

docs(readme): update installation guide

refactor(products): simplify service layer

test(accounts): add login tests
```

---

# Versionamento

O projeto utiliza Semantic Versioning.

Formato:

```text
MAJOR.MINOR.PATCH
```

Exemplo:

```text
1.4.2
```

Onde:

MAJOR

Mudanças incompatíveis.

MINOR

Novas funcionalidades.

PATCH

Correções de bugs.

---

# Branches

O fluxo de desenvolvimento seguirá o padrão Git Flow simplificado.

```text
main

develop

feature/*

bugfix/*

hotfix/*
```

Exemplos:

```text
feature/login

feature/customers

feature/products

bugfix/dashboard

hotfix/security
```

---

# Qualidade de Código

Todo Pull Request deverá passar pelas seguintes validações.

- Formatação automática
- Linter
- Testes unitários
- Testes de integração
- Cobertura mínima
- Revisão de código

Nenhum código será enviado diretamente para a branch principal.

---

# Documentação

Toda documentação oficial encontra-se na pasta:

```text
docs/
```

Ela será dividida em módulos independentes.

Exemplo:

```text
00-PROJETO.md

01-RHEL10.md

02-LINUX.md

03-GIT.md

04-PYTHON.md

05-DJANGO.md

06-POSTGRESQL.md

07-DATABASE.md

08-NGINX.md

09-GUNICORN.md

10-SELINUX.md

11-FIREWALLD.md

12-API.md

13-DEPLOY.md

14-BACKUP.md

15-TROUBLESHOOTING.md

16-ROADMAP.md
```

Nosso objetivo é que qualquer pessoa consiga instalar o ERP apenas seguindo essa documentação.

---
---

# Requisitos do Sistema

Antes de instalar o ERP Drakkars, verifique se seu ambiente atende aos requisitos mínimos.

## Ambiente Recomendado

| Componente | Recomendado |
|------------|-------------|
| Sistema Operacional | Red Hat Enterprise Linux 10 |
| CPU | 4 vCPUs |
| Memória RAM | 8 GB |
| Armazenamento | 50 GB SSD |
| Python | 3.13 ou superior |
| PostgreSQL | 17 ou superior |
| Nginx | Última versão estável |
| Gunicorn | Última versão estável |

---

## Ambiente de Desenvolvimento

| Recurso | Valor |
|----------|-------|
| VS Code | Última versão |
| Git | 2.45+ |
| Python | 3.13+ |
| PostgreSQL | 17+ |
| Navegador | Chrome, Firefox ou Edge |

---

# Sistemas Operacionais Suportados

| Sistema | Status |
|----------|:------:|
| Red Hat Enterprise Linux 10 | ✅ Oficial |
| Rocky Linux 10 | ✅ Compatível |
| AlmaLinux 10 | ✅ Compatível |
| Oracle Linux 10 | ✅ Compatível |
| Fedora | ⚠️ Apenas para desenvolvimento |
| Ubuntu | ❌ Não suportado oficialmente |
| Debian | ❌ Não suportado oficialmente |
| Windows | ❌ Não suportado |
| macOS | ⚠️ Apenas para desenvolvimento |

> **Observação:** Toda a documentação deste projeto será baseada no **Red Hat Enterprise Linux 10 (RHEL 10)**.

---

# Estrutura Geral do Projeto

```text
                    ERP Drakkars

                         │
                         ▼

                 Interface Web (Bootstrap)

                         │
                         ▼

                 Django Views / Templates

                         │
                         ▼

                 Camada de Serviços

                         │
                         ▼

                    Django ORM

                         │
                         ▼

                   PostgreSQL 17
```

---

# Arquitetura Modular

O ERP será dividido em módulos independentes.

Cada módulo terá seu próprio:

- Models
- Views
- URLs
- Templates
- Services
- Forms
- Tests
- Documentação

Essa abordagem facilita manutenção, testes e evolução.

---

# Módulos Planejados

## Administração

- Login
- Usuários
- Grupos
- Permissões
- Configurações
- Auditoria

---

## Dashboard

- Indicadores
- Resumo Financeiro
- Vendas
- Estoque
- Alertas
- Atividades Recentes

---

## Clientes

- Cadastro
- Endereços
- Contatos
- Histórico
- Pesquisa Avançada

---

## Produtos

- Cadastro
- Categorias
- Marcas
- Unidade de Medida
- Código de Barras
- Controle de Ativação

---

## Estoque

- Entrada
- Saída
- Inventário
- Ajustes
- Movimentações
- Localização

---

## Compras

- Fornecedores
- Pedidos
- Recebimento
- Custos

---

## Vendas

- Orçamentos
- Pedidos
- Faturamento
- Entregas

---

## Financeiro

- Contas a Receber
- Contas a Pagar
- Fluxo de Caixa
- Centros de Custo
- Plano de Contas
- Conciliação

---

## Relatórios

- Financeiro
- Comercial
- Estoque
- Clientes
- Produtos

---

# Recursos Planejados para Versões Futuras

- API REST completa
- Autenticação JWT
- Multiempresa
- Multiusuário
- Multiidioma
- Multi-moeda
- Dashboards personalizados
- Workflow de aprovação
- Assinatura digital
- Exportação para PDF
- Exportação para Excel
- Integração com APIs externas
- Webhooks
- Auditoria completa
- Logs estruturados
- Sistema de notificações
- Filas assíncronas
- Cache distribuído
- Monitoramento
- Observabilidade

---

# Tecnologias Utilizadas

## Backend

- Python
- Django
- Django ORM

## Banco de Dados

- PostgreSQL

## Frontend

- HTML5
- CSS3
- Bootstrap 5
- JavaScript

## Servidor

- Gunicorn
- Nginx

## Sistema Operacional

- Red Hat Enterprise Linux 10

## Ferramentas

- Git
- GitHub
- VS Code
- Ruff
- Black
- isort
- pytest

---

# Estrutura de Desenvolvimento

```text
GitHub

        │

        ▼

Feature Branch

        │

        ▼

Pull Request

        │

        ▼

Code Review

        │

        ▼

Testes Automatizados

        │

        ▼

Branch Main
```

Todo código deverá seguir esse fluxo.

---

# Política de Qualidade

Antes de cada release serão executadas validações automáticas.

Entre elas:

- Lint
- Formatação
- Testes Unitários
- Testes de Integração
- Cobertura de Código
- Verificação de Segurança
- Build

Nenhuma versão será publicada sem aprovação dessas etapas.

---

# Filosofia de Documentação

A documentação é considerada parte do software.

Nenhuma funcionalidade será considerada concluída sem:

- Código
- Testes
- Documentação
- Atualização do Changelog
- Atualização do Roadmap (quando aplicável)

Essa política garante que o projeto permaneça útil tanto para usuários quanto para desenvolvedores.

---

# Nosso Compromisso

O ERP Drakkars será desenvolvido com foco em:

- Código limpo
- Arquitetura modular
- Segurança
- Escalabilidade
- Facilidade de instalação
- Documentação de excelência
- Uso exclusivo de tecnologias Open Source

Nosso objetivo é criar um ERP que possa ser utilizado em ambientes reais e, ao mesmo tempo, servir como referência técnica para estudantes e profissionais.

---
---

# Quick Start

A documentação completa de instalação está disponível na pasta `docs/`.

Para usuários experientes, o processo resumido será:

```bash
git clone https://github.com/drakkars-consultoria/erp_drakkars.git

cd erp_drakkars

# Consulte a documentação em docs/01-RHEL10.md
```

A instalação completa será documentada passo a passo para o Red Hat Enterprise Linux 10.

---

# Estrutura da Documentação

Toda a documentação oficial encontra-se na pasta `docs`.

```text
docs/

00-PROJETO.md
01-RHEL10.md
02-LINUX.md
03-GIT.md
04-PYTHON.md
05-DJANGO.md
06-POSTGRESQL.md
07-DATABASE.md
08-NGINX.md
09-GUNICORN.md
10-SELINUX.md
11-FIREWALLD.md
12-API.md
13-DEPLOY.md
14-BACKUP.md
15-TROUBLESHOOTING.md
16-ROADMAP.md
```

Nosso objetivo é que qualquer profissional consiga instalar, configurar, administrar e evoluir o ERP apenas consultando essa documentação.

---

# Como Contribuir

Contribuições são muito bem-vindas.

Antes de enviar alterações, leia atentamente:

- CONTRIBUTING.md
- CODE_OF_CONDUCT.md
- SECURITY.md

Todo Pull Request será revisado antes da integração ao projeto.

---

# Fluxo de Desenvolvimento

```text
Issue

↓

Nova Branch

↓

Desenvolvimento

↓

Testes

↓

Documentação

↓

Pull Request

↓

Code Review

↓

Merge
```

Seguiremos uma política de desenvolvimento baseada em qualidade, revisão de código e integração contínua.

---

# Versionamento

Este projeto utiliza Semantic Versioning.

Exemplo:

0.1.0-alpha

↓

0.2.0-alpha

↓

0.5.0-beta

↓

1.0.0

Todas as mudanças relevantes serão registradas em:

CHANGELOG.md

---

# Segurança

A segurança faz parte da arquitetura do projeto.

Entre as medidas adotadas estão:

- HTTPS em produção
- Hash seguro de senhas
- Proteção contra CSRF
- Proteção contra SQL Injection
- Proteção contra XSS
- Controle de permissões
- Logs de auditoria
- Sessões seguras
- Configuração segura do Django

Vulnerabilidades deverão ser reportadas conforme orientações do arquivo SECURITY.md.

---

# Qualidade

Antes de cada versão serão executadas validações automáticas.

Entre elas:

- Ruff
- Black
- isort
- pytest
- Coverage
- GitHub Actions

Nenhuma versão será publicada sem aprovação dessas etapas.

---

# Filosofia do Projeto

O ERP Drakkars não é apenas um software.

Ele também é um projeto educacional.

Nosso objetivo é mostrar como construir um ERP moderno utilizando apenas tecnologias Open Source e boas práticas de engenharia de software.

Todo código será acompanhado de documentação detalhada.

Toda decisão arquitetural será documentada.

Toda funcionalidade será testada.

---

# Roadmap

## Sprint 0

- Fundação do projeto
- Documentação inicial
- Estrutura do repositório
- Configuração do ambiente

## Sprint 1

- Projeto Django
- PostgreSQL
- Configurações iniciais
- Gunicorn
- Nginx

## Sprint 2

- Login
- Usuários
- Permissões
- Dashboard

## Sprint 3

- Cadastro de Clientes
- Cadastro de Produtos
- Categorias

## Sprint 4

- Estoque
- Compras
- Vendas

## Sprint 5

- Financeiro

## Sprint 6

- Relatórios

## Sprint 7

- API REST

## Sprint 8

- Deploy
- Backup
- Monitoramento
- Documentação Final

---

# Comunidade

O desenvolvimento acontecerá de forma aberta.

Sugestões, correções e melhorias são bem-vindas.

Utilize o GitHub para:

- Reportar problemas
- Solicitar funcionalidades
- Enviar Pull Requests
- Participar das discussões

---

# Licença

Este projeto é distribuído sob a licença MIT.

Consulte o arquivo LICENSE para mais informações.

---

# Agradecimentos

Agradecemos a todos que contribuírem para este projeto.

Cada sugestão, correção ou melhoria ajudará a tornar o ERP Drakkars uma plataforma cada vez melhor.

---

# Desenvolvido por

**Drakkars Consultoria**

Especialistas em:

- Arquitetura de Software
- Cloud Computing
- DevOps
- FinOps
- Inteligência Artificial
- Modernização de Aplicações
- Infraestrutura
- Segurança
- Open Source

---

# Aviso

Este projeto encontra-se em desenvolvimento ativo.

Novas funcionalidades serão adicionadas continuamente.

A documentação será atualizada a cada nova versão.

---

## Primeira Release

Versão:

0.1.0-alpha

Status:

🚧 Em desenvolvimento

---

**ERP Drakkars Community**

Construindo um ERP moderno, escalável e totalmente Open Source.
