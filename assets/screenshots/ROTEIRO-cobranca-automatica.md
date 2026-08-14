<!-- Roteiro de capturas — NÃO é página do manual. Excluído do build em _config.yml. -->

# Roteiro de capturas — Cobrança Automática (v7.110.x)

Quem captura: **Bruno**, com Playwright, na sessão autenticada dele.
Onde salvar: `docs-publicos/assets/screenshots/<nome>.png`
Viewport padrão: **desktop 1920×1080**. Onde a versão de celular importa, está dito.

Depois de salvar os arquivos, cada marcador `<!-- PRINT: nome — ver roteiro de capturas -->`
em `modulos/cobranca-automatica.md` deve ser trocado pela imagem:

```markdown
![Texto alternativo descritivo](/assets/screenshots/nome.png)
```

⚠️ **Dados fictícios.** As telas mostram nome, unidade, CPF e valor de morador. Capturar
no condomínio de teste (Residencial TESTE) e, quando houver dado pessoal visível, repetir
embaixo da imagem a legenda já usada em outras páginas:
*Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

---

## Telas do módulo

Todas em **Cobrança automática** (menu lateral), rota `/cobranca-automatica`, com o
condomínio de teste ativo e a conta de cobrança **aprovada** — salvo os três primeiros,
que só existem antes da aprovação.

| # | Arquivo | Como chegar | O que precisa aparecer | Entra em |
|---|---|---|---|---|
| 01 | `cobranca-01-visao-geral.png` | `/cobranca-automatica`, aba **Cobranças** | A tela inteira com as três abas visíveis (Cobranças, Emitir, Ajustes) e o cartão **Como estão as cobranças** com contadores preenchidos. É a imagem de abertura do capítulo | `cobranca-automatica.md`, logo abaixo do parágrafo de abertura (linha 11) |
| 02 | `cobranca-02-antes-de-comecar.png` | Condomínio **sem** conta aberta | O texto explicativo de primeira visita e o início do formulário **Dados para abrir a conta** | Seção "Abrir a conta de cobrança", após o parágrafo de introdução |
| 03 | `cobranca-03-formulario-abertura.png` | Mesmo lugar, rolado até o formulário | O formulário completo: titular, razão social, CNPJ, e-mail, celular, tipo de empresa, faturamento e endereço. **Preencher com dados fictícios** | Seção "Abrir a conta de cobrança", depois da lista dos 6 campos |
| 04 | `cobranca-04-situacao-da-conta.png` | Após o envio do cadastro | O cartão **Situação da conta** com os três indicadores (Dados comerciais, Documentação, Conta bancária) e o botão **Verificar agora** | Subseção "Acompanhar a aprovação", depois da tabela de indicadores |
| 05 | `cobranca-05-documentos.png` | Mesma tela, quando o Asaas pedir documentos | O cartão **Documentos que o Asaas precisa**, com a lista do que falta e o link de envio | Subseção "Acompanhar a aprovação", último parágrafo |
| 06 | `cobranca-06-aba-emitir.png` | Aba **Emitir** | A aba com o botão **Emitir cobrança** em destaque | Seção "Emitir uma cobrança", antes da lista numerada |
| 07 | `cobranca-07-drawer-emitir.png` | Aba **Emitir** → botão **Emitir cobrança** | O painel lateral aberto com o campo de vencimento, a lista **Lançamentos em aberto** (com pelo menos um selecionado) e o quadro **O que vai acontecer** | Seção "Emitir uma cobrança", depois da lista numerada |
| 08 | `cobranca-08-aba-ajustes.png` | Aba **Ajustes** | Os dois cartões: agrupamento (um boleto por item / por vencimento) e **Quando lembrar o morador**, com as quatro opções (2, 3, 5, 7 dias) e o bloco **Avisos automáticos do Asaas** com o botão **Ajustar moradores antigos**. Se não couber, capturar rolado o suficiente para os dois aparecerem | Seção "Ajustes", logo após a frase de abertura |
| 09 | `cobranca-09-lista-cobrancas.png` | Aba **Cobranças** | **O cartão de contadores com números diferentes de zero em pelo menos três estados**, os dois filtros (Estado e Período) e a tabela abaixo com várias linhas e estados distintos. Idealmente com uma linha em cada estado: Emitida, Paga, Vencida, Cancelada | Seção "Acompanhar as cobranças", antes da tabela de estados |
| 10 | `cobranca-10-detalhe-cobranca.png` | Clicar numa cobrança **emitida** (não paga) | O painel de detalhe com o bloco **Onde o morador paga** (botões *Abrir cobrança* e *Boleto em PDF*), **Valores** e **De onde veio esta cobrança** | Subseção "O detalhe de uma cobrança", antes da lista de blocos |
| 11 | `cobranca-11-cancelar-confirmacao.png` | No detalhe de uma cobrança cancelável → **Cancelar cobrança** | O diálogo de confirmação *"Cancelar a cobrança da unidade X?"* com os botões **Voltar** e **Sim, cancelar** | Seção "Cancelar uma cobrança", antes da lista "O que acontece" |
| 12 | `cobranca-12-composicao-pagamento.png` | **Financeiro** → abrir o lançamento de uma cota **já paga** por cobrança | O bloco **Composição do pagamento**: valor cobrado, valor pago, juros e multa (se houver), tarifa do Asaas, uso da plataforma e líquido creditado | Subseção "A composição do pagamento" |
| 13 | `cobranca-13-financeiro-linhas-recolhidas.png` | **Financeiro** → lista de lançamentos do mês da cota paga | A linha da cota com os lançamentos automáticos **recolhidos dentro dela** (e, se der, a mesma linha expandida numa segunda captura) | Subseção "A composição do pagamento", ao fim |

