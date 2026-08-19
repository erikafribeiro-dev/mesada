# Configurar Google Drive Sync Automático

## ⏱️ Tempo: 5 minutos

---

## PASSO 1: Criar Google Cloud Project

1. Acesse: https://console.cloud.google.com
2. No topo, clique em **"Selecionar um projeto"**
3. Clique **"Novo projeto"**
4. Nome: `Mesada do Leo`
5. Clique **"Criar"**
6. Aguarde carregar (1-2 min)

---

## PASSO 2: Ativar Google Drive API

1. Na barra de busca, procure: **"Google Drive API"**
2. Clique no resultado
3. Clique **"Ativar"**
4. Aguarde ativar

---

## PASSO 3: Configurar OAuth Consent Screen

1. No menu esquerdo, clique **"OAuth consent screen"**
2. Selecione **"Externo"** → Clique **"Criar"**
3. Preencha:
   - **App name**: `Mesada do Leo`
   - **User support email**: seu email
   - **Developer contact**: seu email
4. Clique **"Salvar e continuar"**
5. Na próxima tela, clique **"Salvar e continuar"** novamente
6. Clique **"Voltar para painel"**

---

## PASSO 4: Criar Credenciais (Client ID)

1. No menu esquerdo, clique **"Credenciais"**
2. Clique **"+ Criar credencial"** → **"ID do cliente OAuth"**
3. Tipo de aplicativo: **"Aplicativo da web"**
4. Nome: `Mesada Leo Web`
5. Em **"URIs autorizados de redirecionamento"**, adicione:
   ```
   https://erikafribeiro-dev.github.io/mesada/
   http://localhost:8000/
   ```
6. Clique **"Criar"**
7. Na popup, clique copiar ou abra o arquivo `.json`

---

## PASSO 5: Copie o Client ID

Na credencial criada:
- Você verá um **Client ID** como:
  ```
  123456789-abc123def456.apps.googleusercontent.com
  ```
- **COPIE ESTE VALOR**

---

## PASSO 6: Configure no Código

Avise-me o **Client ID** e vou adicionar ao código da app!

Formato:
```
Cliente ID: 123456789-abc123def456.apps.googleusercontent.com
```

---

## Pronto! ✅

Depois de adicionar o Client ID:
1. Ajustes → "☁️ Google Drive"
2. Clica "🔗 Autorizar Google Drive"
3. Popup do Google aparecer
4. Autoriza
5. ✅ Salva automático na pasta!

---

## Dúvidas?

Se não aparecer popup ou der erro, verifique:
- ✅ Google Drive API ativada
- ✅ Client ID correto no código
- ✅ URLs de redirecionamento configuradas
- ✅ OAuth Consent Screen criado

Pronto! Avise quando tiver o Client ID 🚀
