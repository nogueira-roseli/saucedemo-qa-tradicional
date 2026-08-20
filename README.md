# saucedemo-qa-tradicional

Projeto de testes manuais realizados na aplicação SauceDemo, contemplando desde o planejamento dos testes até a execução, registro de defeitos rastreabilidade e relatório final.

## Sobre o projeto

O projeto tem como objetivo demonstrar a aplicação prática de técnicas e processos de QA Manual, utilizando a aplicação SauceDemo como sistema sob teste.

Foram realizadas atividades de planejamento, análise funcional, definição de cenários e casos de teste, execução dos testes, registro de defeitos, rastreabilidade dos requisitos e elaboração do relatório final.

## Ferramentas e tecnologias

- GitHub — versionamento e documentação do projeto
- SauceDemo — aplicação utilizada como sistema sob teste
- Microsoft Word — elaboração da documentação
- PDF — formato final dos documentos

## Documentação

A documentação completa do projeto está disponível na pasta [`documentos`](./documentos/).

Os documentos incluem:

1. Plano de Teste
2. Análise Funcional do Sistema
3. Cenários de Teste
4. Casos de Teste
5. Execução dos Casos de Teste
6. RTM — Matriz de Rastreabilidade
7. Relatório de Erros
8. Relatório Final de Testes

## Escopo dos testes

Os testes foram direcionados às principais funcionalidades da aplicação SauceDemo, considerando os fluxos de:

- Autenticação de usuários
- Navegação e catálogo de produtos
- Ordenação de produtos
- Adição e remoção de produtos do carrinho
- Processo de checkout
- Validação das informações do pedido
- Finalização da compra
- Logout

Os testes contemplaram cenários positivos e negativos, com registro dos resultados obtidos durante a execução.

## Resultado da execução

Foram planejados e executados 15 casos de teste.

| Resultado | Quantidade |
|---|---:|
| Passou | 13 |
| Falhou | 1 |
| Bloqueado | 1 |
| **Total** | **15** |

Durante a execução foi identificado 1 defeito crítico relacionado ao fluxo de checkout, registrado no BUG-001.

## Defeito encontrado

### BUG-001 — Tela branca durante o checkout

Durante a execução do fluxo de checkout, a aplicação apresentou uma tela branca, interrompendo a continuidade do processo e impedindo a finalização da compra.

- **Severidade:** Crítica
- **Prioridade:** Alta
- **Status:** Novo
- **Impacto:** Impede a conclusão da compra
- **Frequência:** 100%
- **Caso relacionado:** CT-014
- **Caso bloqueado em consequência:** CT-015

O defeito foi documentado no [BUG Report](./documentos/07-BUG%20Report%20-%20SauceDemo.pdf).

Como o defeito impede a conclusão do fluxo principal de compra, a recomendação final foi **não liberar a aplicação para produção até que o problema seja corrigido e validado por novos testes**.

## Conclusão

A execução dos testes permitiu validar a maior parte das funcionalidades previstas no escopo. Entretanto, o defeito crítico identificado no fluxo de checkout interrompe a jornada principal de compra.

Dessa forma, a aplicação foi considerada **não recomendada para liberação em produção** até que o BUG-001 seja corrigido e submetido a novos testes de validação e regressão.

## Estrutura do projeto

```text
saucedemo-qa-traditional/
│
├── documentos/
│   ├── 01-Plano de Teste - SauceDemo.pdf
│   ├── 02-Análise Funcional do Sistema - SauceDemo.pdf
│   ├── 03-Cenários de Teste - SauceDemo.pdf
│   ├── 04-Casos de Teste - SauceDemo.pdf
│   ├── 05-Execução dos Casos de Teste - SauceDemo.pdf
│   ├── 06-RTM - SauceDemo.pdf
│   ├── 07-BUG Report - SauceDemo.pdf
│   └── 08-Relatório Final de Testes - SauceDemo.pdf
│
└── README.md
