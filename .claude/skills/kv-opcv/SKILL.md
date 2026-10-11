---
name: kv-opcv
description: Identidade visual (KV) do Ó Pro Cê Vê (OPCV), boteco mineiro contemporâneo na Vila Buarque (São Paulo), do Grupo XEPA. KV = EXATAMENTE a estética das peças do Thobias (cartaz serigráfico em papel creme, vermelho + azul + teal, sobreposição de tinta, títulos com sombra azul-clara). Use ao criar posts, cartazes, rótulos, cardápios, ilustrações ou qualquer peça do OPCV. Traz paleta medida nos PSDs, fontes exatas e alternativas, 4 modelos de peça com medidas, guia de estilo de ilustração, prompt pronto (pt-BR/EN) e referências para anexar.
---

# KV · Ó Pro Cê Vê (OPCV)

**Boteco mineiro contemporâneo** · a boemia de Belo Horizonte na Vila Buarque. **Melhor boteco de SP, voto popular 2026.**
Chef e sócio: Bruno Perial. Instagram: **@opcv.uai** · Endereço: **R. Jaguaribe, 520 - Vila Buarque, São Paulo**.

Assets: `marcas/opcv/` · tokens prontos: `marcas/opcv/tokens.css`
Fonte da verdade (11/10/2026): as peças do **Thobias** em Drive falecomxepa `GRUPO XEPA/OPCV/MARCA/2026/POSTS/` (`post1.psd` a `post4.psd`, `rotulo_03.pdf`). Os PSDs não vão para este repositório público (peça ao Grupo XEPA).

> Pedido do dono: **"atualizar o KV para ficar EXATAMENTE o que o Thobias criou, exatamente essa estética"** e **"quando for pedida uma ilustração ou qualquer coisa, respeitar EXATAMENTE esse estilo e traço igual das peças do KV; precisa ser idêntico ao estilo que o Thobias aplicou"**.

## Essência e tom de voz
- Baixa gastronomia com orgulho: pratos clássicos, receitas populares, memória afetiva. Comida direta, honesta, pra compartilhar.
- Ritual: pão de queijo de verdade, estufa cheia, cachaça mineira, cerveja no **copo lagoinha**, chopp gelado.
- Tom: mineirês de balcão, bem-humorado e curto. Bordões: *"Vem tomar uma no OPCV"*, *"uai, sô!"*, *"Fiado só amanhã"*, *"tem base um trem desse não"*. Piada de horário: *"das 12h00 às 12h00"*.

## Paleta (medida nas camadas dos PSDs · "impresso" = depois da textura de papel)
| Token | Tinta (HEX) | Impresso | Uso |
|---|---|---|---|
| `--opcv-papel` / `--opcv-creme` | `#f6f6ea` | `#edebdc` | fundo de papel; tinta creme de textos e formas sobre azul/teal/vermelho |
| `--opcv-vermelho` | `#ea4136` | `#e24a3f` | títulos, script, OPCV gigante, endereço sobre creme |
| `--opcv-vermelho-ilustra` | `#f3433b` | — | serigrafia das ilustrações (copos, copo lagoinha), canto "Hoje tem", selo OPCV |
| `--opcv-azul` | `#17a4de` | — | objeto em serigrafia azul (garrafa) |
| `--opcv-azul-fundo` | `#00abe3` | `#16a9d4` | fundo azul chapado (modelo D) |
| `--opcv-azul-moldura` | `#2d92b4` | `#4499ae` | moldura azul (modelo B) |
| `--opcv-teal` | `#378793` | `#40878d` | faixa inferior verde-azulada (modelo C) |
| `--opcv-azul-claro` | `#71c7cb` | `#79c0bf` | sombra deslocada dos títulos; cópia atrás do selo OPCV |
| `--opcv-amarelo-cerveja` | `#ffdb3f` | `#f7d24e` | **só** o líquido da cerveja |
| `--opcv-sobreposicao` | `#353a3d` | — | não é tinta: é o quase-preto que nasce quando o azul cruza o vermelho em multiply |
| Rótulo | `#e33226` / `#40a2b1` / `#f7f5ef` | — | embalagem "Pão de queijo tradicional" (vermelho, azul-petróleo, creme) |

