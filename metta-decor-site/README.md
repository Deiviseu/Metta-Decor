# Metta Decor — site

Site de uma página da Metta Decor (móveis e estofados sob medida, São Paulo).
HTML, CSS e JavaScript puros, sem etapa de build.

## Estrutura

```
index.html            página completa (estilos e scripts embutidos)
img/                  fotos em WebP, logo, ícone e imagem de compartilhamento
favicon.ico
apple-touch-icon.png
robots.txt
sitemap.xml
vercel.json           cache das imagens, redirecionamento /index.html → /
```

Dependências externas (via CDN): GSAP 3.12.5 + MotionPathPlugin (galeria circular dos sofás) e as fontes Bodoni Moda e Jost do Google Fonts.

## Rodar localmente

Abra `index.html` no navegador, ou sirva a pasta:

```
npx serve .
```

## Publicar na Vercel

1. Suba esta pasta para um repositório no GitHub.
2. Na Vercel: **Add New → Project**, importe o repositório.
3. Framework Preset: **Other**. Build Command e Output Directory: deixe em branco.
4. Deploy.
5. Para usar `mettadecor.com.br`, adicione o domínio em **Settings → Domains** e ajuste o DNS conforme a Vercel indicar.

## Onde editar

- **WhatsApp:** constante `WA` no script (`551129562570`). Os botões com `data-wa` montam o link com a mensagem.
- **Produtos:** listas `SOFAS`, `MESAS`, `POLT` e `AMB` no script (título, descrição, texto alternativo).
- **Cores do simulador de tecido:** lista `COLORS` (amostra `c` e cor aplicada `paint`).
- **Endereço e horário:** seção `#loja` e o bloco JSON-LD no `<head>`.

## Pendências com o cliente

- Bairro e CEP do endereço.
- Nomes reais dos modelos (os atuais foram descritos a partir das fotos).
- Google Analytics 4, se o cliente quiser manter (`G-1BV5YK4LMH` era o ID do site antigo).
