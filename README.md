# NORTE Mentoria — landing page

Site estático de uma página. Sem build, sem dependências de servidor.

## Arquivos

- `index.html` — a página inteira (HTML + CSS embutido). É o único arquivo obrigatório.
- `samuel.jpg` — retrato do Samuel na seção "Quem conduz". **Você precisa adicionar este arquivo.**
  Enquanto ele não existir, a página mostra um quadro vazio no lugar, sem quebrar.
  Formato ideal: vertical 4:5 (ex.: 1200 × 1500 px), fundo escuro, até ~300 KB.
- `CNAME` — domínio personalizado do GitHub Pages. Ajuste ou apague se não for usar domínio próprio.
- `.nojekyll` — evita que o GitHub Pages processe os arquivos com Jekyll.

## Como publicar no GitHub Pages

1. Crie um repositório novo no GitHub (público).
2. Envie o conteúdo desta pasta para a raiz do repositório:

   ```
   git init
   git add .
   git commit -m "Landing page NORTE Mentoria"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/SEU-REPO.git
   git push -u origin main
   ```

   (Ou use "Add file › Upload files" pela interface do GitHub — funciona igual.)
3. No repositório, vá em **Settings › Pages**.
4. Em *Source*, escolha **Deploy from a branch**; branch `main`, pasta `/ (root)`. Salve.
5. Em um ou dois minutos o site fica no ar em `https://SEU-USUARIO.github.io/SEU-REPO/`.

## Domínio próprio (nortementoria.com.br)

Se for usar o domínio, mantenha o arquivo `CNAME` e configure no seu provedor de DNS:

- Registro **CNAME** de `www` apontando para `SEU-USUARIO.github.io`
- Registros **A** do domínio raiz apontando para: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153

Depois, em Settings › Pages, marque **Enforce HTTPS**.

## O que editar na página

Tudo está dentro de `index.html`:

- **WhatsApp** — busque por `wa.me/5561992481062` (3 ocorrências: header, hero e CTA final).
- **Currículo Lattes** — busque por `lattes.cnpq.br` e troque pela URL real do currículo.
- **Bônus da primeira turma** — a seção começa no comentário do bloco com borda dourada; apague a
  `<section>` inteira quando a turma de lançamento fechar.
- **Contato no rodapé** — telefone, e-mail, Instagram e site.
