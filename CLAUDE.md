# CLAUDE.md — ALAST

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** ALAST
**Nicho:** Negócios e Empreendedorismo
**Keywords:** Associacao Latino Americana de Estudos do Trabalho Unimos esse grupo para compartilharmos
**Paleta de cores:** gold | **Fonte:** playfair

Associação Latino Americana de Estudos do Trabalho Unimos esse grupo para compartilharmos conteúdos relacionados às áreas que envolvem o Trabalho. Nosso grupo é composto por diversos profissionais que enviam suas análises sobre determinados temas de suas especialialidades, como: – Técnicos da segurança o trabalho – Advogados especializados em Direito Trabalhista – Especialistas em e-Social – Administradores de empresas – Coachs de líderes – Empresários – Executivos – Gerentes – Jornalistas. Dentre outros.. Nosso objetivo é informar nossos leitores à cerca de tudo que acontece no Mundo do Trabalho. Se você quiser juntar-se a nós e escrever nesse Blog também clique aqui: Entrar em Contato Att, Vitor Lima Contador. Sobre Eu sou o Vitor, Contador e Responsável Técnico de Contabilidade da minha empresa e dos meus clientes. Tenho o prazer de simplificar os processos para pequenos empreendedores, para trabalhadores em geral e profissionais que têm interesse no assunto. Então, nada mais justo começarmos a simplificar a forma de falarmos sobre TRABALHO.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-D |
| Hero | Hero-E |
| Features | Features-H |
| About Section | About-I |
| Posts | Posts-C |
| Footer | Footer-D |
| Página Sobre | Sobre-B |
| Página Contato | Contato-A |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
