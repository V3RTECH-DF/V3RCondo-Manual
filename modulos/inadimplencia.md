---
title: Inadimplência e Acordos
parent: Módulos
nav_order: 3.5
---

# Inadimplência e Acordos

{% include video.html id="inadimplencia-e-acordo"
                      titulo="Inadimplência e acordo de parcelamento"
                      descricao="Quem deve e quanto deve, a notificação em lote, e o acompanhamento dos acordos — inclusive os que quebraram." %}

O módulo de **Inadimplência** reúne, por unidade, tudo o que está em atraso no condomínio e as ferramentas para recuperar esses valores — **acordos de parcelamento** e **notificação extrajudicial**.

{: .note }
> **Onde fica e quem acessa**
>
> A Inadimplência tem **item próprio na barra lateral** (logo abaixo de Financeiro) — não fica mais dentro de Relatórios. A página tem **duas abas: Inadimplentes** e **Acordos**.
>
> É uma área de gestão: o **síndico** opera tudo; **Conselho Fiscal** e **Contador** entram em **modo leitura** (veem devedores e acordos, mas não operam); o **condômino comum não acessa** — ele acompanha só a própria dívida e os próprios acordos na **Minha Área**.
>
> **Visualizar** os inadimplentes está no plano **Básico**. As **ações de recuperação** (fechar acordos, emitir notificação extrajudicial e liberar a negociação pelo próprio condômino) são do plano **Pro**. Nos 30 dias grátis tudo fica liberado.

![Módulo Inadimplência com as abas Inadimplentes e Acordos, e a lista de unidades devedoras](/assets/screenshots/inad-visao-01.png)

{: .warning }
> **Sem a categoria da cota configurada, esta tela não apura nada — e diz isso**
>
> A Inadimplência precisa saber qual categoria financeira é a taxa condominial (marcada em **Configurações → Categorias → Financeiro**, ver [Configurações](/modulos/configuracoes/)). Faltando essa configuração, a tela avisa que **a inadimplência não pôde ser apurada**, em vez de mostrar que está tudo em dia — um "zero" ali seria falso, não uma resposta. Marque a categoria em Configurações para a apuração voltar a funcionar; a mesma falta de configuração também bloqueia a emissão de Nada Consta e Certidão de Quitação (ver [Minha Área](/modulos/minha-area/)) e aparece como "não apurada" na Prestação de Contas e no Relatório de Gestão.

## Aba Inadimplentes

### Como a dívida aparece

A aba **Inadimplentes** lista as **unidades devedoras** e, dentro de cada uma, os lançamentos vencidos e ainda não pagos. No topo, um card mostra o **Total Inadimplente** e a quantidade de lançamentos vencidos. É a partir daqui que você notifica um devedor ou fecha um acordo.

{: .note }
> **O que conta como inadimplência?** Um lançamento entra quando é do tipo **receita**, tem vencimento **no passado** e **não** foi pago. Lançamentos com vencimento futuro, mesmo em aberto, ainda estão no prazo e não entram.
>
> Lançamentos de uma **categoria financeira que você excluiu** também deixaram de entrar na conta. Antes eles continuavam somando no total de inadimplência mesmo depois de a categoria sair da lista, o que inflava o valor devido de unidades que já estavam quitadas para efeitos práticos. Se o total do seu condomínio diminuiu sem que ninguém tenha pago, é provável que seja isto.

{: .note }
> Uma unidade que fechou um acordo **sai desta lista** enquanto o acordo estiver em dia — a dívida não sumiu, está "em acordo". Se o acordo for descumprido ou cancelado, a dívida **volta a aparecer** aqui. O acordo em si você acompanha na aba **Acordos** (veja abaixo).

### Notificar devedores (notificação extrajudicial) *(Pro)*

Ao expandir uma unidade, você vê os débitos individuais e pode emitir uma **notificação extrajudicial** — um PDF formal de cobrança.

- **Individual:** expanda a unidade, marque os lançamentos e clique em **Notificar**. Abre um painel com prazo, observações e canal de envio.
- **Em lote:** marque várias unidades e use **Notificar em lote** — uma notificação por unidade, na mesma operação.

![Modal de notificação individual com seleção de lançamentos, prazo e canal de envio](/assets/screenshots/91-inadimplencia-modal-individual.png)

*Dados pessoais fictícios, apenas ilustrativos.*

**Canais:**

