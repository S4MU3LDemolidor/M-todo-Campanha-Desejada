# DESIGN.MD — Sistema Visual
## Método Campanha Desejada | Julia Cardoso Aragão

---

## VISÃO GERAL

**Estilo:** Elegante, premium, feminino e minimalista  
**Referência de vibe:** Editorial de moda brasileira — não é fria nem corporativa. Tem calor, mas tem sofisticação.  
**Feeling que a página deve transmitir:** "Essa mulher sabe o que está fazendo. E eu quero aprender com ela."

---

## PALETA DE CORES

### Cores primárias

| Nome | Hex | Uso |
|---|---|---|
| Marrom escuro | `#3B2314` | Títulos principais, CTA, elementos de destaque |
| Marrom médio | `#7C4A2D` | Subtítulos, ícones, detalhes |
| Off-white quente | `#F5F0E8` | Background principal da página |
| Creme | `#EDE5D8` | Fundo de seções alternadas, cards |

### Cores de apoio

| Nome | Hex | Uso |
|---|---|---|
| Branco puro | `#FFFFFF` | Texto sobre fundos escuros, cards flutuantes |
| Marrom claro / bege | `#C4A882` | Bordas, separadores, detalhes decorativos |
| Marrom muito escuro | `#1E110A` | Texto corrido (body) |

### Gradiente de seção (opcional)
- De `#F5F0E8` para `#EDE5D8` — transição suave entre blocos

---

## TIPOGRAFIA

### Hierarquia

| Elemento | Fonte | Peso | Observação |
|---|---|---|---|
| Headlines H1 | Serif (ex: Playfair Display ou Cormorant Garamond) | 400 italic ou 700 | Grandes, elegantes |
| Headlines H2 | Sans-serif (ex: DM Sans ou Inter) | 700 | Limpas, diretas |
| Palavra de destaque em H1 | Serif itálico | 400 | Mix serif/sans dentro da mesma linha (igual refs) |
| Body text | Sans-serif (DM Sans ou Inter) | 400 | 16–18px, espaçamento generoso |
| Labels / tags | Sans-serif uppercase | 500–600, letter-spacing +0.1em | Ex: "MÓDULO 01", "BÔNUS" |
| CTA buttons | Sans-serif | 600 | Uppercase ou sentence case |

### Combinações recomendadas (Google Fonts — free)
- **Opção A:** Cormorant Garamond (serif) + DM Sans (sans) ← mais elegante
- **Opção B:** Playfair Display (serif) + Inter (sans) ← mais legível em mobile

### Regras de tipografia
- Headline principal: mix de pesos e estilos dentro da mesma linha (como nas refs)  
  Ex: `Suas peças são` [regular] + `lindas.` [italic serif]
- Nunca usar mais de 2 famílias tipográficas
- Line-height generoso no body: 1.7–1.8
- Tamanho mínimo de body no mobile: 16px

---

## LAYOUT E ESTRUTURA

### Grid
- **Desktop:** Container centralizado, max-width `1100px`, padding lateral `80px`
- **Mobile:** Padding lateral `20px`, stack vertical de todos os elementos

### Seções e espaçamento
- Espaço entre seções: `120px` no desktop, `80px` no mobile
- Seções alternadas entre fundo off-white `#F5F0E8` e creme `#EDE5D8`
- Uma seção pode ter fundo marrom escuro `#3B2314` com texto branco (ex: bloco de preço ou depoimentos)

### Elementos visuais recorrentes

**Linha decorativa fina**  
- `1px solid #C4A882` — usada como separador horizontal ou detalhe ao lado de títulos

**Tag / label de seção**  
- Texto uppercase pequeno, letra espaçada, marrom médio  
- Ex: `— MÓDULO 01 —` ou `BÔNUS EXCLUSIVO`

**Destaque de palavra em headline**  
- Palavra em serif itálico dentro de headline sans  
- Ou palavra com underline decorativo (linha fina abaixo, cor marrom claro)

**Caixa de destaque / callout**  
- Fundo `#EDE5D8`, borda esquerda `3px solid #7C4A2D`  
- Para quotes, depoimentos ou pontos de atenção

---

## COMPONENTES

### Botão CTA
```
Background: #3B2314
Texto: #F5F0E8 (off-white)
Border-radius: 2px (quase reto — look premium, não arredondado demais)
Padding: 18px 40px
Font: DM Sans 600, uppercase ou sentence case
Hover: background #1E110A (mais escuro)
```

**Variante outline (CTA secundário):**
```
Background: transparent
Border: 1.5px solid #3B2314
Texto: #3B2314
Hover: background #3B2314, texto #F5F0E8
```

### Card de módulo
```
Background: #FFFFFF
Border: 1px solid #EDE5D8
Border-radius: 4px
Padding: 32px
Sombra suave: 0 2px 12px rgba(59,35,20,0.06)
Número do módulo: label uppercase marrom médio
Título: serif bold
Descrição: sans regular, marrom muito escuro
```

### Card de bônus
```
Background: #EDE5D8
Border-radius: 4px
Padding: 32px
Ícone ou número: marrom médio
Badge "BÔNUS": tag uppercase pequena
```

### Bloco de preço
```
Background: #3B2314
Texto: #F5F0E8
Preço em destaque: Cormorant Garamond, grande (64px+)
Parcelamento: DM Sans regular, menor
CTA: botão off-white com texto marrom
```

### FAQ — accordion
```
Borda inferior: 1px solid #C4A882
Título da pergunta: DM Sans 600, marrom escuro
Resposta: DM Sans 400, expandível
Ícone de toggle: + / − em marrom médio
```

---

