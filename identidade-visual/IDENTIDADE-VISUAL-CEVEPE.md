# Identidade Visual — CEVEPE (Centro Veterinário de Petrolina)

> **Para o Claude:** este arquivo é a **fonte da verdade da identidade visual do CEVEPE**.
> Quando o Rafael disser *"pega a identidade visual do CEVEPE"* ou *"faz na identidade do CEVEPE"* —
> para qualquer peça (post, carrossel, roteiro, documento, capa, relatório) — reproduza exatamente
> os tokens, a tipografia e os padrões de componente abaixo.
> As cores foram amostradas direto do logo oficial (1080px) e das artes do perfil `@clinica_cevepe`.
> Para impressão/vetor, peça sempre o arquivo oficial do logo à designer (Gessica).

---

## 1. Marca

| Campo | Valor |
|---|---|
| Nome completo | **CEVEPE — Centro Veterinário de Petrolina** |
| Assinatura / logotipo | **cevepe** (minúsculas, bold arredondado e encorpado) + tagline *centro veterinário de petrolina* |
| Símbolo | **Oval verde** (anel aberto) com um **swoosh verde** embaixo, envolvendo um **cluster de animais em traço grafite** — avestruz, cabra, cavalo, cão e gato. Representa o cuidado com **todos** os animais. |
| Segmento | Clínica veterinária **24h** — + Pet Shop, Farmácia, Banho e Tosa, Cirurgia, Exames |
| Local | Petrolina · PE |
| Posicionamento | "Cuidando de quem você ama" — cuidado completo, humano e acessível, há **30 anos** |
| Instagram | `@clinica_cevepe` · linktr.ee/cevepeclinica |
| Contato | Urgência (87) 98814-1272 · WhatsApp 87 98825-3766 · atende **24h** |

### Regras de uso do logo
**Pode:** manter área de proteção (mín. = altura do oval do símbolo); usar sobre fundo branco (versão principal); usar a versão monocromática branca sobre fundos verde-pinho ou grafite; reduzir mantendo a legibilidade da tagline (abaixo de ~120px de largura, **omitir a tagline**).
**Não pode:** distorcer/inclinar/mudar proporção; trocar o verde por outro tom; recolorir os animais; aplicar sombra/contorno/brilho; reescrever "cevepe" em outra fonte; colocar sobre fundo de baixo contraste sem um "respiro" branco/claro.

---

## 2. Cores (tokens)

```css
:root{
  /* Verdes — assinatura CEVEPE */
  --verde:        #84C127;  /* verde-folha do logo · COR PRINCIPAL da marca */
  --verde-dark:   #5E9016;  /* botões pressionados, fim de gradiente */
  --verde-pinho:  #00483C;  /* verde escuro · fundos hero, faixas escuras */
  --lima:         #7BDB0F;  /* lima vibrante · realces, CTAs, números, destaques nas artes */
  --verde-xlight: #EDF6DA;  /* fundos leves, tags, blocos de apoio */

  /* Neutros */
  --grafite: #37423F;  /* wordmark, títulos, texto forte (cor dos animais do logo) */
  --ink:     #1D2320;  /* texto principal */
  --cinza:   #6A716E;  /* texto secundário */
  --linha:   #E4E9E0;  /* bordas e divisórias */
  --bg:      #FFFFFF;  /* fundo base */
  --bg-soft: #F5F8EF;  /* seções alternadas (verde levíssimo) */
}
```

| Papel | Cor |
|---|---|
| Cor principal da marca | `#84C127` (verde-folha) |
| Realce / CTA / número | `#7BDB0F` (lima vibrante) |
| Fundo escuro (hero) | `#00483C` (verde-pinho) |
| Texto sobre branco | `#1D2320` |
| Texto secundário | `#6A716E` |
| Texto sobre fundo escuro | `#FFFFFF` (corpo) / `#84C127` ou `#7BDB0F` (destaque) |

> **Acessibilidade:** o verde `#84C127` e o lima `#7BDB0F` **não** têm contraste suficiente para texto pequeno sobre branco — use-os em **blocos, ícones, números grandes e realces**, não em corpo de texto. Para texto, use `#1D2320`/`#37423F`.

---

## 3. Gradientes

