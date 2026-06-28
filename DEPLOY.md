# Deploy — SAL OCEANO aromas

## GitHub Pages (domínio customizado)

1. Crie um repositório no GitHub (ex: `saloceano-site`)
2. Faça upload de todos os arquivos desta pasta para a raiz do repositório
3. Vá em **Settings > Pages**
4. Em *Source*, selecione `Deploy from a branch` → branch `main` → pasta `/ (root)`
5. Em *Custom domain*, insira `www.saloceano.com.br` e salve
6. No painel DNS do seu domínio, configure:
   - Tipo `CNAME` | Host `www` | Aponta para `seu-usuario.github.io`
7. Aguarde a propagação DNS (até 24h). O HTTPS é ativado automaticamente.

## Estrutura de arquivos

```
/
├── index.html          ← site principal (tudo inline)
├── imagens/            ← fotos dos produtos, quiosques, loja
├── assets/             ← logo, ícones e arquivos extras
├── flags/              ← bandeiras para futura versão multilíngue
├── CNAME               ← domínio customizado (não editar)
├── .gitignore
├── DEPLOY.md           ← este arquivo
└── README.md
```

## Imagens necessárias

Todas as imagens ficam em `imagens/`. As principais referenciadas no HTML:

- `logo.png`
- `difusor-*.jpeg / .png`
- `vela-*.jpeg`
- `agua-tecido-*.jpeg`
- `loja-conceito-01.png`, `loja-conceito-02.png`, `loja-interior.jpeg`
- `kiosque-render-01.png` até `kiosque-render-04.png`
- Imagens lifestyle, artesanal, bolsas, kits

## Formulário de contato

O formulário usa **Formspree** (`https://formspree.io/f/xnjkpyoq`).
Na primeira submissão, confirme o e-mail de destino no painel do Formspree.

## Atualizar o site

Edite `index.html` e faça commit. O GitHub Pages atualiza em ~1 minuto.