## Telas novas da v7.110.x — prioridade alta

Estas três são o motivo desta rodada: descrevem comportamento que mudou e hoje não tem
nenhuma imagem.

| # | Arquivo | Como chegar | O que precisa aparecer | Entra em |
|---|---|---|---|---|
| 14 | `cobranca-14-detalhe-paga.png` | Aba **Cobranças** → clicar numa cobrança com estado **Paga** | O bloco **Comprovante da cobrança**, com o botão **Abrir fatura** e a frase *"O pagamento já entrou. A fatura fica disponível como comprovante."* — **sem** o botão de boleto em PDF. Se couber na mesma imagem, incluir também o bloco **Lançamentos gerados por esta cobrança** (tarifas e juros) | Subseção "O detalhe de uma cobrança", depois da lista de blocos |
| 15 | `cobranca-15-detalhe-sem-onde-pagar.png` | Aba **Cobranças** → clicar numa cobrança **Cancelada** | O bloco **Não há onde pagar** com o texto explicando que não há mais boleto, Pix nem fatura e orientando emitir nova cobrança a partir do Financeiro | Subseção "O detalhe de uma cobrança", logo após a #14 |
| 16 | `cobranca-16-lista-acoes-icones.png` *(opcional)* | Aba **Cobranças**, desktop, capturando a tabela inteira (cabeçalho + linhas), **sem passar o mouse sobre nenhum ícone** | A coluna **Ações** com os dois ícones (olho e link externo), mostrando lado a lado o link **desabilitado** nas cobranças **canceladas** e **ativo** nas **pagas/emitidas**. Enquadrar com o cabeçalho legível e **sem dica flutuante aberta** — o tooltip tapa a coluna "Pagamento". Se quiser mostrar a dica, use uma segunda imagem separada | Subseção "O detalhe de uma cobrança", no parágrafo que descreve a coluna de ações |

## Já capturado — não precisa refazer

| Arquivo | Página | Situação |
|---|---|---|
| `perfil-como-sou-avisado-01.png` | `modulos/perfil.md` | **Atualizado** com os controles novos (cobranças, comunicados, mural, documentos, tarefas, e-mail, Telegram, resumo). Já conectado na página |
| `perfil-completo-01.png`, `perfil-dados-01.png` | `modulos/perfil.md` | Válidos |

## Situação em 12/08/2026

Capturadas e já conectadas em `modulos/cobranca-automatica.md`: **01, 04, 06, 07, 08, 09, 10, 11, 12, 13, 14, 15, 16**.

Ressalvas:

- **04** foi capturada num condomínio com a conta **já aprovada** (os três indicadores em "Aprovado") — o identificador da conta no Asaas foi borrado na imagem. A versão "em análise" continua pendente.
- **07** mostra a lista com um lançamento selecionado e o quadro "O que vai acontecer"; o campo de vencimento, no topo do painel, ficou fora do enquadramento porque o painel é muito mais alto que a tela.
- **13** mostra a linha da cota **expandida**, com o lançamento de tarifas recolhido dentro dela.

Ainda **não capturáveis**: **02, 03, 05** — dependem de um condomínio **sem** conta aberta/aprovada, estado que não existe mais no Residencial TESTE. Os marcadores seguem no texto.

