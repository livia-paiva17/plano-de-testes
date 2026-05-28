# Plano de Testes - Health Way

---

# 1. Identificação do Documento

- Título: Plano de Testes - Health Way
- Versão: 1.0
- Autor: Kauany Silva, Livia Paiva, Maria Julia Costa e Yasmin Salgado
- Data de criação: 15/05/2026
- Última revisão: 15/05/2026
- Status:
- Histórico de Revisões:

---

# 2. Introdução

## 2.1 Resumo do Projeto

O Health Way é um sistema web desenvolvido para auxiliar usuários no gerenciamento de vacinas, consultas , medicamentos e cuidados com os pets.
Desenvolvimento em React (frontend) + Node.js (backend) + PostgreSQL. 

## 2.2 Objetivo do Plano de Testes

Este documento define a estratégia, escopo, cronograma e critérios de testes do sistema Heath Way versão 1.0. Abrange os níveis de teste de integração,
sistema e aceitação.

## 2.3 Público-alvo

- Desenvolvedores
- Equipe QA
- Professor

---

# 3. Escopo

## 3.1 O que será testado (In Scope)

- Cadastro de usuários
- Login
- Agendamento de vacinas
- Consulta de vacinas
- Cadastro de medicamentos
- Consulta de hospitas próximos
- Consulta de agendamentos
- Responsividade mobile

## 3.2 O que NÃO será testado (Out of Scope)

- APIs externas do governo
- Compatibilidade com navegadores antigos
- Infraestrutura do servidor

---

# 4. Estratégia de Teste

## 4.1 Níveis de teste

- Teste funcional
- Teste de integração
- Teste E2E

## 4.2 Ferramentas

- GitHub
- Cypress
- Google Chrome

---

# 5. Critérios

## 5.1 Critérios de entrada

- Sistema funcionando
- Banco de dados conectado

## 5.2 Critérios de saída

- Todos os testes executados
- Nenhum bug crítico aberto

---

# 6. Entregáveis

- Plano de testes
- Relatório de bugs
- Casos de teste

---

# 7. Ambiente de Teste

- Windows 11
- Google Chrome
- Celular Android

---

# 8. Riscos e Contingências

## Riscos

- Sistema offline
- Falha no login
- Lentidão
- Ambiente de staging instável
- Flakiness em testes automatizados
- Mudança de requisitos durante a execução dos testes 


## Contingências

- Refazer testes
- Corrigir bugs encontrados

---

# 9. Cronograma

| Etapa | Data |
|---|---|
| Planejamento | 15/05 |
| Testes de login | 16/05 |
| Testes de agendamento | 17/05 |
| Testes Pagina pets | 18/05 |
| Correções | 19/05 |

---

# 10. Recursos e Papéis

| Desenvolvedora Front-end | Livia |
| Desenvolvedora Back-end | Kauany |
| Designer UI/UX | Maria Julia |
| Designer UI/UX | Yasmin |
| Testadora | Equipe |

---

# 11. Aprovações

| Equipe | Kauany Silva, Livia Paiva, Maria Julia Costa e Yasmin Salgado |
| Equipe | QA |
| Marco Antônio | Avaliador |

---

# 12. Glossário

- Bug: erro no sistema
- Login: acesso ao sistema
- E2E: teste ponta a ponta
