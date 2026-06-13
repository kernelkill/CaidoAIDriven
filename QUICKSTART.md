# Quickstart — Pentest AI Lab

> Este guia cobre os primeiros passos para explorar o ambiente.
> O guia completo de instalação (15 capítulos, Ubuntu 24.04 validado) está disponível sob solicitação — veja o [README](README.md).

---

## Antes de começar — contas obrigatórias

Sem essas duas contas, nada funciona:

| Serviço | Plano | Link |
|---|---|---|
| **Claude.ai** | **Pro ou Team (pago)** | https://claude.ai |
| **Caido** | Free tier | https://caido.io |

> ⚠️ O plano Free do Claude.ai **não funciona** com Claude Code. Verifique sua assinatura antes de continuar.

---

## Passo 1 — Pré-requisitos (Ubuntu 24.04)

```bash
# Atualizar o sistema
sudo apt-get update && sudo apt-get upgrade -y

# Dependências
sudo apt-get install -y git golang-go libfuse2

# Node.js 20+ via NodeSource
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -
sudo apt-get install -y nodejs

# Verificar
node --version   # esperado: v20.x.x
go version       # esperado: go1.20+
git --version
```

---

## Passo 2 — Claude Code

```bash
npm install -g @anthropic-ai/claude-code
claude --version   # esperado: 2.x.x (Claude Code)

# Autenticar (abre browser na primeira vez)
claude
```

> ✅ Após a autenticação, você verá a tela de boas-vindas com seu nome.

---

## Passo 3 — Criar pasta de trabalho

```bash
mkdir -p ~/Documentos
```

---

## Próximos passos

A partir daqui, o guia completo cobre:

- Instalação e configuração do Caido Proxy (AppImage, certificado CA, browser como proxy)
- Instalação das 792 skills (defensivas + ofensivas)
- Instalação dos 35 subagentes com doctor.sh e ferramentas Tier 2
- Configuração do CLAUDE.md global
- Instalação e autenticação do Caido MCP Server v4.0 (64 tools)
- findings.sh com múltiplos clientes e persistência entre sessões
- Checklist de inicialização para uso diário
- Prompts validados para cada tipo de engajamento
- Atualização do MCP Server sem quebrar o ambiente
- Troubleshooting com erros reais

**Para receber o guia completo:**

- 💼 [LinkedIn — Joabe Kachorroski](https://www.linkedin.com/in/joabekachorroski)
- 🐛 Abra uma [Issue](../../issues/new?title=Solicitar+guia+de+instalação&body=Olá!+Gostaria+de+receber+o+guia+completo+de+instalação+do+Pentest+AI+Lab.) com o título **"Solicitar guia"**

---

> ⚠️ Use apenas em ambientes autorizados — pentest contratado, bug bounty em programas válidos, CTFs e laboratórios próprios.
