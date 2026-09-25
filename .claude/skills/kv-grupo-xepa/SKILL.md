---
name: kv-grupo-xepa
description: Identidade visual (KV) do Grupo XEPA, a marca-mãe de XEPA, Ó Pro Cê Vê e Xodó. Use ao criar ou revisar qualquer peça, página, tela do Sistema XEPA, e-mail, apresentação ou material institucional do grupo (site xepa.cc, vagas, jornalzinho, relatórios). Traz cores, fontes, logos, tom de voz e regras de uso.
---

# KV · Grupo XEPA

Grupo gastronômico de São Paulo (desde 2023). Três casas com voz própria que "falam a mesma língua":
**XEPA** (parrilla, burger e coquetelaria), **Ó Pro Cê Vê** (boteco mineiro) e **Xodó** (comida brasileira do dia a dia).
Marcas em desenvolvimento: **Hambúrguer do Xepinha** e **Xuxuzin** (bolo & pão de queijo).

Assets: `marcas/grupo-xepa/` · tokens prontos: `marcas/grupo-xepa/tokens.css`

## Essência e tom de voz
- Manifesto: *"Fogo, boteco & comida de verdade — restaurantes que são cultura."*
- Restaurante é **plataforma multicultural**, não só ponto de venda.
- Tom: direto, caloroso e orgulhoso, sem pompa. Frases curtas. Português do dia a dia.
- Provas que o grupo usa: **#1 Burger de SP (2025)**, **#1 Boteco de SP, voto popular (2026)**, 3 casas.
- Fundador: Lierson Mattenhauer Jr. Chefs sócios: Bruno Perial (OPCV) e Cauê Xóris (Xodó).

## Cores
| Token | Hex | Uso |
|---|---|---|
| `--green-900` | `#12291c` | fundo principal escuro, barras, botões |
| `--green-700` | `#23503a` | fundo secundário, barras de gráfico |
| `--green-500` | `#3c7a57` | apoio, estados positivos |
| `--cream` | `#f1e8d2` | texto sobre verde, fundos claros |
| `--yellow` | `#f4c430` | destaque, números grandes, CTA secundário |
| `--red` | `#e2553d` | alerta, marcação "hoje", meta |
| `--ink` | `#14201a` | texto sobre claro |
| `--muted` | `#5c6a60` | legendas |

Cor de cada casa dentro da marca do grupo: XEPA `#3f9a6a` · OPCV `#4d8db3` · Xodó `#f4c430` (com `#1f5a2e`).

## Tipografia (Google Fonts)
- **Anton**: títulos em caixa alta, números grandes (`--display`).
- **Fraunces itálico**: subtítulos charmosos logo abaixo do título (`--serif`).
- **DM Sans**: texto corrido e interface (`--sans`).

Padrão de título: `ANTON CAIXA ALTA` + linha de baixo em *Fraunces itálico* verde.

## Logos e imagens
- Logos das casas no site: Builderall CDN (ver `marcas/README.md`, seção "Logos no CDN").
- `imagens/grupo-xepinha-logo.png`, `grupo-xepinha-kv.webp`, `grupo-xepinha-mascote.webp`, `grupo-xepinha-sacola.webp`: Hambúrguer do Xepinha.
- `imagens/grupo-xuxuzin-logo.png`: Xuxuzin.
- Assinatura do chef: `https://www.mattenhauer.com/img/assinatura-clara.png`.

## Regras
- Cantos arredondados generosos (`--radius: 22px`, cards 22–26px, botões pílula).
- Fundo creme `#f6f1e4` / `#faf5ea` com cards brancos; blocos de destaque em verde-escuro com gradiente radial (`#2b5a40` → `#12291c`).
- Amarelo é destaque, não fundo de página inteira.
- Nunca misturar a paleta de uma casa com a de outra na mesma peça; na peça do grupo, cada casa aparece só com sua cor de assinatura.
- Acessibilidade: texto creme sobre verde-escuro e tinta sobre creme (contraste AA).
