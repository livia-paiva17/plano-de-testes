Plano de Testes - Health Way



1. Identificação do Documento

# Título: Plano de Testes – Health Way
# Versão:  2.0
# Autores: Kauany Silva, Livia Paiva, Maria Julia Costa e Yasmin Salgado
# Data de criação: 15/05/2026
# Última revisão: 26/06/2026
# Status: Em revisão
# Histórico de Revisões:

| Versão | Data       | Descrição                                |
| ------ | ---------- | ---------------------------------------- |
| 1.0    | 15/05/2026 | Criação do documento                     |
| 2.0    | 26/06/2026 | Ajustes conforme devolutiva do professor |



2. Introdução

 2.1 Resumo do Projeto

O Health Way é um sistema web desenvolvido para auxiliar usuários no gerenciamento de vacinas, consultas, medicamentos e cuidados com pets. O sistema foi desenvolvido utilizando React no frontend, Node.js no backend e PostgreSQL como banco de dados.

 2.2 Objetivo do Plano de Testes

Este documento define a estratégia, escopo, ambiente, critérios, cronograma e responsabilidades da execução dos testes da versão 1.0 do sistema Health Way, garantindo a qualidade das funcionalidades implementadas.

 2.3 Público-alvo

* Desenvolvedores
* Equipe de Testes
* Professor Avaliador



 3. Escopo

 3.1 Funcionalidades que serão testadas

| Funcionalidade                 | Prioridade |
| ------------------------------ | ---------- |
| Cadastro de usuários           | Alta       |
| Login                          | Alta       |
| Agendamento de vacinas         | Alta       |
| Consulta de vacinas            | Média      |
| Cadastro de medicamentos       | Média      |
| Consulta de hospitais próximos | Média      |
| Consulta de agendamentos       | Alta       |
| Responsividade mobile          | Baixa      |

 3.2 Fora do Escopo

* APIs externas do governo
* Compatibilidade com navegadores antigos
* Infraestrutura do servidor
* Testes em ambiente de produção



 4. Estratégia de Testes

 4.1 Níveis de Teste

| Nível                   | Objetivo                                                         | Escopo                                                     | Ferramenta |
| ----------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------- | ---------- |
| Testes Funcionais       | Validar se cada funcionalidade atende aos requisitos             | Cadastro, login, medicamentos, consultas, vacinas e pets   | Cypress    |
| Testes de Integração    | Verificar a comunicação entre frontend, backend e banco de dados | APIs, autenticação, gravação e consulta no PostgreSQL      | Cypress    |
| Testes End-to-End (E2E) | Simular o uso completo do sistema pelo usuário                   | Fluxo completo de cadastro, login, agendamento e consultas | Cypress    |

 4.2 Testes Não Funcionais

| Tipo        | Objetivo                                                                                         |
| ----------- | ------------------------------------------------------------------------------------------------ |
| Performance | Verificar tempo de carregamento das páginas principais e resposta das APIs.                      |
| Segurança   | Validar autenticação, autorização e tratamento de entradas inválidas (ex.: SQL Injection e XSS). |
| Usabilidade | Avaliar facilidade de navegação, organização das telas e responsividade em dispositivos móveis.  |



 5. Critérios

 5.1 Critérios de Entrada

* Sistema compilando sem erros.
* Banco de dados disponível.
* Ambiente de testes configurado.
* Casos de teste elaborados.

 5.2 Critérios de Saída

* 95% dos casos de teste executados.
* Pelo menos 90% dos testes aprovados.
* Nenhum bug crítico ou alto em aberto.
* Relatório de testes concluído.

 5.3 Critérios de Aprovação dos Testes

Um teste será considerado:

* **Aprovado:** resultado obtido corresponde ao esperado.
* **Falho:** resultado diferente do esperado.
* **Bloqueado:** não foi possível executar devido a problemas externos.

 5.4 Classificação da Severidade dos Bugs

