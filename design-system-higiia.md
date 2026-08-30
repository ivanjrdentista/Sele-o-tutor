# Design System — Higiia Cirurgia Plástica (higiia.com.br)

Absorvido a partir de screenshots enviadas pelo usuário (não foi possível
acessar o site ao vivo neste ambiente — rede bloqueada para domínios
externos). Documento serve de referência para replicar o mesmo padrão de
qualidade em outros sites.

## 1. Personalidade da marca
Clínica de cirurgia plástica premium, 28 anos de tradição, multidisciplinar
(cirurgiões plásticos, otorrino, bariátrica, capilar, nutrição, dermato).
Tom: elegante, sóbrio, caloroso — não é "clínica fria", é "resultado com
confiança". Autoridade construída por números (anos, pacientes, cirurgias),
não por adjetivos.

## 2. Paleta de cores
| Token | Hex aprox. | Uso |
|---|---|---|
| `--brass` | `#AD8A52` | botões primários, números "+", ícones "+", detalhes |
| `--brass-dark` | `#8F6F3E` | hover/estado ativo do brass |
| `--ink` | `#1C1C1C` | títulos, texto de alto contraste |
| `--body` | `#5C5C5C` | parágrafos |
| `--muted` | `#767676` | legendas pequenas, labels de stats |
| `--paper` | `#FFFFFF` | fundo padrão das seções |
| `--sand` | `#EDEBE7` | fundo da barra de estatísticas e blocos alternados |
| `--line` | `#D8D5CF` | bordas finas (inputs, cards) |
| `--whatsapp` | `#25D366` | botão flutuante de WhatsApp |

Contraste alto entre texto branco e fotos escuras no hero (overlay
gradiente escuro por trás do texto para legibilidade).

## 3. Tipografia
- **Títulos (display):** serifada, elegante, levemente arredondada nas
  curvas (efeito "soft serif") — usada em "HIGIIA" (logo), "Sua beleza em
  harmonia.", "Nossa Clínica", "Cirurgias", "Nossos Pacientes", "Nossa
  equipe". Peso regular/medium, sem itálico no corpo principal.
  → Equivalente Google Fonts: **Fraunces** (ou Playfair Display como
  alternativa mais clássica).
- **UI / navegação / botões:** sans-serif geométrica, caixa alta, tracking
  largo (letter-spacing ~0.12em), peso médio. Usada no menu (HOME, NOSSA
  CLÍNICA…) e em todos os botões (AGENDE SUA CONSULTA, SAIBA MAIS, ENVIAR).
  → Equivalente: **Poppins** (peso 500).
- **Corpo de texto:** mesma família sans-serif, peso leve/regular (300–400),
  cor cinza (`--body`), line-height confortável (~1.7).

## 4. Elemento de assinatura visual
Linhas curvas finas (arcos concêntricos, estilo "onda"/"impressão digital"),
brancas translúcidas, sobrepostas à foto do hero, atrás do texto. É o
elemento gráfico mais distintivo da marca — repetível como marca d'água em
outras seções escuras.

## 5. Botões
- **Primário:** pílula (border-radius total), preenchido em `--brass`,
  texto uppercase, tracking largo, padding generoso (~16px 32px).
  Ex.: "AGENDE SUA CONSULTA", "ENVIAR".
- **Secundário:** pílula com borda `--brass` 1px, fundo transparente/branco,
  texto `--brass` uppercase. Ex.: "SAIBA MAIS", "TODAS CIRURGIAS".
- Sem sombras pesadas; transição suave (~0.2s) de cor/leve translação no
  hover.

## 6. Componentes recorrentes
- **Header fixo/transparente sobre o hero:** logo serifado à esquerda, nav
  uppercase ao centro-direita, CTA pill em brass à direita.
- **Barra de estatísticas** logo abaixo do hero: fundo `--sand`, 3 números
  grandes em brass ("+28", "+50.000", "+18.000") com legenda pequena cinza
  ao lado ("anos de clínica", "pacientes atendidos", "cirurgias
  realizadas"). Constrói autoridade antes de qualquer outro conteúdo.
- **Colagem de fotos sobrepostas** (seção "Nossa Clínica"): duas imagens
  retangulares desalinhadas sobre um bloco de textura neutra, criando
  profundidade.
- **Cards de procedimento/serviço:** foto full-bleed no card, gradiente
  escuro na base, título branco + link "SAIBA MAIS" sobre a foto.
- **Carrossel de depoimentos:** cards em fundo `--sand`, iniciais do
  paciente em negrito (privacidade: nunca nome completo), texto do
  depoimento, setas de navegação nas laterais.
- **Grid de conteúdo social:** thumbnails estilo Reels/Instagram com ícone
  de play e legenda sobreposta — usado para prova de autoridade educativa.
- **Formulário de contato:** campos em pílula com borda fina preta/escura,
  sem preenchimento cinza, placeholder discreto; botão "ENVIAR" pill cheio
  em brass, largura confortável.
- **Cards de equipe:** foto + nome (serifado) + especialidade + registro
  profissional (CRM/RQE) + ícone "+" circular em brass para expandir bio;
  carrossel horizontal com setas.
- **Botão flutuante do WhatsApp:** círculo verde padrão, fixo no canto
  inferior direito, visível em todas as seções.

## 7. Layout e espaçamento
- Container central com largura máxima ampla (~1240–1280px), bastante
  respiro lateral.
- Seções com padding vertical generoso (80–100px), fundo alternando entre
  branco e `--sand` para separar blocos sem precisar de linhas divisórias
  pesadas.
- Títulos de seção sempre curtos, serifados, alinhados à esquerda (exceto
  seções de fechamento/prova social, que centralizam).

## 8. O que este site "ensina" sobre credibilidade médica/estética
1. Números concretos logo no topo (tempo de atuação, volume de pacientes).
2. Prova social com iniciais reais, não depoimentos genéricos.
3. Conteúdo educativo (vídeos curtos) como prova de autoridade contínua,
   não só na hora da venda.
4. Registro profissional (CRM/RQE) exposto junto ao nome de cada médico —
   sinal de transparência regulatória, essencial em saúde.
5. CTA de baixo compromisso ("agende uma consulta"), nunca venda direta de
   procedimento na própria página.

## 9. Limitações desta absorção
- Feita a partir de 6 screenshots de desktop fornecidas pelo usuário —
  não foi possível abrir o HTML/CSS real do site (bloqueio de rede do
  ambiente), então cores e fontes acima são **aproximações visuais fiéis**,
  não valores extraídos do código-fonte.
- Não vimos: versão mobile, seção de FAQ (se existir), rodapé completo,
  página interna de cirurgia individual, formulário em estado de erro/êxito.