## Acrescentado em 12/08/2026 — mudanças de interface das versões 7.113.0 a 7.115.3

Estas capturas **não são de Cobrança Automática**, mas entram aqui para não espalhar
roteiro. Mesmas regras: condomínio de teste, dados fictícios, legenda de dados
fictícios embaixo da imagem quando houver nome, unidade ou CPF visível.

| # | Arquivo | Viewport | Como chegar | O que precisa aparecer | Entra em |
|---|---|---|---|---|---|
| 17 | `financeiro-detalhe-lancamento-01.png` | desktop | **Financeiro** → clicar **na linha** de um lançamento (não no lápis) | O painel **Detalhes do lançamento** aberto: valor com a etiqueta de situação, Unidade, Categoria, Conta, Vencimento, Competência, Pago em, Observações e o bloco **Anexos** com ao menos um arquivo listado. Escolher um lançamento **pago e com comprovante anexado**, para o painel sair cheio. **Não** deve haver botão de salvar nem de excluir dentro do painel | `modulos/financeiro.md`, seção "Ver os detalhes de um lançamento" — trocar o marcador `<!-- PRINT: financeiro-detalhe-lancamento-01 … -->` |
| 18 | `navegacao-abas-celular-01.png` *(opcional)* | **celular 375×812** | Qualquer tela com muitas abas — **Configurações** é a melhor (6 abas) | As abas **quebradas em duas linhas**, todas visíveis ao mesmo tempo, sem corte na borda direita da tela. É a prova visual de que nenhuma aba fica escondida | `guia/navegacao.md`, seção "Abas das telas no celular" — trocar o marcador `<!-- PRINT: navegacao-abas-celular-01 … -->` |

Não foi pedida captura para as demais mudanças de 12/08 (botões maiores, exclusão
afastada, caixas de confirmação novas, texto de exclusão corrigido, vencimento no
passado recusado, relatório de inadimplência): são alterações que o texto descreve
bem e que renderiam imagens quase idênticas às que já existem.

## Ordem sugerida de captura

1. Sessão com condomínio **aprovado**: 01, 09, 10, **14**, **15**, 16, 06, 07, 08, 11
2. Ida ao **Financeiro** do mesmo condomínio: 12, 13
3. Só se houver um condomínio **sem conta aberta** à mão: 02, 03, 04, 05 — estas quatro
   dependem de um estado que não se reproduz depois da aprovação; se não houver, o
   capítulo segue publicável sem elas

---

## Acrescentado em 13/08/2026 — versões 7.120.0 a 7.124.1

Mesmas regras de sempre: condomínio de teste, dados fictícios, e a legenda de dados
fictícios embaixo da imagem quando houver nome, unidade, CPF ou valor de morador
visível.

⚠️ **Três destas telas dependem de um condomínio recém-criado** (a partir de
13/08/2026) — o cartão de configuração inicial não aparece em condomínio antigo.
Se o Residencial TESTE não servir, criar um condomínio novo só para a captura.