**Regra de cor:** cada peça usa **papel creme + 1 cor de fundo/estrutura + vermelho** (no máximo 3 tintas + creme). Amarelo só dentro do copo. Nunca verde (é do XEPA/Xodó), nunca preto puro como tinta, nunca gradiente.

## Tipografia (nomes exatos das camadas de texto dos PSDs)
| Camada nos PSDs | Onde aparece | Alternativa livre | Regra |
|---|---|---|---|
| **ModestoCondensed** (Modesto Condensed, Parkinson Type / Adobe Fonts) | "NESTA QUINTA", "12:00 / 00:00", "FRANGO com QUIABO", endereço | **Alfa Slab One** (títulos) · **Oswald** (endereço) | CAIXA ALTA; títulos com sombra azul-clara dura; "com" menor (≈50%) entre palavras grandes; endereço com tracking 210 |
| **NewstarRegular** (Newstar) | "DOMINGO", "12h00", "KAOL e / FRANGO com QUIABO" | **Archivo Black** | CAIXA ALTA, tracking +10; "e"/"com" pequenos (≈65%) |
| **SinkRegular** (Sink) | um "12h00" do post Domingo | **League Gothic** | números condensados |
| **StoryScript-Regular** (Story Script, Google, OFL) | "Vem tomar uma no", "das / as / até", "até o horário de almoço", "Hoje tem" | **a mesma** (Google Fonts) | caixa baixa ou alta, tracking -30 a -70, sempre em vermelho ou creme |
| **Futura-CondensedMedium** (Futura Condensed Medium) | endereço em 2 linhas do post 1 | **Oswald 500** | 1ª linha grande (100%), 2ª linha 70% |
- **Lettering em imagem** (não é fonte, usar o PNG): "Ó PRO CÊ VÊ" arqueado (`kv/elementos/o-pro-ce-ve-arqueado.png`), "OPCV" gigante arqueado (`opcv-gigante-vermelho.png`), selo OPCV Belo Horizonte–São Paulo (`selo-opcv-bh-sp.png`), "CHOPP EM DOBRO" (`titulo-arqueado-chopp-em-dobro.png`, exemplo de título arqueado creme).
- **Arqueamento:** títulos grandes vêm em arco convexo suave (sobe no centro) ou em arco ascendente (modelo D). Script nunca arqueado.
- **Sombra do título** (PSD: Sombra Projetada normal 100%, cor `#71c7cb`, ângulo 123°, distância 8 px, tamanho 0): cópia **dura**, deslocada **≈0,25% da largura para a direita e ≈0,35% para baixo**, sem desfoque. CSS: `text-shadow: 4px 7px 0 #71c7cb` (canvas 1900 px).
- Fontes comerciais (Modesto Condensed, Newstar, Sink, Futura Condensed) **não estão no repositório**: Modesto Condensed está no Adobe Fonts (conta Creative Cloud); Newstar e Sink precisam de licença; Futura vem no macOS.

## Acabamento obrigatório (todas as peças · camadas do topo dos PSDs)
1. **"Texture"**: preenchimento de padrão (grão de papel) em **Multiplicação, opacidade 50%**, sobre a peça inteira → `kv/elementos/textura-graos-multiply.jpg`.
2. **"Highlight"**: preenchimento de padrão em **Tela (Screen), opacidade 15%** → clareia levemente e dá o aspecto de papel impresso.
3. Objetos de serigrafia (copo, garrafa, copos de chopp) entram como **"Imagem Inserida" em Multiplicação**: onde cruzam outra tinta, escurecem (azul × vermelho ≈ `#353a3d`).
4. Fotos de prato: recorte em **Escurecer (Darken)** com **Curvas** e **Equilíbrio de Cores** clipados, para "assentar" no papel; sombra azul suave sob o prato (`sombra-azul-prato.png`, Multiplicação 72%). É a ÚNICA sombra suave permitida.
- Pronto: `kv/elementos/papel-creme-opcv.jpg` = creme `#f6f6ea` já com as duas camadas aplicadas (fica `#edebdc`).

