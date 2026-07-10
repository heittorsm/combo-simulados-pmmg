# Setup Vercel — Guia Rápido

## O que você vai fazer

Hospedar o app na Vercel gratuitamente e gerar um link público para compartilhar com os alunos.

Tempo estimado: **5 minutos**

---

## Pré-requisitos

- [ ] Conta no GitHub (crie em https://github.com/signup se não tiver)
- [ ] Conta na Vercel (crie em https://vercel.com/signup — pode usar GitHub para autenticar)

---

## Passo 1: Criar repositório no GitHub

1. Acesse https://github.com/new
2. **Repository name:** `combo-simulados-pmmg`
3. **Description:** Aplicativo para acompanhamento de simulados PMMG
4. **Visibility:** Public (importante para os alunos acessarem)
5. Clique em **Create repository**

Você será levado a uma página mostrando comandos. **Copie a URL** (tipo `https://github.com/SEU_USUARIO/combo-simulados-pmmg.git`).

---

## Passo 2: Fazer push (enviar código para o GitHub)

Abra o **PowerShell** (ou cmd) e digite:

```powershell
cd C:\Users\heitt\Documents\claude
```

Depois:

```powershell
git remote add origin https://github.com/SEU_USUARIO/combo-simulados-pmmg.git
git branch -M main
git push -u origin main
```

⚠️ **Substitua** `SEU_USUARIO` pelo seu username do GitHub  
⚠️ Se pedir autenticação, use seu token pessoal (https://github.com/settings/tokens)

Se tudo deu certo, você verá:
```
Enumerating objects: ...
remote: Create a pull request for 'main' on GitHub...
```

---

## Passo 3: Deploy na Vercel

1. Acesse https://vercel.com/new
2. Clique em **Import Git Repository**
3. Cole a URL do seu repositório: `https://github.com/SEU_USUARIO/combo-simulados-pmmg.git`
4. Clique em **Import**
5. Vercel vai detectar que é um projeto estático (não precisa fazer nada)
6. Clique em **Deploy**

Aguarde ~1 minuto. Vercel mostrará uma tela de sucesso com o link final.

---

## 🎉 Pronto!

Seu link será algo como:
```
https://combo-simulados-pmmg.vercel.app
```

**Compartilhe este link com os alunos!**

---

## Próximos passos

- **Atualizar o app:** edite o arquivo HTML local, faça push para o GitHub, e Vercel fará deploy automático
- **Monitorar uso:** na dashboard da Vercel, você vê quantas visitas o app teve
- **Adicionar domínio personalizado:** Vercel oferece a opção de conectar um domínio seu

---

## Troubleshooting

### "fatal: Authentication failed for 'https://github.com/...'"
→ Use um **token pessoal** em vez de senha (https://github.com/settings/tokens/new)

### "Repository not found"
→ Verifique se o repositório é **Public** e se a URL está correta

### "Deploy failed"
→ Vercel pode ter um erro. Clique em "Redeploy" na dashboard dele

---

**Dúvidas?** Abra uma issue no repositório ou envie um e-mail.
