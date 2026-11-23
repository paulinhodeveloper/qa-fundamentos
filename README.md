<h1 align="center">🧪 QA Fundamentos: Sauce Demo</h1>

<p align="center">
  <img alt="CTFL 4.0" src="https://img.shields.io/badge/ISTQB-CTFL%204.0-1F3A5F?style=for-the-badge">
  <img alt="Status" src="https://img.shields.io/badge/status-em%20andamento-F2B705?style=for-the-badge">
  <img alt="Markdown" src="https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white">
  <a href="https://www.saucedemo.com"><img alt="Sauce Demo" src="https://img.shields.io/badge/alvo-Sauce%20Demo-E2231A?style=for-the-badge&logo=saucelabs&logoColor=white"></a>
</p>

<p align="center">
  Aplicação prática das técnicas de teste do syllabus <strong>CTFL 4.0</strong> em um e-commerce de demonstração.<br>
  O trabalho de QA que vem <strong>antes</strong> da automação: entender o sistema, planejar, desenhar casos com técnicas formais e reportar defeitos com clareza.
</p>

---

## 🎯 Escopo

| Funcionalidade | Coberta |
| --- | :---: |
| 🔐 Login e bloqueio de usuário | ✅ |
| 🛍️ Catálogo e ordenação de produtos | ✅ |
| 🛒 Carrinho | ✅ |
| 💳 Checkout (dados, resumo e finalização) | ✅ |
| ☰ Menu lateral e logout | ✅ |

## 📦 Entregáveis

| Documento | Conteúdo | Status |
| --- | --- | :---: |
| 📋 [Plano de teste](01-plano-de-teste.md) | Objetivo, escopo, abordagem, riscos e critérios | ![Em andamento](https://img.shields.io/badge/-em%20andamento-F2B705) |
| 🧾 [Casos de teste](02-casos-de-teste.md) | Casos com pré-condição, passos, dados e resultado esperado | ![A fazer](https://img.shields.io/badge/-a%20fazer-9AA5B1) |
| 🧠 [Técnicas aplicadas](03-tecnicas-aplicadas.md) | Partição de equivalência, valor limite, tabela de decisão e transição de estados | ![A fazer](https://img.shields.io/badge/-a%20fazer-9AA5B1) |
| 🐞 [Bug reports](04-bug-reports.md) | Defeitos encontrados, com severidade, prioridade e evidência | ![A fazer](https://img.shields.io/badge/-a%20fazer-9AA5B1) |

## 👤 Usuários de teste

O Sauce Demo disponibiliza usuários públicos com comportamentos diferentes, usados aqui como massa de dados:

| Usuário | Comportamento |
| --- | --- |
| `standard_user` | Fluxo normal |
| `locked_out_user` | Bloqueado no login |
| `problem_user` | Interface com defeitos propositais |
| `performance_glitch_user` | Respostas lentas |
| `error_user` | Erros em ações específicas |
| `visual_user` | Diferenças visuais |

> A senha de todos é a mesma, exibida na própria página de login.

## 🧰 Técnicas e conceitos

![Partição de equivalência](https://img.shields.io/badge/Partição%20de%20equivalência-2E86AB)
![Valor limite](https://img.shields.io/badge/Valor%20limite-2E86AB)
![Tabela de decisão](https://img.shields.io/badge/Tabela%20de%20decisão-2E86AB)
![Transição de estados](https://img.shields.io/badge/Transição%20de%20estados-2E86AB)
![Teste exploratório](https://img.shields.io/badge/Teste%20exploratório-2E86AB)
![Teste baseado em risco](https://img.shields.io/badge/Teste%20baseado%20em%20risco-2E86AB)

## 🚀 Próximos passos

Os casos de maior prioridade deste projeto serão automatizados com Playwright e TypeScript em um repositório próprio.

---

<p align="center">
  Feito por <a href="https://paulinhodeveloper.github.io">Paulo Henrique Santos Borges</a> ·
  <a href="https://www.linkedin.com/in/paulinhoborges">LinkedIn</a>
</p>