```css
/* Hero — fundo verde-pinho com brilho verde (capas, topos de página, fundo de arte) */
background:
  radial-gradient(1100px 520px at 80% -10%, rgba(132,193,39,.45), transparent 60%),
  linear-gradient(155deg, #05231C 0%, #00332A 45%, #00483C 100%);

/* Marca — botões, faixas e pílulas sólidas */
background: linear-gradient(90deg, #84C127, #5E9016);

/* Realce — cards e destaques (do escuro pro verde) */
background: linear-gradient(135deg, #00483C 0%, #84C127 100%);
```

Sobre o hero escuro, aplicar uma **textura sutil** (patinhas/pontos ou grid a ~10% de opacidade branca), com máscara radial desvanecendo nas bordas. Manter o hero limpo — o protagonista é o pet/mensagem.

---

## 4. Tipografia

O wordmark do logo é um **display arredondado e encorpado** (minúsculas). Para o sistema (web, docs, posts), usar uma família amigável e legível que converse com essa redondeza.

- **Família principal (sistema):** `Poppins` (Google Fonts). Fallback `sans-serif`.
- **Família de destaque (opcional, "eco do logo"):** `Fredoka` ou `Baloo 2` — para títulos/headline que imitam a redondeza do "cevepe".
- Imports:
  `https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap`
  `https://fonts.googleapis.com/css2?family=Fredoka:wght@500;600;700&display=swap`

| Uso | Família / Peso | Tamanho ref. | Observações |
|---|---|---|---|
| Título de impacto (H1) | Fredoka 700 **ou** Poppins 800 | 40–58px | redondo, amigável; caixa baixa ok |
| Título de seção (H2) | Poppins 700 | 26–34px | |
| Subtítulo / destaque | Poppins 600 | 20–26px | |
| Corpo | Poppins **400** | 16px | `line-height:1.6`, arejado |
| Rótulo de seção / etiqueta | Poppins 700 | 12–13px | **MAIÚSCULAS**, `letter-spacing:.12em`, cor verde |

Hierarquia = peso + caixa + cor de rótulo. Corpo sempre regular (400); títulos encorpados (700–800).

---

## 5. Componentes

**Rótulo de seção** — traço curto verde + texto maiúsculo espaçado verde:
```css
.section-label{display:flex;align-items:center;gap:12px;font-size:13px;font-weight:700;
  letter-spacing:.14em;text-transform:uppercase;color:#5E9016}
.section-label::before{content:"";width:34px;height:3px;background:#84C127;border-radius:3px}
```

**Pílula / etiqueta** — contorno verde, cantos totalmente arredondados:
```css
.pill{border:1.5px solid #84C127;color:#4E7A12;border-radius:100px;padding:8px 16px;
  font-size:12px;font-weight:700;letter-spacing:.08em;text-transform:uppercase}
.pill.solid{background:linear-gradient(90deg,#84C127,#5E9016);color:#fff;border-color:transparent}
```

**Botão:**
```css
.btn{background:linear-gradient(90deg,#84C127,#5E9016);color:#fff;border-radius:12px;
  padding:12px 22px;font-weight:700}
.btn.ghost{background:transparent;color:#4E7A12;border:2px solid #84C127}
```

**Card de destaque** (fundo suave, rótulo verde em cima, número/ícone grande):
```css
.mini-card{border:1px solid #E4E9E0;border-radius:16px;padding:16px 18px;background:#F5F8EF}
.mini-card small{color:#5E9016;font-size:11px;font-weight:700;letter-spacing:.1em;text-transform:uppercase}
.mini-card b{font-size:22px;font-weight:800;color:#00483C}
```

**Swoosh (elemento gráfico da marca)** — o traço curvo verde do logo, reutilizável como sublinhado/divisória:
```html
<svg viewBox="0 0 240 24" fill="none" aria-hidden="true">
  <path d="M4 16 C 70 2, 170 2, 236 14" stroke="#84C127" stroke-width="6" stroke-linecap="round"/>
</svg>
```

**Raios de canto:** pílulas `100px` · cards/blocos `16–20px` · botões `12px` · detalhes `6px`.
**Bordas:** `1px solid #E4E9E0`. Sombras: usar com parcimônia; o sistema é limpo, definido por **cor e forma arredondada** (mais orgânico/amigável que o da Brito Mídias).