| Severidade | Descrição                                                            |
| ---------- | -------------------------------------------------------------------- |
| Crítica    | Impede o uso do sistema ou causa perda de dados.                     |
| Alta       | Afeta funcionalidades principais, mas existe alternativa temporária. |
| Média      | Impacta funcionalidades secundárias sem impedir o uso.               |
| Baixa      | Problemas visuais ou pequenos erros de usabilidade.                  |

A classificação será realizada pela equipe de testes em conjunto com os desenvolvedores.



 6. Entregáveis

* Plano de Testes
* Casos de Teste
* Relatório de Execução
* Relatório de Bugs
* Evidências (prints e vídeos quando necessário)



 7. Ambiente de Testes

| Ambiente            | URL                                | Configuração    |
| ------------------- | ---------------------------------- | --------------- |
| Desenvolvimento     | https://healthway-gray.vercel.app/ | React + Node.js |
| Backend             | Hospedagem na máquina              | Node.js         |
| Banco de Dados      | PostgreSQL 16                      | Banco local     |
| Navegador           | Google Chrome 137 ou superior      | Cache limpo     |
| Sistema Operacional | Windows 11                         | Atualizado      |
| Mobile              | Android 13 ou superior             | Google Chrome   |



 8. Riscos e Contingências

 Riscos

* Sistema indisponível.
* Banco de dados offline.
* Lentidão do sistema.
* Falhas de integração.
* Mudanças de requisitos.
* Instabilidade do ambiente de testes.

 Contingências

* Reexecução dos testes.
* Correção dos bugs encontrados.
* Atualização dos casos de teste.
* Utilização de ambiente local caso o servidor esteja indisponível.



 9. Cronograma

| Atividade                        | Data  |
| -------------------------------- | ----- |
| Planejamento                     | 10/05 |
| Elaboração dos casos de teste    | 20/05 |
| Testes de Login e Cadastro       | 22/05 |
| Testes de Vacinas e Agendamentos | 22/05 |
| Testes da Página de Pets         | 27/05 |
| Correção dos Bugs                | 10/06 |
| Reexecução dos Testes            | 25/06 |
| Entrega Final                    | 10/10 |



 10. Recursos e Papéis

| Integrante  | Função                   | Responsabilidades                                   
| ----------- | ------------------------ | --------------------------------------------------- | 
| Kauany      | Desenvolvedora Back-end  | Correção de APIs e apoio aos testes de integração   | 
| Livia       | Desenvolvedora Front-end | Correção de interface e apoio aos testes funcionais | 
| Maria Julia | UI/UX e Testes Manuais   | Execução dos testes funcionais e registro de bugs   | 
| Yasmin      | Líder de Testes          | Planejamento, validação dos resultados e testes E2E |



 11. Aprovações

| Nome              | Cargo               | Data | Status   |
| ----------------- | ------------------- | ---- | -------- |
| Kauany Silva      | Desenvolvedora      | ____ | Pendente |
| Livia Paiva       | Desenvolvedora      | ____ | Pendente |
| Maria Julia Costa | UI/UX               | ____ | Pendente |
| Yasmin Salgado    | Líder de Testes     | ____ | Pendente |
| Marco Antônio     | Professor Avaliador | ____ | Pendente |



 12. Glossário

| Termo              | Definição                                                                                |
| ------------------ | ---------------------------------------------------------------------------------------- |
| API                | Interface responsável pela comunicação entre frontend e backend.                         |
| Bug                | Defeito identificado durante os testes.                                                  |
| E2E                | Teste que simula o fluxo completo do usuário.                                            |
| Staging            | Ambiente de testes semelhante ao ambiente de produção.                                   |
| Mock               | Simulação de um serviço ou API utilizada durante os testes.                              |
| Regression Testing | Testes executados para garantir que alterações não quebraram funcionalidades existentes. |
| Pipeline CI/CD     | Processo automatizado de integração, testes e implantação do sistema.                    |
| PostgreSQL         | Sistema Gerenciador de Banco de Dados utilizado pelo projeto.                            |
