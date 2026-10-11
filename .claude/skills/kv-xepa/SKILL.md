---
name: kv-xepa
description: Identidade visual (KV) do XEPA, restaurante de parrilla, burger e coquetelaria autoral na Santa Cecília (São Paulo), flagship do Grupo XEPA. KV "XEPA ELEGANTE" (linguagem do cardápio em InDesign): fundo claro, uma cor verde, creme, molduras finas e muito respiro. Use ao criar posts, cardápios, hotsite, embalagens, cartazes, ilustrações ou qualquer peça do XEPA. Traz paleta medida, fontes e alternativas, regras de layout, estilo de ilustração, prompt pronto e referências.
---

# KV · XEPA (XEPA ELEGANTE)

**O melhor burger de São Paulo** · drinks autorais & média gastronomia · Santa Cecília · desde 2023.
Eleito melhor hambúrguer de SP e 2º melhor do Brasil (Hambúrguer Perfeito). Instagram: **@xepabr** · www.xepa.cc

Assets: `marcas/xepa/` · tokens prontos: `marcas/xepa/tokens.css`
Fonte da verdade: cardápio `mennu_xepa_final_setembro_CORTE_2026` (InDesign, Drive falecomxepa: GRUPO XEPA/XEPA/CARDAPIO/ANO 3.5.1/FINAL). Referência visual: `kv/referencia-cardapio-comidas.jpg` e `kv/referencia-cardapio-drinks.jpg`.

> Pedido do dono (11/10/2026): **"ELEGANTE, apenas dessas cores e o InDesign; XEPA é nessa elegância, sóbrio, claro."**

## Essência e tom de voz
- Manifesto: *"A forma como transformamos o alimento também nos transforma."*
- Fogo bem usado e respeito pelos ingredientes; valoriza o pequeno produtor; técnica **e** afeto.
- Tom: seguro, elegante, sem gritar. Frases curtas. Humor só nas ilustrações (Xepinha, Diogo), nunca no layout.
- Produto-herói: **Cheese Bacon à Cavalo** (180 g na parrilla, queijo prato, bacon de barriga defumado da casa, ovo, pão de batata).

## Paleta (só estas cores · medidas no PDF do cardápio e nas ilustrações)
| Token | HEX | Uso |
|---|---|---|
| `--xepa-branco` | `#ffffff` | **fundo principal** (o cardápio é branco) |
| `--xepa-papel` | `#f6f2e9` | fundo alternativo: papel creme claro (`kv/textura-papel-menu.jpg`) |
| `--xepa-verde` | `#3c8e6c` | **a cor da marca**: títulos de seção, faixas cheias, molduras, logo, lettering "Cheese Bacon à cavalo" |
| `--xepa-musgo` | `#364b3d` | texto (nomes e descrições) e traço das ilustrações sóbrias (nas artes mede `#3d4c3b`) |
| `--xepa-creme` | `#fefceb` | preenchimento das ilustrações e caixas |
| `--xepa-creme-texto` | `#f1e7d5` | texto e filetes **sobre** a faixa verde |
| `--xepa-salvia` | `#96a478` | ilustração em traço leve (copinho), detalhe |
| `--xepa-garrafa` | `#008f6b` | ilustração dos copos brindando |
| `--xepa-pontilhado` | `#009a70` | a corrente de losangos ◇◇◇ entre nome e preço |

**Cor de campanha (secundária):** menta `#81d0a7` + preto `#000000` só em peças comemorativas (ex.: "Festa de Aniversário Ano 2", `kv/kv-trio.png`). Nunca no cardápio nem no dia a dia.
**Proibido:** coral, rosa, salmão, vermelho, amarelo, azul, gradientes, sombra deslocada, fundo escuro de página inteira.
> A "matriz das artes" de 03/10 (menta + preto + sombra deslocada, commit `ebff34b`) **saiu do KV do dia a dia**: o deslocamento e o preto contradizem o sóbrio. Menta + preto sobrevivem só como cor de campanha de aniversário.

## Tipografia
| Papel | Fonte original (InDesign) | Alternativa Google Fonts | Regra |
|---|---|---|---|
| Títulos de seção | **Harmond SemiBold Condensed** | **Instrument Serif** | CAIXA ALTA, tracking +6%, verde `#3c8e6c`, centralizado na caixa |
| Nomes dos itens | **Harmond SemiBold Condensed** | **Instrument Serif** | CAIXA ALTA, tracking +3%, musgo `#364b3d` (creme/branco sobre faixa verde) |
| Descrições | **Brandon Grotesque Light** | **Jost 300** | caixa normal, entrelinha justa (~1.15), musgo |
| Selos curtos | **Shackleton Condensed** | **Oswald 500** | CAIXA ALTA, só em selo ("MELHOR HAMBÚRGUER DE SÃO PAULO") |