---

## 6. Layout

- Container central: `max-width` ~980–1100px, padding lateral 28px.
- Página típica: **hero verde-pinho** (gradiente + textura) no topo → seções em **fundo branco**, alternando com `#F5F8EF` (`.soft`) → **footer** `#00483C` ou `#1D2320`.
- Cada seção abre com um **rótulo de seção** verde (traço + maiúsculas), depois H2, depois um parágrafo de intro em `#6A716E`.
- Formas arredondadas em tudo (cards, fotos, botões) — combina com a redondeza do logo e o tom acolhedor.

---

## 7. Tom de voz

Clínica de bairro que virou referência: **acolhedora, próxima, bem-humorada e confiável.**
- **Acolhedor:** fala com quem ama o pet como parte da família ("quem você ama", "seu pet").
- **Próximo e regional:** jeito petrolinense, leve, sem formalidade fria. Humor nos vídeos (esquetes) é bem-vindo.
- **Cuidadoso e confiável:** informação correta de saúde animal, sem sensacionalismo; 24h, 30 anos de história, estrutura completa.
- **Chamada clara:** todo conteúdo leva a uma ação (agendar, salvar, visitar, WhatsApp).

**Regras de escrita das legendas** (padrão fechado com o Rafael):
- **Nunca** travessão (—) no corpo do texto. Frases mais longas e naturais, nunca curtas e secas em sequência (evita "cara de IA").
- Sempre **"condições especiais"**, nunca "desconto exclusivo".
- Estrutura: gancho/contexto → bloco da campanha vigente (ex.: SPA PET, um serviço por linha) → bloco dos 30 anos → `TAGS PARA SEO:` → `HASHTAGS`.
- Fecho padrão: `📲 Fale com a gente no WhatsApp · 📞 87 98825-3766`.

Português do Brasil. Emojis com moderação e sempre a serviço da leitura (patinhas, coração, serviços).

---

## 8. O logo (referência de construção)

Estrutura, de cima pra baixo:
1. **Oval verde** (`#84C127`), anel de traço grosso, ligeiramente aberto.
2. **Cluster de animais** em traço **grafite** (`#37423F`) dentro do oval: avestruz, cabra, cavalo, cão e gato.
3. Wordmark **`cevepe`** — minúsculas, bold arredondado, grafite.
4. **Swoosh verde** curvo sublinhando o wordmark.
5. Tagline **`centro veterinário de petrolina`** — grafite, peso regular, espaçada.

### Arquivos disponíveis (pasta `png/`)
| Arquivo | Conteúdo | Onde usar |
|---|---|---|
| `png/logo-cevepe.png` | Logo **colorido**, fundo **transparente** (447px) | Fundos claros (branco, verde suave). Versão principal. |
| `png/logo-cevepe-branco.png` | Verde mantido, **animais e texto em branco**, fundo transparente | Fundos escuros (verde-pinho, grafite). |

Versões ainda a pedir à designer (para impressão/alta qualidade):
- **Vetor oficial** (SVG/AI) — o cluster de animais é ilustração detalhada; para print, usar o vetor.
- **Reduzida:** só o símbolo (oval + animais) para avatar/ícone/carimbo.

> ⚠️ Os PNGs acima foram gerados removendo o fundo branco do logo oficial (447px) — ótimos para web/tela. Para **impressão grande**, peça o vetor. Não recriar o cluster de animais à mão.

---

## 9. Checklist rápido para qualquer peça nova

- [ ] Fonte Poppins (400 corpo / 700–800 títulos); Fredoka opcional nos headlines
- [ ] Verde `#84C127` como cor de marca; lima `#7BDB0F` só em realce; verde-pinho `#00483C` nos fundos escuros
- [ ] Neutros `#1D2320 / #6A716E / #E4E9E0`; nunca verde em corpo de texto pequeno
- [ ] Hero verde-pinho com gradiente + textura leve; seções brancas/`#F5F8EF`; footer escuro
- [ ] Cada seção com rótulo maiúsculo verde + traço; formas bem arredondadas
- [ ] Logo correto pro fundo (colorido no claro; branco no escuro); tagline some se ficar pequena
- [ ] Tom acolhedor, próximo e com chamada clara pra ação
