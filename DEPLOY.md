# Deploy na Vercel

## Preparação (feita)

✅ Repositório Git inicializado  
✅ Arquivo HTML pronto  
✅ Configuração Vercel criada  

## Próximos passos (você faz)

### 1. Criar repositório no GitHub

1. Abra https://github.com/new
2. Nome do repositório: `combo-simulados-pmmg`
3. Descrição: "Aplicativo para acompanhamento de simulados PMMG"
4. Selecione **Public** (para os alunos acessarem)
5. Clique em **Create repository**

### 2. Fazer push do repositório local

No terminal, dentro de `C:\Users\heitt\Documents\claude`:

```bash
git add .
git commit -m "Initial commit: Combo de Simulados app"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/combo-simulados-pmmg.git
git push -u origin main
```

⚠️ Substitua `SEU_USUARIO` pelo seu usuário do GitHub.

### 3. Deploy na Vercel

1. Abra https://vercel.com/new
2. Clique em **Import Git Repository**
3. Cole o link: `https://github.com/SEU_USUARIO/combo-simulados-pmmg.git`
4. Clique em **Import**
5. Vercel detectará automaticamente que é um projeto estático
6. Clique em **Deploy**

Pronto! Em ~1 minuto, você terá um link público tipo:  
`https://combo-simulados-pmmg.vercel.app/`

### 4. Compartilhar com alunos

Copie o link e compartilhe por:
- Área de membros do seu site
- E-mail
- WhatsApp
- Seu LMS (Google Classroom, Moodle, etc.)

## Atualizar o app no Vercel

Sempre que você editar o arquivo HTML localmente:

```bash
git add combo-simulados-pmmg.html
git commit -m "Descrição da alteração"
git push
```

Vercel faz deploy automático em ~30 segundos. Os alunos sempre veem a versão mais recente.

## Dúvidas

- **Preciso pagar?** Não. Vercel oferece hosting gratuito para projetos estáticos.
- **E se o GitHub cair?** Os alunos continuam usando normalmente — a Vercel já fez cache da versão.
- **Como os alunos fazem backup dos dados?** Aba "Configurações" → "Exportar backup" → arquivo JSON (local no computador deles).
