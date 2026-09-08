# Setup Netlify — Portal Executivo SN Company

## 1️⃣ Preparar repositório Git local

```bash
cd ~/seu-projeto/portal-sn-company
git init
git add .
git commit -m "Portal Executivo SN Company - Deploy inicial"
```

## 2️⃣ Subir para GitHub/GitLab

```bash
git remote add origin https://github.com/seu-usuario/portal-sn-company.git
git branch -M main
git push -u origin main
```

## 3️⃣ Conectar Netlify

1. Acesse **https://netlify.com**
2. Clique **"New site from Git"**
3. Selecione **GitHub/GitLab**
4. Escolha repositório `portal-sn-company`
5. Clique **"Deploy"**

✅ Site publicado automaticamente!

## 4️⃣ Atualizações diárias

**Opção A: Editar via Git (recomendado)**
```bash
# Editar dados em data.json ou HTML
git add .
git commit -m "Atualizar dados financeiros - Set/08"
git push
# Netlify faz deploy automaticamente em ~2 min
```

**Opção B: Editar via Netlify UI**
1. Acesse dashboard Netlify
2. Clique em "File browser"
3. Edite `data.json` ou `index.html`
4. Salve → Deploy automático

## 📊 Estrutura

```
portal-sn-company/
├── index.html           # Portal completo (auto-contido)
├── data.json           # Dados financeiros (JSON)
├── netlify.toml        # Config Netlify
├── README.md           # Este arquivo
├── SETUP.md            # Instruções setup
└── .gitignore
```

## 🔗 URLs

- **Preview**: https://seu-site.netlify.app
- **Production**: seu-dominio-customizado.com (opcional)
- **Admin**: https://app.netlify.com/sites/seu-site/overview

