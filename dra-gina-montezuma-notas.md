# Site — Dra. Gina Montezuma (v2.1 — pronta para apresentação)

**Status:** QA visual feito (screenshot em desktop 1440px e mobile 390px via
Chromium headless). Dois bugs reais encontrados e corrigidos nessa
passada: botão "Solicitar informações" do menu com texto invisível
(branco sobre branco) e foto real ainda não ligada no bloco de colagem da
seção "Sobre". Site está pronto para ser mostrado à Dra. Gina como
material de revisão — os pendentes abaixo (endereço, instituição de
docência, aprovação final de texto) continuam em aberto, mas nada bloqueia
a apresentação.


Arquivo da página: `dra-gina-montezuma.html`.
Design system de referência (absorvido da Higiia): `design-system-higiia.md`.
Foto: ver `assets/README.md`.

## O que mudou da v1 para a v2
A v1 foi feita sem nenhuma informação real sobre a Dra. Gina (só o link do
manus.im, inacessível). Nesta passada o usuário enviou 5 documentos reais
(diagnóstico e plano de melhoria do Instagram, estratégia de tráfego pago,
roteiros de conteúdo já aprovados, brief de homepage) e uma foto real dela.
A página foi reconstruída em cima desses documentos — todo texto abaixo tem
origem rastreável, nada foi inventado.

## Fatos confirmados (usados no site)
- **Nome:** Dra. Gina Montezuma
- **Formação:** Cirurgiã-dentista, Mestre em Ortodontia, Especialista em
  Harmonização Orofacial (HOF)
- **Registro:** CRO-CE 5039
- **Cidade/atendimento:** Fortaleza-CE (privado)
- **Outras frentes:** docência, gestão da qualidade/liderança em serviços
  públicos de saúde (trajetória institucional — não usada como endosso
  comercial, conforme exigido pelos próprios documentos), nova frente de
  cursos/capacitações/mentorias em preparação (sem data confirmada)
- **Instagram real:** [@dra.ginamontezuma](https://www.instagram.com/dra.ginamontezuma/)
  — usado como link real na seção "Conteúdo" e no rodapé
- **Posicionamento-âncora** (citado quase literalmente no hero/sobre):
  "A Dra. Gina ajuda pessoas a compreenderem possibilidades de cuidado
  odontológico individualizado, com planejamento, experiência clínica e uma
  visão integrada de técnica, organização e responsabilidade."

## Textos reaproveitados dos roteiros já aprovados
Boa parte da copy (Sobre, Diferencial "Técnica, gestão e cuidado não são
áreas separadas", FAQ, nota de privacidade no formulário, mensagem padrão
do WhatsApp) foi adaptada diretamente dos roteiros de Instagram que já
passaram pelo mesmo processo de research/estratégia — não são textos novos
e não testados, são a mesma voz de marca já desenhada para ela, só
reformatada para site. Mesmo assim, os documentos da própria Dra. Gina são
explícitos: **"Antes de publicar, a Dra. Gina deve revisar todo conteúdo
técnico, confirmar dados curriculares e aprovar imagens, legendas e
chamadas."** Esse site não é exceção — precisa da revisão dela antes de ir
ao ar.

## Decisão sobre a paleta — resolvida
O pedido original do usuário foi replicar a identidade visual da Higiia
(dourado/brass sobre branco e areia), enquanto os próprios documentos de
estratégia da Dra. Gina recomendavam outra direção (verde profundo/azul-
petróleo). O usuário confirmou manter o dourado da Higiia — e depois pediu
para tirar até o tom esverdeado que eu tinha deixado só no gradiente do
hero (como aceno à sugestão de marca dela). Removido: o hero agora usa o
mesmo cinza-carvão neutro da Higiia (`#2b2b2b` → `#6b6b66`), sem nenhum
verde na página além do ícone padrão do WhatsApp. Paleta 100% Higiia,
decisão final.

## Regras de compliance aplicadas (Resolução CFO-196/2019, citada nos docs)
- Sem imagem de antes/depois, sem imagem de procedimento/transcurso.
- Sem "resultado garantido", "transformação garantida" ou linguagem de
  urgência/medo — CTAs usam "Solicitar informações", "Conhecer a proposta".
- Sem depoimento de paciente sem autorização por escrito — por isso **não
  há seção de depoimentos** (foi removida da v1; não existe conteúdo
  autorizado para usar).
- Identificação profissional (nome + CRO-CE 5039) presente no rodapé e na
  seção de autoridade.
- Cargo institucional (gestão pública) tratado só como trajetória de
  carreira, nunca como selo comercial da prática privada.
- Formulário de contato avisa explicitamente para não enviar foto/exame/
  dado clínico na primeira mensagem — texto vem direto do roteiro aprovado
  de mensagem inicial de WhatsApp.

## O que ainda falta (bem mais curto que na v1)
- [x] ~~WhatsApp real~~ — confirmado pelo usuário: `55 85 99050679`, já
      ativo no botão flutuante e no formulário de contato.
- [x] ~~Decisão de paleta~~ — confirmado manter o dourado da Higiia.
- [x] ~~Foto real salva como arquivo~~ — resolvido. O arquivo original
      (14,76 MB) foi enviado pelo usuário via GitHub (sem querer, numa
      branch de outra tarefa: `claude/criar-pagina-uj82bj`), recuperado de
      lá e salvo em `assets/gina-retrato.jpg` já redimensionado/otimizado
      para web (1200×1800, ~244 KB, sem EXIF). Aparece automaticamente no
      hero e na seção de autoridade.
- [ ] **Endereço do consultório** em Fortaleza-CE (usado no FAQ, ainda placeholder).
- [ ] **Confirmar instituição(ões) de docência** — os documentos mencionam
      docência mas não citam a instituição específica.
- [ ] **Aprovação da Dra. Gina** sobre todos os textos técnicos/curriculares,
      conforme exigido pelos próprios documentos dela.
- [ ] **Conferir o número de WhatsApp**: `8599050679` tem 10 dígitos (DDD 85
      + 8 dígitos). Celular brasileiro com o 9º dígito teria 11 dígitos
      (DDD + 9XXXXXXXX). Pode ser um fixo/linha comercial válido — só
      sinalizando para conferir se não faltou um dígito na hora de digitar.

## O que foi deliberadamente removido/não incluído
- Seção de depoimentos (sem consentimento por escrito disponível).
- Grid de "conteúdo social" fake — substituído por um card real linkando
  para o Instagram verdadeiro dela.
- Números de anos/pacientes/procedimentos (nenhum foi fornecido) —
  substituídos por uma barra de "territórios de atuação" (HOF, Ortodontia,
  Odontologia individualizada, CRO-CE 5039), sem inventar estatística.
- Carrossel de equipe (ela atua sozinha na parte clínica, pelo que consta
  nos documentos) — virou seção única de autoridade/credenciais.
