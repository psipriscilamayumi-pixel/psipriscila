# Site — Priscila Mayumi Tagima (Psicóloga)

Site institucional em HTML/CSS/JS puro, pronto para deploy gratuito na Vercel via GitHub.

## Arquivos
- `index.html` — estrutura e conteúdo do site
- `style.css` — todo o estilo visual
- `script.js` — pequena interação do FAQ

## Pendências de conteúdo
- [ ] Adicionar a foto real da Priscila. Hoje a seção "Sobre mim" tem uma
      caixa de placeholder no lugar da foto. Para trocar: coloque o arquivo
      de imagem (ex: `foto.jpg`) nesta mesma pasta e, no `index.html`, troque
      este trecho:
      ```html
      <div class="photo-frame">
        <span class="photo-placeholder">Foto de<br>Priscila</span>
      </div>
      ```
      por:
      ```html
      <div class="photo-frame">
        <img src="foto.jpg" alt="Priscila Mayumi Tagima" style="width:100%;height:100%;object-fit:cover;border-radius:4px;">
      </div>
      ```
- [ ] Revisar/completar o texto de apresentação em "Sobre mim"
- [ ] Definir paleta de cores definitiva (atualmente: verde-petróleo + dourado + areia)
- [ ] Adicionar depoimentos reais de pacientes, se e quando houver autorização deles

## Como publicar (passo a passo)

### 1. Criar o repositório no GitHub
1. Acesse [github.com](https://github.com) e crie uma conta gratuita, se ainda não tiver.
2. Clique em **New repository**.
3. Dê o nome `psipriscilamay` (ou o nome que preferir), deixe como **Public**, e clique em **Create repository**.

### 2. Subir os arquivos
**Opção fácil (sem terminal):** na página do repositório recém-criado, clique em **uploading an existing file** e arraste os arquivos desta pasta (`index.html`, `style.css`, `script.js`, e a foto).

**Opção via terminal**, dentro desta pasta:
```bash
git init
git add .
git commit -m "Primeira versão do site"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/psipriscilamay.git
git push -u origin main
```

### 3. Publicar na Vercel
1. Acesse [vercel.com](https://vercel.com) e crie uma conta gratuita usando o login do GitHub.
2. Clique em **Add New → Project**.
3. Selecione o repositório `psipriscilamay`.
4. Como é um site estático (sem framework), a Vercel detecta automaticamente — não precisa mudar nenhuma configuração. Clique em **Deploy**.
5. Em poucos segundos o site estará no ar em um endereço como `psipriscilamay.vercel.app`.

### 4. Atualizações futuras
Sempre que quiser mudar algo, edite os arquivos, suba de novo pro GitHub (`git add .`, `git commit`, `git push`, ou reenviando pelo site), e a Vercel atualiza o site sozinha automaticamente.

### 5. Domínio próprio (opcional, pago à parte)
Se um dia ela quiser um domínio tipo `priscilatagima.com.br`, dá pra comprar num registrador (ex: registro.br) e conectar direto no painel da Vercel, em **Settings → Domains**.