## Os 4 modelos de peça (feed 4:5 · canvas original 1900 × 2385 px; % = posição/tamanho relativo ao canvas)

### Modelo A · "Vem tomar uma no OPCV" (objeto-herói em serigrafia sobre OPCV gigante) · ref. `kv/opcv_kv_post1.jpg`
- **Fundo:** papel creme liso, sem moldura.
- **Script** "Vem tomar uma no" (Story Script, vermelho, Multiplicação): centralizado, topo em 15%, altura ≈4% (x 30–70%).
- **OPCV gigante** arqueado em vermelho (`opcv-gigante-vermelho.png`, Multiplicação): largura 73% (x 14–87%), y 21–49%.
- **Objeto-herói** (garrafa) em serigrafia azul `#17a4de`, vertical, centralizado: largura 27%, altura 82% (y 9–91%); passa **por cima/por baixo** do OPCV e cria a sobreposição escura nas letras.
- **Objeto secundário** (copo lagoinha: traço vermelho `#f3433b` + cerveja amarela `#ffdb3f` com falhas) no canto inferior esquerdo, sobrepondo a base do herói: x 17–41%, y 62–89% (`copo-lagoinha-cerveja.png`).
- **Endereço** em 2 linhas, vermelho, Futura Condensed/Oswald, alinhado à esquerda do bloco em x 65–82%, y 82–87%: "R. Jaguaribe, 520" (100%) / "Vila Buarque, São Paulo" (70%).
- Marca de terceiro (cerveja patrocinadora) só com contrato; sem patrocinador, o herói é garrafa/copo **sem rótulo de marca** (rótulo com "OPCV" ou liso).

### Modelo B · "DOMINGO das 12h00 às 12h00" (moldura azul + oval creme + prato) · ref. `kv/opcv_kv_post2.jpg`
- **Fundo:** papel creme; **moldura azul** `#2d92b4` sangrando com borda creme irregular de ≈2% em volta (`moldura-azul.png`); filete creme fino a ≈4% da borda, acompanhando o retângulo.
- **Oval creme** central (`oval-creme.png`): x 11–89%, y 17–88%, com um segundo filete oval creme fino por fora.
- **"Ó PRO CÊ VÊ"** arqueado creme no topo, sobre o azul: x 31–69%, y 8–16%.
- **Título** "DOMINGO" (Newstar/Archivo Black, vermelho): x 31–69%, y 27,5–33%; **filete vermelho** logo abaixo, da largura do título (`filete-vermelho.png`).
- **Linha de horário**: "das" e "as" em Story Script (≈57% do tamanho) + "12h00" em Newstar/Sink, vermelho, y 35–41%, x 21–79%.
- **Prato** em foto recortada, centralizado, x 23–78%, y 44–66%, com a sombra azul suave por baixo.
- **Nome do prato** "KAOL e / FRANGO com QUIABO" (Newstar, 2 linhas, 2ª menor), vermelho, y 72–77,5%; filete vermelho; **"até o horário de almoço"** em Story Script vermelho, y 79,5–82%.
- **Endereço** em CAIXA ALTA espaçada (tracking 210), creme `#fff2f1`, sobre o azul abaixo do oval: centralizado, y 91–93%, altura de letra ≈1,6%.

### Modelo C · "NESTA QUINTA das 12:00 até 00:00" (papel + faixa teal com prato atravessando) · ref. `kv/opcv_kv_post3.jpg`
- **Fundo:** papel creme; **faixa teal** `#378793` ocupando de 65% até a base, largura total, com filete creme interno (`faixa-teal.png`).
- **Selo OPCV** arqueado vermelho com cópia azul-clara atrás, triangulinho vermelho entre dois filetes azul-claros embaixo e "Belo Horizonte" / "São Paulo" em script vermelho nas pontas (`selo-opcv-bh-sp.png`): x 36–62%, y 6–15%.
- **Título** em 2 linhas "NESTA / QUINTA" (Modesto Condensed/Alfa Slab One, vermelho, **sombra azul-clara dura**), levemente arqueado: x 25–75%, y 18–43,5%; cada linha ≈12,5% da altura.
- **Horário**: "das" e "até" em Story Script pequeno + "12:00" e "00:00" em Modesto (≈70% do título) com a mesma sombra: x 27–73%, y 45–52%.
- **Prato** em foto recortada **atravessando** a borda de cima da faixa (metade no papel, metade no teal): x 20–80%, y 54–71%.
- **Nome do prato** "FRANGO com QUIABO" creme sobre teal (Modesto Condensed, "com" ≈50%): x 17–83%, y 74–82%.
- **"— até o horário de almoço —"** Story Script creme entre filetes creme (`filete-creme.png`): y 84–87,5%.
- **Endereço** creme espaçado: y 90–91,5% · **fileira de losangos creme** (`losangos-creme.png`): y 94–96,5%, centralizada.

