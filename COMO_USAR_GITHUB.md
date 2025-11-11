# 📚 Como Enviar o Projeto para o GitHub

## Opção 1: Usando a Interface Web do GitHub (Mais Fácil)

### Passo 1: Criar Repositório no GitHub
1. Acesse https://github.com
2. Faça login na sua conta
3. Clique no botão **"+"** no canto superior direito
4. Selecione **"New repository"**
5. Preencha:
   - **Repository name**: `loja-do-tchulica`
   - **Description**: "E-commerce de smartphones e acessórios - Projeto Faculdade"
   - Deixe **Public** (ou Private se preferir)
   - ✅ Marque **"Add a README file"**
6. Clique em **"Create repository"**

### Passo 2: Fazer Upload dos Arquivos
1. No seu repositório criado, clique em **"Add file"** → **"Upload files"**
2. Arraste todos os arquivos e pastas do projeto (exceto `node_modules` e `dist`)
3. Adicione uma mensagem de commit: "Commit inicial - Loja do Tchulica"
4. Clique em **"Commit changes"**

**Pronto!** Seu projeto está no GitHub! 🎉

---

## Opção 2: Usando Git pela Linha de Comando (Avançado)

### Pré-requisitos
- Git instalado no seu computador
- Download do arquivo ZIP e descompactado

### Comandos

```bash
# 1. Navegue até a pasta do projeto
cd loja-do-tchulica

# 2. Inicialize o repositório Git
git init

# 3. Adicione todos os arquivos
git add .

# 4. Faça o primeiro commit
git commit -m "Commit inicial - Loja do Tchulica"

# 5. Adicione o repositório remoto (substitua SEU_USUARIO pelo seu usuário do GitHub)
git remote add origin https://github.com/SEU_USUARIO/loja-do-tchulica.git

# 6. Envie para o GitHub
git branch -M main
git push -u origin main
```

---

## 📝 Atualizando o Projeto no Futuro

### Pela Interface Web
1. Vá até o repositório
2. Clique em **"Add file"** → **"Upload files"**
3. Selecione os arquivos modificados
4. Commit as mudanças

### Por Linha de Comando
```bash
# Adicionar arquivos modificados
git add .

# Fazer commit com mensagem descritiva
git commit -m "Descrição da alteração"

# Enviar para o GitHub
git push
```

---

## 🔧 Configuração Inicial do Git (Primeira vez)

Se for a primeira vez usando Git, configure seu nome e email:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu.email@exemplo.com"
```

---

## 📋 Estrutura de Commits Recomendada

Exemplos de mensagens de commit:

- `feat: adicionar página de checkout`
- `fix: corrigir bug no carrinho de compras`
- `style: melhorar design do header`
- `docs: atualizar README com instruções`
- `refactor: reorganizar componentes`

---

## 🌐 Compartilhar o Projeto

Depois de fazer upload, compartilhe o link:
```
https://github.com/SEU_USUARIO/loja-do-tchulica
```

---

## 🚀 Dicas Extras

### Deploy Gratuito (Hospedar o Site)

Você pode colocar o site no ar gratuitamente usando:

#### **Vercel** (Recomendado)
1. Acesse https://vercel.com
2. Conecte sua conta do GitHub
3. Selecione o repositório `loja-do-tchulica`
4. Clique em **Deploy**
5. Pronto! Seu site estará online em minutos

#### **Netlify**
1. Acesse https://netlify.com
2. Arraste a pasta `dist` (depois de fazer `npm run build`)
3. Site publicado instantaneamente

#### **GitHub Pages**
```bash
# Instalar gh-pages
npm install --save-dev gh-pages

# Adicionar no package.json em "scripts":
"predeploy": "npm run build",
"deploy": "gh-pages -d dist"

# Publicar
npm run deploy
```

O site ficará disponível em:
```
https://SEU_USUARIO.github.io/loja-do-tchulica
```

---

## ❓ Problemas Comuns

### "Permission denied" ao fazer push
- Certifique-se de estar logado no Git
- Configure um token de acesso pessoal no GitHub
- Ou use SSH keys

### Arquivos muito grandes
- Certifique-se de que `node_modules` e `dist` estão no `.gitignore`
- Nunca faça commit dessas pastas

### Conflict ao fazer push
```bash
git pull origin main --rebase
# Resolve conflitos se houver
git push origin main
```

---

## 📞 Precisa de Ajuda?

- Documentação Git: https://git-scm.com/doc
- GitHub Guides: https://guides.github.com
- YouTube: Procure por "Git e GitHub para iniciantes"

---

**Boa sorte com seu projeto! 🚀**
