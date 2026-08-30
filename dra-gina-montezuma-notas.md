# Site — Dra. Gina Montezuma

Arquivo da página: `dra-gina-montezuma.html`.
Design system de referência (absorvido da Higiia): `design-system-higiia.md`.

## Como este site foi feito
1. Pedido: replicar a identidade visual de higiia.com.br e aplicar no site
   da Dra. Gina Montezuma (link original em manus.im).
2. Não foi possível acessar `higiia.com.br` nem `manus.im` diretamente —
   este ambiente tem bloqueio de rede para domínios externos (só a busca
   funciona, sem trazer HTML/CSS real). O usuário então enviou 6 screenshots
   do site da Higiia (desktop), a partir das quais o design system foi
   reconstruído "no olho" — ver limitações no fim de `design-system-higiia.md`.
3. Não havia nenhuma informação sobre a Dra. Gina Montezuma (especialidade,
   cidade, CRM, procedimentos, fotos, telefone, bio) — nada disso foi
   inventado como fato. Por analogia ao site de referência (clínica de
   estética/cirurgia plástica), assumimos provisoriamente "Medicina Estética
   e Bem-Estar" como especialidade, mas isso **precisa ser confirmado**.

## O que foi replicado da Higiia
- Paleta brass/dourado sobre branco e "sand" (bege claro), tipografia serifada
  elegante (Fraunces) + sans-serif geométrica em caixa alta (Poppins).
- Estrutura de seções: hero cheio + linhas em arco decorativas, barra de
  estatísticas logo abaixo do hero, colagem de fotos na seção "Sobre", grid
  de cards de procedimento com foto+gradiente, carrossel de depoimentos com
  iniciais, grid de conteúdo social estilo Reels, formulário de contato em
  campos pílula, seção de credenciais do profissional, botão flutuante de
  WhatsApp.
- Botões pílula (preenchido brass / contorno brass), a mesma lógica de CTA
  de baixo compromisso ("agende sua consulta"), não venda direta.

## Decisão importante: sem fotos e sem depoimentos fabricados
Não há ferramenta de geração de imagem disponível neste ambiente (o usuário
sugeriu Higgsfield, mas não está integrado aqui). Em vez de usar fotos de
banco de imagens fingindo ser a Dra. Gina, o consultório ou pacientes reais
— o que seria enganoso num site médico — todos os espaços de foto foram
substituídos por **blocos de placeholder visualmente integrados ao design**
(borda tracejada + ícone de câmera + instrução), fáceis de identificar e
trocar depois.

Pela mesma razão, a seção de depoimentos usa uma estrutura de exemplo
(iguais às iniciais "L.R" da Higiia), claramente marcada como placeholder.
Depoimento fabricado atribuído a paciente real é falta ética grave e pode
configurar propaganda enganosa perante o CFM — por isso a página traz um
aviso (`.tbd-box`) recomendando remover a seção até haver depoimentos reais
e autorizados.

## Como identificar o que falta preencher
No HTML, procure por:
- `.tbd` — texto inline com sublinhado tracejado dourado: passe o mouse
  (`title`) para ver o que precisa ser confirmado/trocado.
- `.tbd-box` — caixas com borda tracejada e aviso maior, para decisões que
  exigem mais contexto (ex.: depoimentos, procedimentos oferecidos).
- `WHATSAPP_NUMERO` no `<script>` final — hoje é um placeholder
  (`55XXXXXXXXXXX`), o botão flutuante e o formulário de contato não vão
  funcionar de verdade até ele ser trocado pelo número real.

## PENDENTE (para a Dra. Gina / responsável preencher)
- [ ] Nome de tratamento correto e especialidade real (confirmar se é
      medicina estética, dermatologia, ginecologia, outra).
- [ ] CRM (obrigatório em publicidade médica) e RQE, se houver.
- [ ] Cidade/endereço do consultório.
- [ ] WhatsApp/telefone real para contato.
- [ ] Lista real de procedimentos/especialidades oferecidos.
- [ ] Bio profissional (formação, trajetória) — sem inventar títulos.
- [ ] Fotos reais (dela, do consultório, opcionalmente de pacientes com
      autorização) para substituir os blocos placeholder.
- [ ] Depoimentos reais e autorizados, ou remoção da seção enquanto não houver.
- [ ] Conteúdo social real (posts/reels) ou remoção da seção "Acompanhe nas
      redes sociais".
- [ ] Respostas reais para o FAQ (primeira consulta, pagamento, endereço).

## Próximos passos sugeridos
- Depois que a Dra. Gina confirmar os pontos acima, dá para rodar o
  `construtor-de-pagina-lp` ou `detetive-de-nicho` para refinar copy e
  posicionamento, se fizer sentido para o objetivo do site (institucional
  vs. página de conversão).
