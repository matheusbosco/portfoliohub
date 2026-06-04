# Política de Segurança — PortfolioHUB

A segurança deste repositório é levada a sério, mesmo sendo um projeto acadêmico e pessoal. Este documento descreve as práticas adotadas e como relatar uma vulnerabilidade.

## Versões suportadas

| Versão | Suportada |
|--------|-----------|
| 1.x (branch `master`) | ✅ |
| Versões anteriores | ❌ |

## Como relatar uma vulnerabilidade

Encontrou um problema de segurança? **Não abra uma issue pública.**

1. Acesse a aba **Security** do repositório → **Report a vulnerability** (GitHub Private Vulnerability Reporting); ou
2. Entre em contato pelo LinkedIn: <https://linkedin.com/in/matheusbosco>

Você receberá uma resposta em até **5 dias úteis**. Após a confirmação, a correção será priorizada e você será informado sobre o andamento.

## Práticas de segurança adotadas

Este repositório implementa as seguintes medidas, alinhadas às boas práticas do GitHub:

- **Autenticação em duas etapas (2FA)** habilitada na conta do mantenedor.
- **Branch protection** na branch `master`: exige Pull Request com revisão, impede push direto e *force-push*.
- **CODEOWNERS**: alterações exigem revisão do responsável definido.
- **Secret scanning** e **push protection** ativados para impedir o vazamento de segredos (tokens, chaves).
- **Dependabot** monitorando as versões das GitHub Actions usadas no CI.
- **Integração contínua (CI)** validando o HTML e os links a cada Pull Request.
- **Princípio do menor privilégio**: permissões mínimas (`contents: read`) nos workflows.

## Boas práticas para colaboradores

- Nunca faça commit de segredos (senhas, tokens, chaves de API). Use variáveis de ambiente ou *GitHub Secrets*.
- Mantenha as dependências e Actions atualizadas (acompanhe os PRs do Dependabot).
- Revise o código antes de aprovar qualquer Pull Request.

---
*Documento mantido por Matheus Bosco — última revisão: junho/2026.*