| # | Arquivo | Viewport | Como chegar | O que precisa aparecer | Entra em |
|---|---|---|---|---|---|
| 19 | `setup-01-cartao-configuracao-inicial.png` | desktop | `/dashboard` de um condomínio **criado a partir de 13/08/2026**, com pendências de sobra | O cartão **Configuração inicial** inteiro: a barra de progresso com **"n de 7 passos concluídos"** (eram 6 até a v7.134; o valor da cota entrou na contagem), o botão **Continuar de onde parei** e ao menos quatro itens da lista, cada um com seu botão de ação. Se der, incluir um item com o selo **Pulado** | `modulos/dashboard.md`, seção "Configuração inicial" — trocar o marcador `<!-- PRINT: setup-01-cartao-configuracao-inicial … -->` |
| 20 | `setup-02-cobranca-em-analise.png` *(opcional)* | desktop | Mesmo cartão, num condomínio com o cadastro da conta **enviado e em análise** | A linha **Cobrança automática — em análise no Asaas**, com a data do envio, o selo **Com o Asaas** e o botão **Aguardando** desabilitado. É a prova de que o cartão distingue o que depende do síndico do que depende de terceiro | `modulos/dashboard.md`, subseção "A linha da Cobrança automática muda de texto conforme o andamento" — hoje sem marcador; inserir logo abaixo da tabela |
| 21 | `cobranca-17-origem-do-pagamento.png` | desktop | **Financeiro** → abrir o lançamento de uma cota **paga por cobrança** | O bloco **Origem do pagamento**, com a frase **"Liquidado pelo Asaas · Pix"** (ou o meio que for), a data, o identificador da cobrança e o botão de copiar. Enquadrar junto com a **Composição do pagamento** acima dele, para a última linha **"Creditado na conta do condomínio"** aparecer na mesma imagem | `modulos/cobranca-automatica.md`, subseção "De onde veio o pagamento" — trocar o marcador `<!-- PRINT: cobranca-17-origem-do-pagamento … -->` |
| 22 | `minha-area-cobrancas-01.png` | desktop | Entrar como **condômino** de unidade com cobrança emitida → **Minha Área** → aba **Minhas cobranças** | O bloco **Em aberto** com ao menos uma cobrança: valor, "Vence em …", a unidade, o selo de situação e o botão **Pagar**. Se houver, o bloco **Histórico** logo abaixo. **Dados fictícios obrigatórios** — a tela mostra unidade e valor | `modulos/minha-area.md`, seção "Aba Minhas cobranças" — trocar o marcador `<!-- PRINT: minha-area-cobrancas-01 … -->` |
| 23 | `minha-area-cobrancas-02-pagar.png` *(opcional)* | **celular 375×812** | Na mesma aba → botão **Pagar** | O painel de pagamento aberto na aba **Pix**, com o **QR Code**, o código copia-e-cola e, no rodapé, o texto do **prazo de reconhecimento** ("Pix e cartão costumam ser reconhecidos em minutos; boleto…"). O celular é o enquadramento certo porque é onde o morador vai pagar | `modulos/minha-area.md`, subseção "Pagar" — hoje sem marcador; inserir depois da tabela de formas |
| 24 | `config-unidades-gerar-em-lote.png` *(opcional)* | desktop | **Configurações → Unidades** → botão **Gerar unidades em lote** | O diálogo com o padrão preenchido (faixa ou bloco), o campo **Taxa mensal das unidades criadas (R$) — opcional** e a **prévia** dizendo quantas serão criadas e quantas já existem | `modulos/configuracoes.md`, subseção "Criar várias unidades de uma vez" — hoje sem marcador; inserir após o primeiro parágrafo |

