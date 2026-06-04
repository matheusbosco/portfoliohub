# Guia de Contribuição — PortfolioHUB

Obrigado pelo interesse em contribuir! Este guia descreve o fluxo de trabalho, os padrões de código e as práticas de colaboração do projeto.

## Sumário
- [Pré-requisitos](#pré-requisitos)
- [Como rodar localmente](#como-rodar-localmente)
- [Fluxo de trabalho (Git)](#fluxo-de-trabalho-git)
- [Padrão de commits](#padrão-de-commits)
- [Pull Requests](#pull-requests)
- [Revisão de código](#revisão-de-código)

## Pré-requisitos
- Conta no GitHub com **2FA** habilitado.
- Git instalado (`git --version`).
- Navegador moderno. Opcional: Node.js para servir o site localmente.

## Como rodar localmente
```bash
git clone https://github.com/matheusbosco/portfoliohub.git
cd portfoliohub/academico/portfoliohub

# abrir direto no navegador (Windows)
start index.html

# ou servir localmente
npx serve .
```

## Fluxo de trabalho (Git)
Usamos um fluxo simples baseado em *feature branches*:

1. Atualize a branch principal: `git pull origin master`
2. Crie uma branch para sua mudança: `git checkout -b feat/nome-curto`
3. Faça commits pequenos e descritivos.
4. Envie a branch: `git push -u origin feat/nome-curto`
5. Abra um **Pull Request** para `master`.

> A branch `master` é protegida: não é possível fazer push direto. Toda mudança entra por Pull Request revisado.

## Padrão de commits
Seguimos **Conventional Commits**:

| Tipo | Quando usar |
|------|-------------|
| `feat` | Nova funcionalidade |
| `fix` | Correção de bug |
| `docs` | Documentação |
| `style` | Formatação (sem mudar lógica) |
| `refactor` | Refatoração de código |
| `chore` | Tarefas de manutenção/configuração |
| `ci` | Mudanças de integração contínua |

Exemplo: `feat: adiciona seção de certificações no portfólio`

## Pull Requests
- Preencha o template de PR (carregado automaticamente).
- Vincule a issue relacionada (ex.: `Closes #12`).
- Garanta que o **CI** (validação de HTML e links) passou.
- Aguarde a revisão do CODEOWNER (@matheusbosco).

## Revisão de código
- PRs exigem pelo menos **1 aprovação**.
- Comentários devem ser resolvidos antes do merge.
- Prefira *squash merge* para manter o histórico limpo.

---
Dúvidas? Abra uma issue ou fale pelo [LinkedIn](https://linkedin.com/in/matheusbosco).
