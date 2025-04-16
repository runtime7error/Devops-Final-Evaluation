# 🚀 Projeto com CI/CD no GitHub Actions

Este é um projeto simples em HTML, CSS e JavaScript com um pipeline de **CI/CD automatizado** usando **GitHub Actions**. Ideal para testes, estudos ou demonstrações de DevOps moderno com **deploy automático no GitHub Pages**!

---

## 📂 Estrutura do Projeto

```
.
├── index.html
├── style.css
├── script.js
└── .github/
    └── workflows/
        └── main.yml
```

---

## ⚙️ Pipeline de CI/CD

Toda vez que você fizer um `push` ou abrir um `pull request` na branch `main`, o GitHub Actions executa **três etapas automáticas**:

### ✅ 1️⃣ Verificar arquivos no repositório

📋 Lista todos os arquivos presentes, ajudando a validar o conteúdo e verificar o que está sendo enviado para o repositório.

```bash
ls -la
```

---

### 🔍 2️⃣ Lint no JavaScript com ESLint

🧹 Instala e executa o ESLint para identificar erros ou problemas de estilo no arquivo `script.js`.  
Mesmo que tenha erro, o CI não falha (usamos `|| true`).

---

### 🚀 3️⃣ Publicar no GitHub Pages

📦 Gera uma versão "buildada" da aplicação (nesse caso, com os arquivos normais)  
🌐 Faz o deploy automático no **GitHub Pages**, acessível diretamente pelo navegador.

---

## 🔄 Quando o pipeline é executado?

Este pipeline é disparado automaticamente:

- quando você **faz push na branch `main`** 🟢  
- quando você **abre um pull request para `main`** 🔁  
- ou manualmente via **Actions → Run workflow** ⚙️

---

## 🌍 Acessar a aplicação

Após o deploy, acesse a aplicação pela URL gerada pelo GitHub Pages:  
🔗 `https://runtime7error.github.io/Devops-Final-Evaluation/`

---

## 🛠 Pré-requisitos para o Deploy funcionar

1. A branch `main` precisa conter o workflow `.github/workflows/main.yml`
2. Ativar GitHub Pages:
   - Vá em **Settings > Pages**
   - Em **Build and deployment**, selecione **GitHub Actions**
3. Commitar qualquer mudança e observar o CI rodando automaticamente 🎉

---

## 📘 Dica Extra

Quer testar sua própria build ou projeto? Edite os arquivos HTML/CSS/JS e veja o deploy acontecer em tempo real com cada push 😄

---

Powered By BigFriend ™