| Canal | O que acontece |
|---|---|
| E-mail | PDF enviado ao e-mail do condômino responsável |
| E-mail + Telegram | PDF por e-mail e aviso no Telegram |
| Apenas baixar PDF | PDF gerado para download — nada é enviado ao condômino |

O **PDF** traz o cabeçalho com logo e dados do condomínio, os dados do notificado — com o rótulo **CPF ou CNPJ** conforme o documento cadastrado para o responsável —, a tabela de débitos (descrição, vencimento, valor, dias em atraso), o prazo para regularização, a cláusula legal e um **código de referência** para rastreio. Todas as notificações emitidas ficam no **Histórico**, ao fim da lista, com botão de download.

{: .note }
> **Responsável pela unidade.** Só o condômino designado **responsável** pela unidade recebe a notificação. O responsável é definido ao expandir a unidade ou em **Configurações → Condôminos** — sempre um único por unidade.

## Fechar um acordo de parcelamento *(Pro)*

Um acordo transforma uma ou mais dívidas vencidas de uma unidade em um parcelamento, com desconto opcional. Comece pela aba **Inadimplentes**, na unidade devedora.

**Passo a passo:**

1. Na unidade devedora, clique em **Gerar Acordo**.
2. **Selecione as dívidas** que entram na negociação.
3. Defina o **número de parcelas** (de 1 a 36) e, se quiser, um **desconto**.
4. Confira o resumo e confirme.

![Assistente de novo acordo: seleção das dívidas vencidas que entram na negociação](/assets/screenshots/inad-acordo-criar-01.png)

**O que o sistema faz ao criar o acordo:**

- As dívidas originais **não são apagadas nem quitadas** — passam para o estado "em acordo" e **saem da lista de inadimplência**.
- São criadas as **parcelas novas** (já com o desconto), que passam a ser o que o condômino deve pagar.
- É gerado um **PDF do acordo** com **atestação eletrônica** (quem fez o acordo, o vínculo com a unidade e a data) e o documento do condômino identificado como **CPF** ou **CNPJ**, conforme o que está cadastrado.

{: .tip }
> Um acordo pode ser iniciado por você (síndico) ou pelo **próprio condômino**, pela negociação self-service — veja "Negociação pelo próprio condômino".

## Aba Acordos — todos os acordos num lugar só

A aba **Acordos** lista **todos** os acordos do condomínio, com filtro por status. Cada item mostra a **unidade** e o **responsável**, o selo de status, a data, o progresso das parcelas e o valor. É aqui que você acompanha, registra pagamentos, baixa o PDF e cancela acordos.

![Aba Acordos: lista consolidada de todos os acordos do condomínio, com selos de status e filtro](/assets/screenshots/inad-acordo-status-01.png)

{: .note }
> **A aba abre em "Em andamento".** Por padrão você vê só os acordos **Ativos** e **Quebrados** — os que ainda pedem alguma ação sua. Os acordos **Concluídos** e **Cancelados** ficam atrás do filtro **Status** (escolha **Todos**, **Concluídos** ou **Cancelados**). Para você não achar que eles sumiram, a tela avisa logo acima da lista: *"1 acordo encerrado oculto"* (ou *"N acordos encerrados ocultos"*), com o atalho **Ver todos**.
>
> Lista vazia com esse aviso não é defeito: quer dizer que todos os acordos do condomínio já foram encerrados.

![Aba Acordos em "Em andamento", com o aviso de que há um acordo encerrado oculto](/assets/screenshots/acordo-lista-02-ocultos.png)

{: .note }
> **Por que esta aba existe.** Antes, o acordo só aparecia grudado na unidade dentro da lista de inadimplência. Quando o acordo cobria **toda** a dívida da unidade, ela saía da lista e o acordo "sumia" da sua visão. Agora, **todo acordo fica sempre visível e gerenciável aqui** — inclusive os que já quitaram a dívida inteira da unidade.

### Registrar um acordo que já existia *(Pro)*

Seu condomínio pode ter começado a usar o V3RCondo com acordos já firmados — no cartório, com advogado, numa reunião de conselho. O botão **Registrar acordo existente**, ao lado do filtro de status, serve para esses casos: você **reconhece** o acordo no sistema, em vez de refazê-lo do zero.

**Por que isto importa.** Refazer o acordo com **Gerar Acordo** criaria parcelas novas por cima de lançamentos que já existem — o morador passaria a dever em dobro, e o valor combinado com ele ficaria diferente do que aparece na tela. Registrar o acordo existente faz o contrário: as parcelas **são** os lançamentos que você já tem em aberto, só passam a ser acompanhadas como acordo (com número de parcela, PDF e quebra automática).

