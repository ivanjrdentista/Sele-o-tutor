# Site — Dra. Gina Montezuma (v2, com conteúdo real)

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

## Decisão sobre a paleta: possível tensão a resolver
O pedido original do usuário foi replicar a identidade visual da Higiia
(dourado/brass sobre branco e areia). Só que os próprios documentos de
estratégia da Dra. Gina recomendam outra direção visual para a marca dela:
> "Paleta: Off-white, areia clara, verde profundo ou azul-petróleo discreto
> e um tom terroso de acento. Tipografia serifada elegante para títulos e
> sans-serif limpa para texto informativo. [...] Evitar dentes, seringas,
> cruzes médicas ou azul-clínica como elementos dominantes."

Mantive a paleta dourada da Higiia porque foi o pedido explícito ("absorve
todo o design... implementa isso no site da Dra. Gina"), e ajustei o
gradiente do hero para um tom verde-acinzentado (mais próximo da sugestão
dela) só nessa área, como meio-termo. Se preferirem seguir 100% a
recomendação do documento de marca dela (verde profundo/azul-petróleo em
vez de dourado), é uma troca rápida de 3 variáveis CSS (`--brass`,
`--brass-dark`, `--brass-light` no início do arquivo) — me avisem qual
caminho seguir.

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
- [ ] **WhatsApp real** — nenhum dos 5 documentos continha o número; ainda é
      `55XXXXXXXXXXX` no `<script>` final do HTML.
- [ ] **Foto real salva como arquivo** — recebida no chat, mas este ambiente
      não permite salvar a imagem em disco a partir de uma mensagem. Ver
      `assets/README.md`: basta colocar o arquivo em `assets/gina-retrato.jpg`
      que ele aparece automaticamente no hero e na seção de autoridade
      (já tem fallback elegante em CSS enquanto o arquivo não existe).
- [ ] **Endereço do consultório** em Fortaleza-CE (usado no FAQ, ainda placeholder).
- [ ] **Confirmar instituição(ões) de docência** — os documentos mencionam
      docência mas não citam a instituição específica.
- [ ] **Aprovação da Dra. Gina** sobre todos os textos técnicos/curriculares,
      conforme exigido pelos próprios documentos dela.
- [ ] Decidir a questão da paleta (dourado Higiia vs. verde/petróleo da
      marca dela) — ver seção acima.

## O que foi deliberadamente removido/não incluído
- Seção de depoimentos (sem consentimento por escrito disponível).
- Grid de "conteúdo social" fake — substituído por um card real linkando
  para o Instagram verdadeiro dela.
- Números de anos/pacientes/procedimentos (nenhum foi fornecido) —
  substituídos por uma barra de "territórios de atuação" (HOF, Ortodontia,
  Odontologia individualizada, CRO-CE 5039), sem inventar estatística.
- Carrossel de equipe (ela atua sozinha na parte clínica, pelo que consta
  nos documentos) — virou seção única de autoridade/credenciais.
