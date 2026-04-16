# CLAUDE.md — TSRCONCURSOS

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** TSRCONCURSOS
**Nicho:** Negócios e Empreendedorismo
**Keywords:** A T S R Prestadora de Servicos S S Ltda empresa constituida
**Paleta de cores:** slate | **Fonte:** outfit

A T.S.R. Prestadora de Serviços S/S Ltda empresa constituída em 01 de junho de 1.997, está voltada á prestação de serviços nas áreas de Administração Pública e Privada. A T.S.R. Prestadora de Serviços S/S Ltda vem atuando em várias cidades, dispondo de um quadro de profissionais altamente especializados e qualificados. A filosofia de trabalho da T.S.R. Prestadora de Serviços S/S Ltda tem por objetivo atingir resultados concretos nas suas respectivas áreas de atuação, levando, consequentemente, benefícios aos nossos clientes, em especial com a prestação de serviços de QUALIDADE e EXCELÊNCIA, trazendo um ótimo ambiente de trabalho, segurança, estabilidade e profissionalismo em sua equipe. Atendendo as exigências de mercado, e sobre tudo a necessidade de seus clientes, fornecendo soluções tecnologicamente adequadas. Tendo assim como missão, excelência técnica e ética aliada a uma atenção especial a nossos clientes. ÁREA DE TRABALHO A T.S.R Prestadora de Serviços S/S Ltda tem como objetivo ser um ponto de apoio importante aos Administradores Públicos e à Administração Pública bem como na Administração Privada em todos os seus níveis. Em todos esses anos de trabalho com experiência comprovada e seriedade incontestável, oferecemos nossos serviços especializados, contando com profissionais altamente qualificados e experiente no trabalho na execução de Prestação de Serviços nas áreas de Processamento de Dados, Organização e Informatização de Almoxarifado e Departamento Pessoal, Licitações Públicas (Treinamento e Assessoria), Comércio Exterior (Assessoria de Exportação e Importação) e outros setores da Administração Pública e Privada. Nossa atuação na Administração Pública, está diretamente voltada a: Treinamento e Assessoria em Licitações Públicas. Curso e Assessoria em Lei de Responsabilidade Fiscal. Realização de Concursos Públicos e Processos Seletivos. Organização das áreas de Almoxarifado, Departamento Pessoal, Expediente e Protocolo. Estudo do Quadro de Pessoal, Plano de Carreira e Propostas para Reforma ou Restruturação Administrativa. Emissão de recibos ou boletos. Coleta de Leituras Informatizadas. Outros demais serviços atinentes ao Serviço Público.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-F |
| Hero | Hero-E |
| Features | Features-A |
| About Section | About-A |
| Posts | Posts-F |
| Footer | Footer-E |
| Página Sobre | Sobre-F |
| Página Contato | Contato-C |

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