{: .note }
> **O que o registro faz e não faz.** Nenhum lançamento é criado, apagado ou muda de valor. **Nenhuma cobrança é emitida e nenhum aviso é enviado** ao morador — registrar é só reconhecer o que já foi combinado. O acordo aparece na lista com o selo **Registrado (anterior ao sistema)**.

O registro acontece numa gaveta lateral, em **3 passos**. Nada é gravado até o último botão.

**Passo 1 — Condições do acordo**

1. Escolha a **Unidade**.
2. Preencha **Valor total da dívida**, **Valor acordado** e **Desconto (%)**.
3. Indique **Quem pediu o acordo** (síndico ou condômino) e, se houver, **Advogado** e **OAB**.
4. Em **Parcelas pagas antes de usar o sistema**, informe a **quantidade** e a **soma (R$)** das parcelas que o morador já cumpriu antes de o condomínio entrar no V3RCondo.
5. Use **Observações** para guardar o que for útil depois (onde foi firmado, em que data, quem testemunhou).
6. Clique em **Escolher parcelas**.

![Passo 1 do registro de acordo existente: unidade, valores, advogado, parcelas pagas antes do sistema e observações](/assets/screenshots/acordo-existente-01-condicoes.png)

{: .warning }
> **O "Valor acordado" é o valor do acordo inteiro — não o total da dívida da unidade.**
>
> A unidade pode ter outros lançamentos em aberto que **não** fazem parte do acordo (a taxa do mês corrente, por exemplo). Se você digitar ali o total em aberto da unidade, o acordo passa a mostrar um valor que ninguém combinou. Digite só o que foi acertado no acordo — somando as parcelas que já foram pagas antes do sistema e as que ainda estão em aberto.

{: .note }
> **Parcelas cumpridas antes do sistema não viram lançamento.** Elas ficam guardadas só como informação do acordo (quantidade e soma). Não entram em nenhum total do Financeiro, não aumentam receita e não mexem na inadimplência — o dinheiro entrou numa época em que o condomínio ainda não usava o V3RCondo. A numeração das parcelas do sistema começa depois delas: se duas foram pagas antes, a primeira parcela do sistema é a **3**.

**Passo 2 — Escolha das parcelas**

A gaveta lista os **lançamentos em aberto da unidade**. Marque aqueles que são as parcelas deste acordo. Para cada um marcado você pode:

- **Corrigir o vencimento da parcela.** Data no passado é aceita — acordos antigos costumam ter parcelas que já venceram. O vencimento só muda para o acordo; se o acordo for cancelado, o lançamento volta à data que tinha.
- Marcar **Já foi paga**, informando a data. Use só quando o pagamento aconteceu **depois** de o condomínio começar a usar o sistema e ainda não foi lançado como pago: a baixa lança a receita no mês da data informada.

Lançamentos que não podem ser parcela aparecem desabilitados, com o motivo escrito embaixo: já pagos, já parte de outro acordo, excluídos, de outra unidade ou que não são receita.

![Passo 2: lançamentos em aberto da unidade 403, com três marcados como parcelas, vencimento editável e a caixa "Já foi paga"](/assets/screenshots/acordo-existente-02-parcelas.png)

No fim da lista há a seção recolhida **Vincular dívidas originais (opcional)**. Use-a só se a dívida que deu origem ao acordo ainda estiver cadastrada como lançamento em aberto. Ao vincular, essa dívida **sai da inadimplência** e volta a aparecer se o acordo quebrar — igual ao acordo criado pelo sistema. Se você não vincula nada, o total em aberto da unidade não muda.

![Seção "Vincular dívidas originais (opcional)" aberta, com os lançamentos que podem ser vinculados](/assets/screenshots/acordo-existente-03-vincular-originais.png)

**Passo 3 — Revisão**

A última tela mostra **tudo o que será adotado**, na ordem das parcelas, e o **total em aberto da unidade antes e depois**. É a sua conferência final: só quando você clica em **Registrar acordo** algo é gravado.

![Passo 3: parcelas 3, 4 e 5 listadas, nota sobre as 2 parcelas pagas antes do sistema e total em aberto igual antes e depois (R$ 4.114,00)](/assets/screenshots/acordo-existente-04-revisao.png)

