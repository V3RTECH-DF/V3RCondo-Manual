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