### Modelo D · "HOJE TEM CHOPP EM DOBRO" (fundo azul chapado + canto vermelho + copos em serigrafia) · ref. `kv/opcv_kv_post4.jpg`
- **Fundo:** azul chapado `#00abe3` sangrando com borda creme irregular de ≈1,5–2% (`fundo-azul-borda.png`).
- **Canto vermelho** triangular no topo esquerdo (≈34% da largura × 23% da altura) com **"HOJE TEM"** em Story Script creme na diagonal (≈-35°) e sublinhado em pincelada creme (`canto-hoje-tem.png`).
- **Título** creme arqueado ascendente: palavra principal grande ("CHOPP", Modesto-like serifado, ≈15% da altura) subindo para a direita + complemento menor ("EM DOBRO") descendo em arco à direita: x 19–84%, y 5–37% (`titulo-arqueado-chopp-em-dobro.png` como gabarito).
- **Objetos-herói** em dupla, brindando: dois copos em serigrafia vermelha `#f3433b` sobre corpo creme, inclinados para lados opostos (≈-10° e +15°), sobrepostos: copo 1 x 10–51%, y 25–75%; copo 2 x 41–90%, y 34–87%.
- **"Ó PRO CÊ VÊ"** arqueado creme: x 38,5–61,5%, y 88–92,7% · **endereço** creme espaçado: y 94–95,5%.

### Stories (9:16) e outros formatos
Mesma ordem vertical; ganhe altura aumentando o respiro entre título e objeto e descendo endereço/rodapé para os 8% finais. Mantenha 6% de margem segura no topo e na base.

### Embalagem · rótulo "Pão de queijo tradicional" · ref. `kv/rotulo-pao-de-queijo-referencia.jpg`
Fundo vermelho `#e33226` com moldura creme arredondada; "Ó PRO CÊ VÊ · desde 2025" pequeno no topo entre "BH" e "SP"; "PÃO DE QUEIJO" creme gigante com sombra azul-petróleo `#40a2b1` dura; "Tradicional" em script creme; foto dos pães com meio-tom; **xadrez de losangos** azul-petróleo/creme no rodapé.

## GUIA DE ESTILO DE ILUSTRAÇÃO (Thobias)
Análise das camadas dos PSDs e de recortes ampliados 2–3× das peças finais (`kv/referencias-estilo/`).