{: .warning }
> **Confira o "antes e depois": sem dívida original vinculada, os dois números têm de ser iguais.**
>
> Registrar um acordo **não** quita nada — só reconhece parcelas que já estavam em aberto. Se os totais diferirem sem você ter vinculado dívida original nem marcado parcela como paga, algo foi escolhido errado: volte e confira as parcelas e o valor acordado antes de gravar.

**Exemplo concreto.** Em fevereiro, a unidade 403 do Residencial TESTE firmou em cartório um acordo de R$ 2.500,00, em 5 parcelas de R$ 500,00, sem desconto. Duas parcelas (R$ 1.000,00) foram pagas antes de o condomínio usar o sistema. O síndico informa **Valor total da dívida R$ 2.500,00**, **Valor acordado R$ 2.500,00**, **2 parcelas pagas antes do sistema** somando **R$ 1.000,00**, e marca no passo 2 as três taxas ainda em aberto (março, abril e maio). A revisão mostra as parcelas **3, 4 e 5** e o total da unidade em **R$ 4.114,00 antes e depois** — as outras taxas em aberto da unidade (junho a outubro) continuam como inadimplência normal.

![Acordo registrado: selo "Registrado (anterior ao sistema)", 2/5 pagas e as parcelas 3 a 5 pendentes](/assets/screenshots/acordo-existente-05-registrado.png)

**No celular**, a gaveta ocupa a tela inteira e os passos são os mesmos:

![Passo 3 do registro de acordo no celular](/assets/screenshots/acordo-existente-04-revisao-mobile.png)

**Quando dá errado**

| O que você vê | O que significa e o que fazer |
|---|---|
| Lançamento desabilitado com *"já faz parte de outro acordo"* | O lançamento já é parcela ou dívida original de outro acordo. Cancele o outro acordo primeiro, se foi um engano. |
| *"O pagamento em dd/mm/aaaa cai no período …, que já tem prestação de contas publicada"* | Você marcou uma parcela como paga numa data cujo mês já foi prestado e publicado. Escolha outra data ou registre essa parcela como paga **antes do sistema** (passo 1). Ver o aviso abaixo. |
| O botão **Registrar acordo** não habilita | Falta algo: nenhuma parcela marcada, data de pagamento em branco, ou — se há parcela marcada como paga — a **conta que recebeu os pagamentos** não foi escolhida. |
| Mensagem de erro seguida de *"Nada foi gravado"* | O servidor recusou o registro. Como tudo é gravado de uma vez, nada ficou pela metade: corrija e tente de novo. |
| O botão aparece desabilitado com *"Disponível no plano Pro"* | Registrar acordo é recurso do plano Pro (nos 30 dias grátis fica liberado). |