- Por quê: Instrument Serif é a serifa condensada de alto contraste mais próxima da Harmond SemiBold Condensed (mesmo desenho estreito e "vintage"); Jost Light é geométrica e leve como a Brandon Light; Oswald já vem no pacote do InDesign (pasta *Document fonts*) e é a condensada mais próxima da Shackleton.
- Hierarquia do cardápio (A3 deitado): título de seção 31 pt · nome do item 19 pt · descrição 12 pt (10 pt nos drinks). Proporção ≈ **1 : 0,6 : 0,4**.
- Nada de itálico decorativo, nada de negrito pesado, nada de mais de 2 famílias por peça.
- **Licenças:** Harmond, Shackleton e Brandon Grotesque são comerciais e **não estão neste repositório**. Para o original, comprar licença (Harmond/Dirtyline e Shackleton estavam como "personal use"/teste na pasta FONTS).

## Regras de layout (a linguagem do InDesign)
1. **Fundo claro sempre:** branco ou papel creme `#f6f2e9`. Muito respiro: margem externa ≥ 5% do lado menor; nunca encostar texto na moldura.
2. **Uma cor por peça + creme:** verde `#3c8e6c` para estrutura e títulos, musgo para texto. Sálvia e verde garrafa só dentro de ilustração.
3. **Caixas com moldura fina ornamentada** (`kv/moldura-caixa.png`, ou CSS `.xepa-caixa`): filete verde de ~1,25 pt com cantos em degrau ("orelhas") e um quadradinho vazado em cada canto. Título da seção dentro da caixa, no topo, centralizado.
4. **Faixa verde cheia para destaque** (`kv/faixa-verde.png`, ou `.xepa-faixa`): o item em destaque vira uma faixa verde que **vaza um pouco** para fora da moldura dos dois lados, com filete creme interno e os mesmos cantos em degrau. Texto da faixa em branco/creme. No máximo 1 faixa por caixa.
5. **Preço com pontilhado:** NOME ◇◇◇◇◇◇ PREÇO, na mesma linha; a corrente é de losanguinhos em `#009a70` (CSS: `.xepa-pontilhado`). Preço sem "R$", em Harmond/Instrument Serif, alinhado à direita.
6. **Ícone de vegetariano:** folhinha verde depois do nome.
7. **Ilustração como respiro, não como fundo:** uma ilustração por bloco, encostada num canto da caixa ou "saindo" dela (ex.: Cheese Bacon à cavalo saindo da caixa de Hambúrgueres, jamón ao lado do Abuela).
8. **Logo:** `logos/xepa-logo-verde.png` (verde texturizado) sobre fundo claro; `logos/xepa-logo.png` (musgo) quando a peça pede mais sobriedade. Abaixo: `@xepabr · www.xepa.cc` em descrição pequena. Nunca redesenhar o logo nem pôr sombra.
9. **Post/stories:** mesma gramática do cardápio: fundo claro, uma caixa com moldura, título em CAIXA ALTA verde, uma ilustração em traço, a faixa verde para a informação principal (data, preço, prato).

## Estilo de ilustração (XEPA)
- **Técnica:** gravura (linogravura/xilogravura leve) com **hachura cruzada** e **meio-tom pontilhado** nas sombras, traço de nanquim irregular, contorno à mão. Ver `kv/referencias-estilo/xepa-traco-diogo-zoom.jpg` e `xepa-traco-jamon-zoom.jpg`.
- **Cores:** duas tintas no máximo: traço musgo `#3d4c3b` **ou** verde `#3c8e6c` sobre preenchimento creme `#fefceb`. Variações aceitas: traço sálvia `#96a478` (copinho), verde garrafa `#008f6b` (copos brindando), branco sobre faixa verde (cabeça do Xepinha).
- **Explosão/sunburst** creme atrás do objeto (prato, jamón) para destacar sem usar cor.
- **Lettering** manuscrito de pincel ("CHEESE BACON à cavalo"): verde chapado com sublinhado em pincelada.
- **Personagem: SEMPRE o XEPINHA.** Toda peça do XEPA que tiver ilustração tem o Xepinha, o mascote, como protagonista, interagindo com o tema (segurando garfo ou copo, espiando de trás do prato, apontando para a data). Nunca inventar outro personagem, mascote genérico ou criança qualquer.
  - Como ele é: desenho animado dos anos 1930 ("rubber hose"), cabeça grande, cabelo/topete volumoso, olhos grandes ovais, sorriso largo com a língua de fora, luvas de desenho animado, braços de mangueira; traço verde `#2f6b4f`/musgo com meio-tom pontilhado e preenchimento creme, nunca colorido.
  - Na peça: entra num canto ou "saindo" da moldura, menor que o título e sem cobrir o prato; com tracinhos de movimento verdes em volta e, no máximo, uma estrelinha. Exemplo aprovado: post "Arroz de Fraldinha" (Dia das Crianças, 12/10/2026), com o Xepinha de garfo na mão espiando do canto direito.
  - O bartender Diogo (gravura realista com meio-tom) só aparece em peça de coquetelaria e, mesmo assim, o Xepinha continua presente.