**Técnica: cartaz serigráfico/risográfico digital.**
- **Cores chapadas, sem gradiente**: cada objeto é UMA tinta (azul, vermelho, amarelo ou creme). Volume só com a tinta "vazando" ou falhando, nunca com degradê.
- **Sobreposição de tinta (overprint):** as camadas de objeto ficam em **Multiplicação**. Onde o azul cruza o vermelho nasce um quase-preto `#353a3d`; vermelho sobre amarelo fica vermelho mais quente. Esse cruzamento é intencional e é a assinatura do post A.
- **Falhas de tinta:** bordas com respingos e pontinhos soltos, áreas de cor com furos claros (bolhas da cerveja, gotas no copo), traço que afina e engrossa. Ver `opcv-zoom-copo-chopp-serigrafia.jpg` e `opcv-zoom-copo-lagoinha-serigrafia.jpg`.
- **Traço:** contorno à mão, irregular, espessura média (≈0,8–1,2% da largura do objeto), com cantos levemente arredondados e pontas "secas". Nada de contorno vetorial perfeito. Em objetos de vidro, o traço vermelho desenha só o contorno, o fundo do copo e 3–5 riscos verticais de reflexo.
- **Registro levemente fora:** a cor de preenchimento não coincide 100% com o traço (amarelo sai 1–2% do contorno do copo, creme do copo de chopp vaza para fora do vermelho).
- **Borda das áreas de cor:** irregular, "comida" pelo papel (moldura azul e fundo azul com borda creme rasgada). Ver `opcv-zoom-moldura-borda-irregular.jpg`.
- **Meio-tom:** só em fotos de produto/rótulo dentro do objeto (pães do rótulo, rótulo da garrafa) e no corpo dos copos (pontilhado vermelho que some para o creme).
- **Papel:** creme `#f6f6ea` com grão fino multiplicado (50%) e um véu claro (Screen 15%): tudo ganha a mesma textura, inclusive as fotos.
- **Luz/sombra:** não há luz modelada. Sem sombra projetada nos objetos ilustrados. Única sombra = cópia azul-clara dura atrás dos títulos (e a sombra azul suave sob fotos de prato).
- **Perspectiva e enquadramento:** objetos **frontais**, de lado ou levemente de cima, **grandes** (40–80% da altura da peça), às vezes cortados pela borda; dois objetos se sobrepõem em vez de ficarem lado a lado.
- **Escala texto × objeto:** o título ocupa 25–45% da altura; objeto-herói 40–80%; texto de apoio ≤5%. Título e objeto podem se cruzar (modelo A).
- **Número de cores por peça:** 3 tintas + papel (ex.: azul, vermelho, amarelo + creme no A; azul-moldura, vermelho + creme no B; vermelho, azul-claro, teal + creme no C; azul, vermelho + creme no D).
- **NUNCA:** 3D, gradiente, fotorrealismo dentro da ilustração, sombra suave nos objetos, brilho/reflexo especular, contorno vetorial limpo, cores fora da paleta (verde, roxo, preto puro, dourado), letras "neon", textura de papel envelhecido/manchado, estética "IA brilhante", fundo branco puro.

### Prompt pronto para ilustração/peça (o sistema cola automaticamente)
**pt-BR**
> Ilustração no estilo de cartaz serigráfico (silk-screen/risografia) do boteco Ó Pro Cê Vê, idêntica às imagens de referência anexadas. Cores chapadas e sem gradiente, só estas tintas: vermelho #EA4136, azul #17A4DE (ou azul #00ABE3 de fundo), azul-claro #71C7CB, teal #378793, amarelo #FFDB3F apenas para cerveja, sobre papel creme #F6F6EA com grão fino. Use no máximo 3 tintas além do creme. As tintas se sobrepõem em multiplicação: onde o azul cruza o vermelho fica quase preto (#353A3D). Traço de contorno feito à mão, irregular, com falhas de tinta, respingos, pontinhos soltos e registro levemente desalinhado entre preenchimento e contorno; meio-tom pontilhado só no corpo do objeto. Objeto frontal, grande, ocupando boa parte da peça, podendo ser cortado pela borda. Sem luz modelada, sem sombra suave, sem 3D, sem brilho, sem fotorrealismo, sem contorno vetorial perfeito, sem marcas de terceiros. Tema: [DESCREVA O OBJETO/PRATO/BEBIDA]. [Se for peça completa: siga o modelo (A/B/C/D) do KV, com título em CAIXA ALTA vermelho condensado serifado com sombra azul-clara dura deslocada para baixo à direita, texto de apoio em script vermelho e endereço "R. JAGUARIBE, 520 - VILA BUARQUE, SÃO PAULO" em caixa alta espaçada, formato 4:5.]

