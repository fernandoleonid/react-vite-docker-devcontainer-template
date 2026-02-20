# React + Docker + Dev Container Template

## Sobre este repositório

Este repositório é um template para desenvolvimento de aplicações React utilizando Docker e Dev Container. O objetivo é fornecer um ambiente de desenvolvimento padronizado, isolado e pronto para uso, eliminando problemas de incompatibilidade entre versões do Node e dependências instaladas localmente.

Com este template qualquer desenvolvedor precisa apenas ter o **WSL** e o **Docker** instalados para começar a trabalhar, sem necessidade de instalar o Node.js ou qualquer outra dependência diretamente na máquina.

> **Autor:** Prof. Fernando Leonid

---

## Pré-requisitos

- WSL instalado
- Docker instalado e funcionando
- VSCode com a extensão **Dev Containers** (ms-vscode-remote.remote-containers)

---

## Passo a passo

### 1. Usar este template

Clique em **"Use this template"** no GitHub e clone o repositório criado:

```bash
git clone https://github.com/seu-usuario/seu-repo.git
cd seu-repo
```

### 2. Criar o projeto Vite

```bash
npm create vite@latest meu-app -- --template react
cd meu-app
```

### 3. Copiar os arquivos do template

Mova ou copie os arquivos `Dockerfile`, `docker-compose.yml` e a pasta `.devcontainer` para dentro da pasta do projeto criada pelo Vite.

### 4. Subir o container

```bash
docker-compose up --build -d
```

### 5. Abrir no Dev Container

`Ctrl+Shift+P` → **Reopen in Container**

---

✅ Acessa em **http://localhost:5173**

A partir daqui tudo pelo terminal do VSCode!

---

## Comandos úteis

| Comando | Descrição |
|---|---|
| `docker-compose up -d` | Sobe o container em background |
| `docker-compose up --build -d` | Rebuilda e sobe o container |
| `docker-compose down` | Para e remove o container |
| `npm install pacote` | Instala uma dependência dentro do container |

---

## Estrutura do repositório

```
.
├── Dockerfile
├── docker-compose.yml
├── .devcontainer/
│   └── devcontainer.json
└── README.md
```
# react-vite-docker-devcontainer-template