## IMAGENS E FOTOS

### Estilo fotográfico esperado
- **Tom:** Editorial, natural, com luz quente (não estúdio frio)
- **Paleta das fotos:** Tons quentes, compatíveis com marrom e off-white
- **Poses:** Confiante mas acessível — não é arrogante, é autoridade
- **Roupas na foto:** Tons neutros (off-white, bege, marrom, preto) para harmonizar com a identidade
- **Fundo ideal:** Neutro (off-white, bege, concreto claro) ou ambiente elegante

### Fotos necessárias (lista para Julia)
- [ ] Hero: foto da Julia — enquadramento meio/3/4, levemente acima da dobra, expressão segura
- [ ] História: foto mais casual/humanizada (pode ser sentada, trabalhando ou olhando câmera de forma leve)
- [ ] Credenciais: foto profissional ou em evento (palestras, eventos do setor)
- [ ] Mobile: foto vertical bem enquadrada (ideal 4:5 ou 9:16 cropped)

### Tratamento de imagem
- Overlay sutil marrom/quente se a foto tiver luz muito fria
- Sem filtros pesados — foto deve parecer real, não editada em excesso
- Fotos de produto da Flossie podem aparecer como prova social visual

---

## ANIMAÇÕES E INTERATIVIDADE

### Princípios
- Minimalismo total: não tem animação pra chamar atenção, só pra dar respiro
- Scroll suave (smooth scroll)
- Fade-in sutil nos elementos ao entrar na viewport (`opacity 0 → 1`, `translateY 20px → 0`, duration `0.5s`)
- Sem parallax pesado, sem explosões de elementos

### Hover states
- Botões: transição de cor `0.2s ease`
- Cards: sombra levemente aumentada no hover
- Links: underline que aparece no hover

---

## REFERÊNCIAS VISUAIS (análise das imagens enviadas)

### Imagem 1 — Mag Studio / Mariana Guimarães
**O que absorver:**
- Mix tipográfico entre serif grande e sans uppercase → funciona muito bem como headline
- Foto ambiental com texto sobreposto elegante
- Fundo natural/madeira → faz alusão ao off-white/quente que queremos

### Imagem 2 — Alice Santana (pacotes de design 2026)
**O que absorver:**
- Foto de autoridade como background com texto na parte inferior
- Tipografia mista: sans regular + sans bold na mesma linha
- Paleta marrom + off-white exatamente como queremos
- Tag de contexto no topo ("POSICIONAMENTO VISUAL | BRANDING E CONTEÚDO") — vamos replicar

### Imagem 3 — Karol Lopes | Marketing e Conteúdo
**O que absorver:**
- Hierarquia tipográfica clara: nome/contexto no topo, headline grande no meio
- Mix serif cursiva + sans bold dentro da mesma headline
- Fundo degradê neutro (marrom/bege) com foto do profissional integrada
- "Highlight box" na palavra de destaque ("momento atual" com fundo escuro) — detalhe elegante que podemos usar em CTA ou bloco de dor

---

## ESTRUTURA DE SEÇÕES (ordem na página)

```
01. [HERO] — Foto Julia + headline + subheadline + CTA
02. [LOGOS] — Parceiros (Nuvemshop, Appmax, Olist, Mizui) — barra de credibilidade
03. [DOR] — Identificação com o problema
04. [HISTÓRIA] — Jornada da Julia
05. [O MÉTODO] — O que é + módulos
06. [DIFERENCIAIS] — Por que esse e não outro
07. [PARA QUEM É] — Fit / não fit
08. [BÔNUS] — Cards de bônus com destaque "primeiros dias"
09. [PREÇO + CTA] — Bloco dark, preço, parcelamento, botão
10. [GARANTIA] — Bloco simples, ícone de escudo
11. [FAQ] — Accordion de objeções
12. [FECHAMENTO] — Última headline emocional + CTA final
13. [FOOTER] — Nome da marca, links legais, contato
```

---

## CHECKLIST DE ASSETS NECESSÁRIOS

### Precisa criar do zero (conforme briefing)
- [ ] Logo do "Método Campanha Desejada" (tipográfica, simples, elegant)
- [ ] Favicon
- [ ] OG Image para compartilhamento (1200x630px)
- [ ] Artes de bônus para visualização na página

### Receber da Julia
- [ ] Fotos (ver seção de imagens acima)
- [ ] Logos dos parceiros (Nuvemshop, Appmax, Olist, Mizui) em PNG com fundo transparente
- [ ] Preço final confirmado
- [ ] Plataforma de pagamento (para integração do botão CTA)
- [ ] Texto dos módulos reais do curso

---

## NOTAS TÉCNICAS PARA DESENVOLVIMENTO

- **Framework sugerido:** HTML + CSS + JS vanilla (sem dependência pesada) ou Next.js se preferir
- **Fontes:** Google Fonts (Cormorant Garamond + DM Sans)
- **Responsivo:** Mobile-first. A maioria das alunas vai acessar pelo celular.
- **Performance:** Imagens em WebP, lazy loading, CLS zero
- **Pixel:** Integrar pixel do Meta Ads (orçamento de tráfego confirmado no briefing)
- **Formulário/CTA:** Integrar com plataforma de hospedagem do curso (a definir)
- **Analytics:** Google Analytics 4 + Meta Pixel

---

## ITENS QUE FALTAM (PREENCHER COM JULIA)

- [ ] Fotos da Julia (bloqueador principal)
- [ ] Logo criada / aprovada
- [ ] Plataforma de hospedagem do curso (para integração)
- [ ] Plataforma de pagamento
- [ ] Preço final e parcelamento
