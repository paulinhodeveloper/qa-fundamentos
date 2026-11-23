# QA Fundamentos: Sauce Demo

Aplicação prática das técnicas de teste do syllabus CTFL 4.0 em um e-commerce de demonstração, o [Sauce Demo](https://www.saucedemo.com). O objetivo é mostrar o trabalho de QA que vem **antes** da automação: entender o sistema, planejar, desenhar casos com técnicas formais e reportar defeitos com clareza.

## Escopo

| Funcionalidade | Coberta |
| --- | --- |
| Login e bloqueio de usuário | Sim |
| Catálogo e ordenação de produtos | Sim |
| Carrinho | Sim |
| Checkout (dados, resumo e finalização) | Sim |
| Menu lateral e logout | Sim |

## Entregáveis

| Documento | Conteúdo | Status |
| --- | --- | --- |
| [Plano de teste](01-plano-de-teste.md) | Objetivo, escopo, abordagem, riscos e critérios | Em andamento |
| [Casos de teste](02-casos-de-teste.md) | Casos com pré-condição, passos, dados e resultado esperado | A fazer |
| [Técnicas aplicadas](03-tecnicas-aplicadas.md) | Partição de equivalência, valor limite, tabela de decisão e transição de estados | A fazer |
| [Bug reports](04-bug-reports.md) | Defeitos encontrados, com severidade, prioridade e evidência | A fazer |

## Usuários de teste

O Sauce Demo disponibiliza usuários públicos com comportamentos diferentes, usados aqui como massa de dados:

| Usuário | Comportamento |
| --- | --- |
| `standard_user` | Fluxo normal |
| `locked_out_user` | Bloqueado no login |
| `problem_user` | Interface com defeitos propositais |
| `performance_glitch_user` | Respostas lentas |
| `error_user` | Erros em ações específicas |
| `visual_user` | Diferenças visuais |

A senha de todos é a mesma, exibida na própria página de login.

## Próximos passos

Os casos de maior prioridade deste projeto serão automatizados com Playwright e TypeScript em um repositório próprio.