- **Nunca:** cores fora da paleta, gradiente, 3D, foto-realismo colorido, sombra suave, brilho, estética "IA polida".

### Prompt pronto (colar no ChatGPT / gerador de imagem)
**pt-BR**
> Ilustração no estilo de gravura (linogravura/xilogravura leve) para o restaurante XEPA: traço de nanquim irregular feito à mão, hachura cruzada e meio-tom pontilhado nas sombras, apenas duas cores chapadas — traço verde musgo #3d4c3b (ou verde #3c8e6c) sobre preenchimento creme #fefceb —, fundo branco liso, sem gradiente, sem sombra suave, sem 3D, sem brilho. Opcional: explosão/sunburst creme atrás do objeto. Objeto centralizado, frontal ou levemente de cima, com bastante respiro. Estética elegante e sóbria de cardápio vintage. Personagem obrigatório: o XEPINHA, mascote do XEPA — desenho animado dos anos 1930 (rubber hose), cabeça grande, topete volumoso, olhos grandes ovais, sorriso largo com a língua de fora, luvas de desenho animado —, no mesmo traço verde com meio-tom, interagindo com o tema e sem cobrir o prato; não invente outro personagem. Tema: [DESCREVA O PRATO/OBJETO]. Siga exatamente o traço das imagens de referência anexadas e o desenho do Xepinha.

**English**
> Engraving-style illustration (light linocut/woodcut look) for the XEPA restaurant: irregular hand-drawn ink line, cross-hatching and stippled halftone in the shadows, only two flat colors — moss green line #3d4c3b (or green #3c8e6c) over cream fill #fefceb — on a plain white background; no gradients, no soft shadows, no 3D, no gloss. Optional cream sunburst behind the subject. Subject centered, frontal or slightly from above, generous white space. Elegant, sober vintage-menu aesthetic. Mandatory character: XEPINHA, the XEPA mascot — a 1930s rubber-hose cartoon with a big head, voluminous quiff, large oval eyes, wide grin with tongue out and cartoon gloves — in the same green halftone line, interacting with the subject without covering the dish; never invent another character. Subject: [DESCRIBE THE DISH/OBJECT]. Match the line work of the attached reference images and the Xepinha design exactly.

**Anexar junto:** `marcas/xepa/kv/referencias-estilo/xepa-traco-jamon-zoom.jpg`, `marcas/xepa/kv/referencias-estilo/xepa-traco-diogo-zoom.jpg`, `marcas/xepa/kv/referencias-estilo/xepa-traco-cavalo-prato.jpg`, `marcas/xepa/kv/referencias-estilo/xepa-layout-caixa-faixa-pontilhado.jpg` (para peças com layout).

## Assets (`marcas/xepa/`)
- `logos/xepa-logo-verde.png`: logo verde texturizado (transparente, 2000 px) · `logos/xepa-logo.png`: versão musgo.
- `kv/moldura-caixa.png`: moldura fina com cantos em degrau (transparente) · `kv/faixa-verde.png`: faixa de destaque (transparente).
- `kv/textura-papel-menu.jpg`: papel do cardápio, leve (fundo).
- Ilustrações (transparentes): `kv-cavalo5.png` (lettering verde), `kv-cavalo4.png` (lettering branco, para faixa verde), `kv-cavalo6.png` (prato verde), `kv-cavalo7.png` / `kv-cavalo9.png` (prato musgo/creme), `kv-copos2.png` (copos brindando, verde garrafa), `kv-geleia.png` (geleia de jalapeño), `kv-perfeito.png` (selo Hambúrguer Perfeito), `kv-DIOGRO.png` (Diogo), `ilustra-jamon-abuela.png`, `ilustra-copinho-salvia.png`, `ilustra-xepinha-cabeca-branco.png` (para pôr sobre verde).
- Campanha de aniversário (menta + preto): `kv-trio.png`.
- Referências: `kv/referencia-cardapio-comidas.jpg`, `kv/referencia-cardapio-drinks.jpg`, `kv/referencias-estilo/`.
- Fora do KV (histórico, não usar): `_fora-do-kv/` (ver LEIAME).

## Regras rápidas
- Ilustração no XEPA = Xepinha. Sem o Xepinha, a ilustração está errada.
- Claro, sóbrio, elegante. Se a peça parece "festa", está errada (exceto campanha de aniversário).
- Fotos de comida: luz natural quente, fundo neutro claro; nunca fundo colorido.
- Não usar o amarelo do Grupo, o vermelho/azul do OPCV nem o rosa do XEPA CONVIDA (o Convida tem KV próprio: `/kv-xepa-convida`).
