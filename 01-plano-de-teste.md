# Plano de teste

## 1. Objetivo

Verificar se o fluxo de compra do Sauce Demo (login, catálogo, carrinho e checkout) funciona conforme o esperado para diferentes perfis de usuário, identificando defeitos que impeçam ou prejudiquem a compra.

## 2. Escopo

### Dentro do escopo

- Login, incluindo mensagens de erro e bloqueio de usuário
- Listagem e ordenação de produtos
- Adicionar e remover produtos do carrinho
- Checkout: dados do cliente, resumo e finalização
- Menu lateral e logout

### Fora do escopo

- Testes em celular e tablet
- Testes de carga e performance com ferramentas, pois não há ambiente próprio
- Pagamento real, pois o site é uma demonstração
- Acessibilidade, prevista para uma próxima fase

## 3. Abordagem

| Nível | Tipo | Técnica | Execução |
| --- | --- | --- | --- |
| Sistema | Funcional | Partição de equivalência e valor limite nos campos | Manual |
| Sistema | Funcional | Transição de estados no fluxo de compra | Manual |
| Sistema | Negativo | Tentativas de acesso não permitidas | Manual |
| Sistema | Exploratório | Sessões de 30 minutos com charter | Manual |
| Sistema | Regressão | Casos de maior prioridade | Automatizado depois, com Playwright |

## 4. Ambiente e dados

- **Ambiente:** https://www.saucedemo.com, navegador Brave (motor Chromium), versão atual, em computador
- **Massa de dados:** usuários públicos do Sauce Demo:
  - `standard_user`: fluxo normal
  - `locked_out_user`: teste negativo, o acesso deve ser bloqueado
  - `problem_user`: defeitos funcionais
  - `performance_glitch_user`: lentidão
  - `visual_user`: defeitos visuais

## 5. Riscos

| Risco | Probabilidade | Impacto | Prioridade | Mitigação |
| --- | --- | --- | --- | --- |
| Usuário bloqueado conseguir acessar a loja | Baixa | Alto | Alta | Testar o login com `locked_out_user` e validar a mensagem de bloqueio |
| Cliente não conseguir finalizar a compra | Média | Alto | Alta | Testar o checkout com todos os usuários e com campos vazios ou inválidos |
| Carrinho exibir quantidade ou preço errado | Média | Alto | Alta | Conferir quantidade e total em cada etapa da compra |
| Ordenação de produtos não funcionar | Média | Médio | Média | Testar todas as opções de ordenação com cada usuário |

## 6. Critérios de entrada

- Site disponível e acessível
- Usuários de teste funcionando
- Plano de teste revisado

## 7. Critérios de saída

- Todos os casos de teste de prioridade alta executados
- Todos os defeitos encontrados registrados em bug reports
- Nenhum defeito crítico sem registro

## 8. Entregáveis

- Plano de teste (este documento)
- [Casos de teste](02-casos-de-teste.md)
- [Técnicas aplicadas](03-tecnicas-aplicadas.md)
- [Bug reports](04-bug-reports.md)