{: .warning }
> **Baixa de parcela em mês com prestação de contas já publicada é recusada.**
>
> Vale para **qualquer** acordo, registrado ou criado pelo sistema: **Marcar como pago** com data num mês cuja prestação de contas já foi publicada não é aceito, porque a baixa mudaria um mês que os condôminos já leram. Para dar baixa, [despublique a prestação](/modulos/relatorios/#prestação-de-contas) daquele mês, faça a baixa e gere e publique de novo.

### Acompanhar e receber as parcelas

Conforme o condômino paga, você **registra o pagamento** de cada parcela (expanda o acordo → **Marcar como pago**). O acordo mostra quantas parcelas já foram pagas e quantas faltam.

![Detalhe de um acordo ativo com uma parcela paga e as demais pendentes](/assets/screenshots/inad-acordo-parcelas-01.png)

Quando a **última parcela é paga**, o acordo é marcado como **Concluído** e as dívidas originais são **quitadas** de vez.

### Quando uma parcela atrasa

Um atraso pontual (uma parcela vencida e ainda não paga) **não** encerra o acordo — ele continua **Ativo**. É o "está um pouco atrasado, mas o acordo segue de pé".

### Quando o acordo é descumprido (quebra automática)

Se a unidade acumular **2 parcelas vencidas e não pagas**, o sistema marca o acordo como **Quebrado automaticamente** (uma verificação roda todo dia). Nesse momento:

- O condômino **perde o desconto** e volta a dever o **valor original cheio**.
- **Tudo o que ele já pagou é abatido** — nada do que entrou é perdido.
- As parcelas ainda não pagas **deixam de existir**.
- As dívidas originais **voltam a aparecer na inadimplência**, com o valor certo — **quando o acordo as tem vinculadas**. Sem dívida original vinculada, nada é removido e as parcelas vencidas seguem em aberto (veja [o que o aviso diz](#o-que-o-aviso-de-acordo-quebrado-diz--e-por-que-depende-do-acordo)).
- Você recebe uma **notificação** (app + e-mail, com a identidade do condomínio).

**Exemplo prático:**

> Uma unidade devia **R$ 1.000**. Acordo com **20% de desconto** = **R$ 800 em 8 parcelas de R$ 100**. O condômino pagou **3 parcelas (R$ 300)** e parou. Na segunda parcela vencida sem pagamento, o acordo **quebra**: perde o desconto (volta a dever **R$ 1.000**), o sistema abate os **R$ 300** já pagos, e a unidade **reaparece devendo R$ 700**. Os R$ 300 continuam registrados nas datas em que foram pagos.

{: .warning }
> **Perder o desconto é intencional.** O desconto é o incentivo para o acordo ser cumprido. Descumprido, a base volta a ser a dívida cheia — sempre creditando o que já foi pago.

#### O que o aviso de acordo quebrado diz — e por que depende do acordo

"Acordo quebrado" é o mesmo evento para todo acordo, mas **o que acontece com a dívida depende de uma coisa só: o acordo tem dívidas originais vinculadas, ou não?** O aviso que chega por e-mail e Telegram descreve o caso certo, e vale entender a diferença para não estranhar o texto.

| O acordo tinha… | O que a quebra faz | O que o aviso diz |
|---|---|---|
| **Dívidas originais vinculadas** — acordo criado pelo sistema com **Gerar Acordo**, ou acordo registrado em que você vinculou as dívidas | As dívidas originais **voltam à inadimplência** com o valor cheio, o que já foi pago é **abatido** e as parcelas ainda não pagas são **removidas** | Que a dívida original voltou com o valor cheio, já descontado o que foi recebido, e que as parcelas não pagas deixaram de existir |
| **Nenhuma dívida original vinculada** — o caso típico do acordo *Registrado (anterior ao sistema)* em que você não usou **Vincular dívidas originais** | **Nada é removido nem recalculado.** As parcelas vencidas continuam em aberto, como lançamentos normais, e **elas são a dívida** | Que as parcelas vencidas seguem em aberto e que nada foi removido nem recalculado, e traz o **saldo vencido em aberto da unidade** |

**Por que isto importa.** Quem lê "acordo quebrado" costuma esperar que a dívida original "volte" e as parcelas "sumam". Isso só acontece quando existe dívida original cadastrada para voltar. Num acordo registrado sem vínculo não há dívida antiga no sistema — o que existe são as próprias parcelas, e elas **já estavam** em aberto. Procurar a dívida original reaparecendo na lista, nesse caso, é procurar o que nunca foi cadastrado.

{: .note }
> **A escolha vem das dívidas vinculadas, não da origem do acordo**
>
> Um acordo registrado como anterior ao sistema **pode** ter dívidas originais vinculadas (você as vincula no registro). Nesse caso a quebra se comporta como a de um acordo criado pelo sistema. O que decide o texto do aviso é só se existe vínculo.

**Exemplo concreto.** A unidade 403 do Residencial TESTE tem um acordo registrado de 5 parcelas de R$ 500,00, sem dívida original vinculada. As parcelas 3 e 4 vencem e não são pagas: o acordo quebra. Você recebe o aviso dizendo que as parcelas vencidas continuam em aberto e que o saldo vencido da unidade é de R$ 1.000,00. Na aba **Inadimplentes** a unidade aparece devendo esse valor — são as duas parcelas, não uma dívida "ressuscitada".

{: .tip }
> **O saldo do aviso é o mesmo da tela de Inadimplência**, apurado na hora do envio. Se divergir do que você vê depois, houve pagamento ou lançamento novo no intervalo.

**Quando dá errado.** Se o sistema não conseguir apurar o saldo no momento do envio, o aviso **não inventa um número**: diz que não foi possível apurar agora e manda você conferir na tela de Inadimplência. Se nem o vínculo das dívidas originais puder ser lido, o aviso se limita a pedir que você confira o acordo e a situação da unidade lá. Nos dois casos, a verdade está na aba **Inadimplentes**.

### Cancelar um acordo manualmente

Você pode **cancelar** um acordo ativo a qualquer momento (expanda o acordo → **Cancelar Acordo**). O efeito é o mesmo da quebra automática, com o crédito correto: as dívidas originais voltam para a inadimplência e **tudo o que já foi pago é abatido**, sem duplicar valores.

![Diálogo de cancelamento de acordo com o aviso de que as parcelas já pagas serão creditadas](/assets/screenshots/inad-acordo-cancelar-01.png)

{: .note }
> **O que você já recebeu continua registrado.** Quebrar ou cancelar um acordo **não reescreve meses já fechados** — cada pagamento fica lançado na data em que entrou. O que ele ainda deve é sempre: **dívida original cheia menos o total já pago**.

**Acordo registrado (anterior ao sistema).** Ao cancelar, cada parcela volta ao **vencimento que tinha antes do registro** e continua em aberto como lançamento normal; nada é apagado. Se alguma parcela já foi baixada, o sistema **não cancela em silêncio**: pede que você decida o que fazer com ela antes de continuar.

![Confirmação de cancelamento de acordo registrado: as parcelas voltam ao vencimento anterior e nada é apagado](/assets/screenshots/acordo-cancelar-02-confirmacao.png)

Um acordo cancelado continua na lista, com a tarja **"Cancelado em dd/mm/aaaa — sem efeito"** e o valor riscado. O **PDF** de um acordo cancelado também sai com uma **tarja avisando que ele não tem efeito** — assim ninguém usa por engano um documento que já não vale.

### Excluir um acordo cancelado

Um acordo cancelado que não serve mais (registrado por engano, por exemplo) pode ser **excluído**: clique na lixeira à direita do acordo e confirme. Ele sai da lista, mas fica guardado no histórico; nenhum lançamento, valor ou vencimento muda.

{: .warning }
> **Só dá para excluir acordo cancelado que não tem nenhuma parcela paga.** Se houver parcela paga, a lixeira fica desabilitada e o motivo aparece ao passar o mouse: a parcela paga é a **prova do pagamento**, e o acordo precisa continuar guardado. Acordo ativo, quebrado ou concluído também não se exclui — para o ativo, use **Cancelar Acordo**.

![Acordo cancelado com a tarja "sem efeito" e a dica "Excluir acordo" sobre a lixeira](/assets/screenshots/acordo-cancelado-03-excluir.png)

![Confirmação "Excluir este acordo cancelado?"](/assets/screenshots/acordo-cancelado-04-excluir-confirmacao.png)

### Corrigir os dados de um acordo (lápis)

Digitou o nome do advogado errado ou esqueceu a OAB? Não precisa cancelar o acordo: o **lápis** ao lado do valor abre **Editar dados do acordo** e corrige só os dados descritivos.

| Situação do acordo | O que você pode corrigir |
|---|---|
| **Ativo** ou **Quebrado** | Todos os dados descritivos: dívida total, valor acordado, desconto, quem pediu, advogado, OAB e observações — e, no acordo registrado, a quantidade e a soma das parcelas pagas antes do sistema |
| **Concluído** ou **Cancelado** | Só **advogado, OAB, observações e quem pediu** |

**Parcelas, vencimentos, baixas e dívidas vinculadas nunca se editam ali.** Para mudar uma delas é preciso cancelar o acordo e registrar de novo.

![Editar dados de um acordo ativo: todos os campos descritivos liberados](/assets/screenshots/acordo-editar-dados-01-ativo.png)

![Editar dados de um acordo encerrado: só advogado, OAB, observações e quem pediu](/assets/screenshots/acordo-editar-dados-02-encerrado.png)

### Os status de um acordo

| Status | O que significa |
|---|---|
| **Ativo** | Acordo em andamento; parcelas sendo pagas (pode haver atraso pontual). |
| **Concluído** | Todas as parcelas foram pagas; as dívidas originais foram quitadas. |
| **Quebrado** | Acumulou 2 parcelas vencidas sem pagamento; a dívida voltou (cheia, menos o pago). |
| **Cancelado** | Encerrado manualmente pelo síndico; a dívida voltou (cheia, menos o pago). |

## Negociação pelo próprio condômino *(Pro)*

Quando essa opção está ativa, o **condômino** pode propor e fechar o parcelamento da própria dívida pela **Minha Área**, sem depender de você iniciar. Ele seleciona os débitos, escolhe o número de parcelas (dentro dos limites que você definiu), vê o preview (dívida + multa + juros = total acordado) e confirma um termo de compromisso. O acordo resultante segue exatamente as mesmas regras acima — inclusive a quebra automática por descumprimento.

{: .note }
> **Parâmetros do self-service.** Você configura multa, juros, máximo de parcelas e valor mínimo por parcela em **Configurações → Cobranças & Acordos**. Sem configurar, o padrão é 2% de multa, 1% de juros ao mês, até 12 parcelas e mínimo de R$ 50,00 por parcela.