**English**
> Illustration in the silk-screen / risograph poster style of the Ó Pro Cê Vê bar, identical to the attached reference images. Flat colors, no gradients, only these inks: red #EA4136, blue #17A4DE (or background blue #00ABE3), light aqua #71C7CB, teal #378793, yellow #FFDB3F for beer only, on cream paper #F6F6EA with fine grain. Max 3 inks plus cream. Inks overprint in multiply: where blue crosses red it turns almost black (#353A3D). Hand-drawn irregular outline with ink dropouts, specks, splatter and slight misregistration between fill and outline; stippled halftone only inside the object. Subject frontal and large, filling most of the frame, may be cropped by the edge. No modeled lighting, no soft shadows, no 3D, no gloss, no photorealism, no clean vector outlines, no third-party logos. Subject: [DESCRIBE THE OBJECT/DISH/DRINK]. [For a full piece: follow KV layout (A/B/C/D), headline in red condensed wedge-serif ALL CAPS with a hard light-aqua drop shadow offset down-right, red script supporting text, address "R. JAGUARIBE, 520 - VILA BUARQUE, SÃO PAULO" in widely tracked caps, 4:5 format.]

**Anexar junto ao pedido (nesta ordem):**
1. `marcas/opcv/kv/referencias-estilo/opcv-zoom-copo-lagoinha-serigrafia.jpg` (traço, falhas, registro, amarelo)
2. `marcas/opcv/kv/referencias-estilo/opcv-zoom-sobreposicao-tinta-letras.jpg` (sobreposição azul × vermelho, grão)
3. `marcas/opcv/kv/referencias-estilo/opcv-zoom-titulo-sombra-azul.jpg` (título com sombra azul-clara)
4. A peça do modelo pedido: `marcas/opcv/kv/opcv_kv_post1.jpg` (A) · `post2` (B) · `post3` (C) · `post4` (D)
Extras: `opcv-zoom-copo-chopp-serigrafia.jpg`, `opcv-zoom-moldura-borda-irregular.jpg`, `opcv-zoom-faixa-teal-losangos.jpg`, `opcv-zoom-canto-hoje-tem.jpg`.

## Assets (`marcas/opcv/`)
- **Peças finais (referência):** `kv/opcv_kv_post1.jpg` (A), `kv/opcv_kv_post2.jpg` (B), `kv/opcv_kv_post3.jpg` (C), `kv/opcv_kv_post4.jpg` (D) · rótulo: `kv/rotulo-pao-de-queijo-referencia.jpg`.
- **Elementos reutilizáveis** (`kv/elementos/`, PNG transparente exportado das camadas do PSD, SEM a textura: aplique a textura por cima da peça montada):
  `papel-creme-opcv.jpg` (fundo pronto) · `textura-graos-multiply.jpg` (grão, usar em Multiplicação) · `moldura-azul.png` (B) · `oval-creme.png` (B) · `filete-vermelho.png` · `sombra-azul-prato.png` · `faixa-teal.png` (C) · `losangos-creme.png` (C) · `filete-creme.png` (C) · `selo-opcv-bh-sp.png` (C) · `fundo-azul-borda.png` (D) · `canto-hoje-tem.png` (D) · `titulo-arqueado-chopp-em-dobro.png` (D) · `o-pro-ce-ve-arqueado.png` (B/D) · `opcv-gigante-vermelho.png` (A) · `copo-lagoinha-cerveja.png` (A).
- **Referências de estilo** (`kv/referencias-estilo/`): recortes ampliados de traço, sobreposição, título, moldura, faixa e canto.
- `logos/`: `opcv-logo-menu.webp` ("Ó PRO CÊ VÊ" azul arqueado), `opcv-wordmark.webp` (creme), `opcv-belo-horizonte.png`, `opcv-sao-paulo.png`.
- `imagens/`: fotos da casa e dos pratos (`opcv-g-*.webp`, `opcv-prato-quiabo.webp`), chef `bruno-perial-oficial.webp`, cartazes do site `opcv-cartaz1–4.webp` (= peças A–D), copos/garrafa recortados (`opcv-amstel.webp`, `opcv-garrafa-copo.webp`: têm marca de terceiro, só usar com contrato do patrocinador), OG `opcv-og.jpg`.

## Regras rápidas
- Sempre papel creme com grão; sempre uma das 4 composições; sempre o endereço.
- Humor mineiro no texto; nunca formal nem "gourmet".
- Marca de cerveja/patrocinador só com contrato vigente e logo oficial; nas peças sem patrocínio, objetos sem marca.
- Não usar verde do XEPA/Xodó, nem as fontes do XEPA (Harmond, Brandon).