**Candidatas já existentes.** Na raiz da pasta de trabalho há prints de validação
tirados em 13/08 que podem servir depois de conferidos quanto a dado pessoal e
recortados: `176-cartao-condominio-novo.png` (#19), `176-passo-fecha-sozinho.png`,
`176b-cartao-em-falha-permanente.png`, `177-composicao-corrigida.png`,
`178-origem-do-pagamento.png` (#21), `180-cobrancas-reais-do-morador.png` (#22) e
`unidades-edicao-taxa.png` (#24). **Não foram copiados para `assets/screenshots/`**:
são prints de teste em base de produção e precisam da conferência do Bruno antes de
irem para o manual público.

Não foi pedida captura para os avisos por e-mail (conta de cobrança, pagamento
confirmado, cancelamento) nem para a categoria da cota nascer marcada: o texto
descreve bem, e imagem de e-mail envelhece a cada ajuste de redação.

### ⚠️ Duas imagens quebradas no manual publicado (achado de 13/08)

Não têm relação com as versões acima — são anteriores e estão **quebradas hoje, no ar**:
`modulos/minha-area.md` referencia dois arquivos que **não existem** em
`assets/screenshots/`. O leitor vê o ícone de imagem quebrada.

| # | Arquivo | Viewport | Como chegar | O que precisa aparecer | Entra em |
|---|---|---|---|---|---|
| 25 | `102-minha-area-solicitar-lista.png` | desktop | **Minha Área** → aba **Solicitar Documentos e Serviços** | A lista no computador: Nada Consta, Quitação Anual (IR) com o seletor de ano, Declaração de Débitos/Residência e Certidão de Quitação com cadeado Pro, Solicitar documento (Outros) e Extrato da Unidade, cada item com sua ação à direita | `modulos/minha-area.md` linha 25 — a referência já está no texto, basta o arquivo existir |
| 26 | `103-minha-area-solicitar-cards.png` | **celular 375×812** | A mesma aba | Os mesmos itens como cartões empilhados | `modulos/minha-area.md` linha 29 — idem |

Enquanto não forem capturadas, a alternativa é trocar as duas referências por
marcadores `<!-- PRINT: … -->`, como no resto do manual, para não publicar imagem
quebrada. **Não fiz a troca** para não remover conteúdo sem decisão do Bruno: pode ser
que os arquivos existam fora do repositório e só não tenham sido copiados.

_Nota de arrumação: há três arquivos `debug-minha-area*.png` em `assets/screenshots/`
que nenhuma página referencia — sobra de depuração, candidatos a remoção._

---

## Acrescentado em 14/08/2026 — versões 7.133.0 e 7.134.0

Mesmas regras de sempre: condomínio de teste, dados fictícios, e a legenda de dados
fictícios embaixo da imagem quando houver nome, unidade, CPF ou valor visível.

⚠️ **As duas primeiras dependem de um condomínio SEM conta de cobrança aberta** — o
mesmo estado que já bloqueia as capturas 02, 03 e 05. Se o Residencial TESTE não
servir, criar um condomínio novo só para estas capturas. **Não usar o Vale do Cedro**,
que é o condomínio de produção.

| # | Arquivo | Viewport | Papel | Como chegar | O que precisa aparecer | Entra em |
|---|---|---|---|---|---|---|
| 27 | `cobranca-18-termo-autorizacao.png` | desktop 1920×1080 | síndico | **Cobrança automática**, condomínio **sem conta aberta** → preencher o formulário **Dados para abrir a conta** com dados fictícios → clicar em enviar | A caixa **Termo de Autorização — Conta de Pagamento** aberta: o quadro do topo com condomínio, titular e CNPJ/CPF preenchidos, os três blocos do texto (o que você autoriza, chave Pix, o que a V3RTECH não faz) e, no rodapé, **as duas caixas de seleção** e os botões **Agora não** e **Aceitar e abrir a conta** — este último ainda **desabilitado**, com nenhuma ou só uma caixa marcada. É essa a prova de que os dois consentimentos são exigidos | `modulos/cobranca-automatica.md`, subseção "Autorizar a abertura da conta" — trocar o marcador `<!-- PRINT: cobranca-18-termo-autorizacao … -->` |
| 28 | `cobranca-19-selo-e-suporte.png` | desktop 1920×1080 | síndico | **Cobrança automática** → painel **Antes de começar, o que você precisa saber** (aparece antes da conta aberta e também abaixo do painel da conta já aberta) | O bloco **Suporte sobre a operação financeira** com o telefone **0800 009 0037**, o e-mail **contato@asaas.com.br**, a frase sobre o que fica com a V3RTECH e o **selo do Asaas** logo abaixo. Enquadrar de modo que o **selo do cabeçalho do painel** também apareça, para a imagem mostrar as duas aplicações do selo | `modulos/cobranca-automatica.md`, seção "Com quem falar: Asaas ou V3RTECH" — trocar o marcador `<!-- PRINT: cobranca-19-selo-e-suporte … -->` |
| 29 | `legal-aceite-documentos-01.png` | desktop 1920×1080 | qualquer papel (síndico ou morador) | Entrar no aplicativo com um usuário que **ainda não aceitou** os Termos 1.3 / Privacidade 1.2 | A caixa **Atualizamos nossos documentos** aberta sobre a tela, com o texto de explicação, os dois links (**Termos de Uso** e **Política de Privacidade**), a caixa **Li e aceito…** desmarcada e os botões **Sair da conta** e **Continuar** (desabilitado enquanto a caixa não estiver marcada). **Sem o botão ✕** no canto — é parte do que a imagem precisa provar | `guia/primeiros-passos.md`, seção "Aceitar os Termos de Uso e a Política de Privacidade" — trocar o marcador `<!-- PRINT: legal-aceite-documentos-01 … -->` |
| 30 | `legal-aceite-documentos-02-celular.png` *(opcional)* | **celular 375×812** | qualquer papel | A mesma caixa, no celular | A caixa inteira legível no celular, com os dois botões empilhados e nenhum corte lateral | Mesma seção, como segunda imagem — sem marcador hoje; inserir logo abaixo da #29 |

**Captura que precisa ser refeita:** `setup-01-cartao-configuracao-inicial.png` (#19)
ainda não foi capturada e agora precisa mostrar **"n de 7 passos concluídos"** — a
contagem mudou de 6 para 7 na v7.134. O item **Valor da cota das unidades** deve
aparecer na lista **sem o botão Pular**, ao lado de outro item que tenha o botão: é o
contraste que a página descreve.

Não foi pedida captura para o documento gerado do Termo de Autorização (o PDF com
código e QR), para o aviso de intervalo de datas inválido no Financeiro nem para o
rótulo do exercício corrente na Prestação de Contas: as três são alterações de texto
que a página descreve bem, e renderiam imagens de pouca leitura.
