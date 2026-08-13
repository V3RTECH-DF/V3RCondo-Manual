---
title: Cobrança Automática
parent: Módulos
nav_order: 3.6
---

# Cobrança Automática

A Cobrança Automática permite que o condomínio **cobre a cota por boleto, Pix ou cartão**, com o dinheiro caindo **direto na conta do condomínio**. Quando o morador paga, o V3RCondo fica sabendo sozinho e dá baixa no Financeiro.

![Aba Cobranças da Cobrança Automática, com as três abas do módulo, o cartão "Como estão as cobranças" com um contador por estado, os filtros e o início da lista](/assets/screenshots/cobranca-01-visao-geral.png)

*Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

{: .note }
> **Disponibilidade**
>
> A Cobrança Automática faz parte do **plano Pro** e está sendo **liberada aos poucos**, condomínio a condomínio. Para usá-la, o condomínio precisa ter a **conta de cobrança aberta e aprovada** (o passo a passo está logo abaixo). Se o item **Cobrança automática** ainda não aparece no menu do seu condomínio, fale com a nossa equipe.

## Como funciona, em uma página

- Quem processa o pagamento é o **Asaas**, uma instituição de pagamento autorizada pelo Banco Central. É ele que emite o boleto e o Pix.
- A conta de cobrança é **do condomínio**, aberta em nome dele. **A V3RTECH não fica com o dinheiro em momento nenhum** — o valor da cota cai direto na conta do condomínio.
- A cobrança **sempre parte de um lançamento que já existe no Financeiro**. Nada é lançado em dobro.
- Enquanto a conta não estiver aprovada, **nada muda**: o síndico segue lançando a cota como faz hoje.

## Abrir a conta de cobrança *(síndico — plano Pro)*

No menu lateral, abra **Cobrança automática**. Na primeira vez, a tela explica o que vai acontecer e mostra o formulário **Dados para abrir a conta**.

<!-- PRINT: cobranca-02-antes-de-comecar — ver roteiro de capturas -->

Preencha:

1. **Quem é o titular da conta** — o condomínio (pessoa jurídica) ou uma pessoa física
2. **Nome / Razão social** e **CNPJ ou CPF**
3. **E-mail** e **celular com DDD**
4. **Data de nascimento** (para titular pessoa física) ou **tipo de empresa** (para pessoa jurídica — condomínios normalmente se enquadram como *Associação*)
5. **Faturamento mensal estimado** — digite o valor e o campo formata como moeda sozinho (ex.: `25000` vira `R$ 25.000,00`); confira o valor formatado antes de avançar
6. **Endereço** — CEP, logradouro, número e bairro

<!-- PRINT: cobranca-03-formulario-abertura — ver roteiro de capturas -->

{: .note }
> **Documento não passa pelo V3RCondo**
>
> O formulário pede apenas dados de cadastro. **Nenhum documento, foto ou selfie é enviado pelo aplicativo.** Quando o Asaas exigir documentação, o V3RCondo mostra o que falta e o endereço seguro do próprio Asaas para o envio — o arquivo vai direto de você para eles.

### Acompanhar a aprovação

Depois de enviar, a tela passa a exibir o cartão **Situação da conta**, com três indicadores:

| Indicador | O que significa |
|---|---|
| **Dados comerciais** | As informações do cadastro foram aceitas |
| **Documentação** | Os documentos exigidos pelo Asaas foram enviados e aprovados |
| **Conta bancária** | Situação que o Asaas reporta. É apenas informativo — esse dado não é enviado pelo V3RCondo |

![Cartão "Situação da conta" com os três indicadores — Dados comerciais, Documentação e Conta bancária — e o botão Verificar agora](/assets/screenshots/cobranca-04-situacao-da-conta.png)

*Exemplo de um condomínio com a conta já aprovada: os três indicadores aparecem como Aprovado.*

Cada indicador aparece como **Pendente**, **Em análise**, **Aprovado** ou **Reprovado**. Use o botão **Verificar agora** para consultar o Asaas e atualizar a situação na hora.

Quando o Asaas pedir documentos, aparece o cartão **Documentos que o Asaas precisa**, com a lista do que falta e o link de envio deles (o envio inclui reconhecimento facial, feito no site do Asaas).

<!-- PRINT: cobranca-05-documentos — ver roteiro de capturas -->

{: .warning }
> **Enquanto a conta não estiver aprovada**
>
> A emissão de cobrança fica indisponível, e a tela diz o motivo. **Nada quebra por isso**: o condomínio continua lançando a cota normalmente no Financeiro, como sempre fez, e nenhum condômino é cobrado.

Com a conta aprovada, a tela passa a exibir três abas: **Cobranças**, **Emitir** e **Ajustes**.

## Emitir uma cobrança *(síndico)*

A emissão **parte de um lançamento que já existe no Financeiro** — a cota do mês ou uma taxa avulsa. Se o lançamento ainda não existe, crie-o primeiro no [Financeiro](/modulos/financeiro/).

Na aba **Emitir**, clique em **Emitir cobrança**:

![Aba Emitir, com o botão Emitir cobrança em destaque](/assets/screenshots/cobranca-06-aba-emitir.png)

1. Informe o **vencimento da cobrança**. É a data que o morador vai ver. O vencimento do lançamento no Financeiro **não muda**. O campo só aceita **hoje ou uma data futura**: se você digitar uma data já passada, o aviso aparece na hora e o botão de confirmar fica bloqueado até corrigir — o Asaas não emite cobrança com vencimento no passado. Para uma cota que já venceu, use a data de hoje ou a data-limite que você quer dar ao morador
2. Escolha um lançamento na lista **Lançamentos em aberto** — cada linha mostra unidade, morador, descrição, vencimento e valor
3. Confira o quadro **O que vai acontecer**, que resume quem vai receber a cobrança, de quanto, com que vencimento e quais são os custos
4. Clique em **Confirmar emissão**

![Painel de emissão com um lançamento selecionado na lista e o quadro "O que vai acontecer", que resume quem recebe a cobrança, de quanto e quais são os custos](/assets/screenshots/cobranca-07-drawer-emitir.png)

*Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

Emitida a cobrança, ela aparece na aba **Cobranças** no estado **Emitida**, com o endereço da fatura, que o síndico pode abrir e repassar ao morador se quiser.

### O que impede uma emissão

| Situação | O que acontece |
|---|---|
| Unidade **sem responsável** ou responsável **sem CPF** cadastrado | A emissão é recusada, dizendo qual unidade e o que falta. Cadastre o CPF do responsável em **Configurações → Unidades** |
| Lançamento **já tem uma cobrança em aberto** | A emissão é recusada. Cancele a cobrança atual antes de emitir outra |
| Valor **abaixo de R$ 5,00** | O Asaas não aceita cobranças abaixo desse valor |
| Lançamento de **despesa** | Só lançamentos de receita viram cobrança — despesas nem aparecem na lista |

{: .note }
> **Uma cobrança viva por lançamento**
>
> Cada lançamento pode ter **apenas uma cobrança ativa por vez**. Isso vale mesmo se você clicar duas vezes, abrir duas abas ou reenviar depois de a conexão cair: o morador nunca recebe dois boletos do mesmo item.

## Emissão automática no ciclo mensal *(síndico)*

Quando a rotina mensal gera a cota do condomínio, as cobranças correspondentes são emitidas **sozinhas**, sem o síndico precisar emitir uma por uma. Isso acontece apenas para condomínios com a conta de cobrança **aprovada**.

Alguns pontos importantes:

- **A emissão automática vale do próximo ciclo em diante.** Para a cota deste mês, que já foi lançada, use a emissão avulsa da aba **Emitir** — nada é lançado de novo no Financeiro
- **A falha de uma unidade não derruba as outras.** Se uma unidade estiver sem CPF do responsável, só ela falha; as demais cobranças saem normalmente
- **O lançamento existe de qualquer jeito.** A cota do mês continua no Financeiro mesmo que a cobrança não tenha saído
- **Rodar o ciclo de novo não gera cobrança duplicada**
- O aviso que o síndico já recebe ao fim do ciclo passa a dizer **quantas cobranças saíram, quantas não saíram e por quê**, com a unidade de cada falha

## Ajustes *(síndico)*

Na aba **Ajustes** ficam duas escolhas do condomínio.

![Aba Ajustes, com o cartão de agrupamento (um boleto por item ou por vencimento e unidade) e o cartão "Quando lembrar o morador", com as quatro antecedências e o bloco dos avisos automáticos do Asaas](/assets/screenshots/cobranca-08-aba-ajustes.png)

### Cota e taxas extras: junto ou separado?

Vale para itens da **mesma unidade** com o **mesmo vencimento**:

- **Um boleto por item (padrão)** — cada cobrança fala de uma coisa só. Mais fácil de auditar e de dar baixa
- **Um boleto por vencimento e unidade** — o morador recebe tudo num documento só, e o condomínio paga uma tarifa em vez de três

{: .note }
> Lançamentos com **vencimentos diferentes nunca se agrupam**, e **parcela de acordo sempre tem boleto próprio**, porque o cronograma dela é independente.

### Quando lembrar o morador

Define com quantos dias de antecedência sai o **primeiro lembrete** — **2, 3 (padrão), 5 ou 7 dias antes**. Depois dele, o morador ainda recebe aviso no dia do vencimento e quando a cota fica em atraso. A escolha é salva na hora, sem botão de confirmar.

{: .warning }
> **O lembrete só sai se a cobrança já existir**
>
> Se o condomínio emite as cobranças dois dias antes do vencimento, um lembrete configurado para três dias antes nunca vai acontecer. Escolha uma antecedência **menor** que o intervalo entre a emissão e o vencimento.

### Avisos automáticos do Asaas

Quem avisa o morador é o V3RCondo — os avisos que o Asaas manda por conta própria ficam desligados para não chegar tudo em dobro, **com uma única exceção: o e-mail com a linha digitável do boleto, enviado ao morador no dia do vencimento**.

{: .note }
> **Você não recebe recibo do Asaas**
>
> O síndico não é copiado nos avisos do Asaas. O pagamento aparece para você **no [Financeiro](/modulos/financeiro/), assim que é conciliado**, e no **resumo diário por e-mail** — não há aviso individual de recibo a cada cota paga.

Se moradores cadastrados antes de a régua existir ainda recebem outras mensagens do Asaas, use o botão **Ajustar moradores antigos**, no mesmo cartão. Ele pode ser acionado quantas vezes quiser: rodar de novo não muda o resultado, e a mensagem final diz quantos moradores foram ajustados (ou que já estava tudo certo).

## Acompanhar as cobranças *(síndico)*

A aba **Cobranças** abre no cartão **Como estão as cobranças**, com um **contador por estado**. Cada contador é também um atalho: clique nele para filtrar a lista por aquele estado, e clique de novo para voltar a ver tudo. Logo abaixo ficam os filtros por **estado** e por **período (vencimento)**, este último com um mês por opção.

![Lista de cobranças com os contadores por estado, os filtros de estado e período e a tabela com cobranças emitidas, pagas e canceladas](/assets/screenshots/cobranca-09-lista-cobrancas.png)

*Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

| Estado | Significado |
|---|---|
| **Emitida** | A cobrança está no ar e o morador pode pagar |
| **Paga** | O pagamento entrou e o lançamento foi baixado no Financeiro |
| **Vencida** | Passou do vencimento e continua em aberto |
| **Aguardando confirmação** | A comunicação com o Asaas falhou e ainda não sabemos se a cobrança chegou a ser criada. Precisa de conferência antes de qualquer nova tentativa |
| **Cancelada** | Foi cancelada e não vale mais. Continua na lista como registro |
| **Falha na emissão** | A cobrança não chegou a ser criada. O motivo aparece no detalhe |

{: .note }
> **A tela mostra o estado, não o dinheiro**
>
> Aqui você acompanha quantas cobranças saíram, quais falharam e quais venceram. **Quanto entrou no caixa continua sendo no [Financeiro](/modulos/financeiro/)**, e quem está devendo, na [Inadimplência](/modulos/inadimplencia/) — por isso esta tela não exibe soma nem saldo.

### Quando o Asaas discorda do que está aqui

Uma cobrança pode ser paga, cancelada ou apagada **direto no painel do Asaas**, sem passar pelo V3RCondo. Quando isso acontece, vale sempre o que o Asaas diz — é lá que a cobrança mora —, e a lista deixa isso explícito com um rótulo próprio: **Paga no Asaas**, **Cancelada no Asaas** ou **Removida no Asaas**.

Esse estado real é o que manda também nos **contadores e nos filtros**: procurar por "cancelada" encontra tanto o que foi cancelado aqui quanto o que foi cancelado lá.

### O detalhe de uma cobrança

Clique na linha (ou no ícone de olho, na coluna **Ações**) para abrir o detalhe. Na mesma coluna há o ícone de **abrir a página de pagamento** — ele aparece **desabilitado** quando aquela cobrança não tem onde pagar, e a dica explica o motivo em vez de sumir da tela. No celular, os mesmos dois ícones ficam no rodapé do cartão de cada cobrança.

![Coluna Ações da lista, com o ícone de olho e o ícone de abrir a página de pagamento desabilitado numa cobrança cancelada, e a dica explicando que não há mais onde pagar](/assets/screenshots/cobranca-16-lista-acoes-icones.png)

*Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

![Detalhe de uma cobrança emitida, com o bloco "Onde o morador paga" (Abrir cobrança e Boleto em PDF), os valores e o lançamento que deu origem à cobrança](/assets/screenshots/cobranca-10-detalhe-cobranca.png)

*Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

O detalhe traz:

- **Onde o morador paga** — para uma cobrança viva: a página de pagamento (que oferece boleto, Pix e cartão) e o boleto em PDF
- **Comprovante da cobrança** — para uma cobrança **já paga**: só a fatura, que passa a servir de comprovante. O boleto em PDF não aparece, porque para cota quitada ele não tem função
- **Não há onde pagar** — para uma cobrança **cancelada, removida no Asaas ou com falha na emissão**: em vez de um botão que levaria a uma página de erro, a tela explica o que houve e orienta **emitir uma nova cobrança a partir do lançamento no Financeiro**
- **Valores** — valor cobrado, uso da plataforma e o líquido estimado
- **De onde veio esta cobrança** — os lançamentos do Financeiro que a originaram
- **Lançamentos gerados por esta cobrança** — só em cobrança paga: as tarifas e, quando houver, os juros e multa que a conciliação lançou, cada um com a data do pagamento
- **Cancelar esta cobrança**, quando ela ainda pode ser cancelada

![Detalhe de uma cobrança paga, com o bloco "Comprovante da cobrança" e o botão Abrir fatura, e os lançamentos de tarifa gerados pela conciliação](/assets/screenshots/cobranca-14-detalhe-paga.png)

*Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

![Detalhe de uma cobrança cancelada, com o bloco "Não há onde pagar" explicando que não existe mais boleto, Pix nem fatura](/assets/screenshots/cobranca-15-detalhe-sem-onde-pagar.png)

*Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

{: .note }
> **Líquido estimado é estimativa mesmo**
>
> Antes do pagamento, o Asaas calcula o líquido pelo **pior caso** — como se o morador fosse pagar no cartão. O valor real só é conhecido quando o pagamento entra, e é ele que aparece na composição do lançamento no Financeiro.

## Cancelar uma cobrança *(síndico)*

Errou o valor, o vencimento ou emitiu para a unidade errada? Abra o detalhe da cobrança e clique em **Cancelar cobrança**.

![Diálogo de confirmação perguntando se você quer cancelar a cobrança da unidade, com os botões Voltar e Sim, cancelar](/assets/screenshots/cobranca-11-cancelar-confirmacao.png)

O que acontece:

- A cobrança **sai do ar** e o morador deixa de conseguir pagá-la
- O **lançamento volta a ficar disponível** para nova emissão
- A cobrança **continua aparecendo na lista**, marcada como **Cancelada**, como registro do que houve
- No detalhe dela, no lugar dos caminhos de pagamento, passa a aparecer **"Não há onde pagar"**, com a orientação de emitir uma nova cobrança a partir do lançamento no Financeiro

{: .note }
> **Depois de cancelar, não há link para reaproveitar**
>
> O boleto, o Pix e a fatura de uma cobrança cancelada **deixam de existir do lado do Asaas** — abri-los levaria a uma página de erro. Se o condomínio ainda precisa receber aquele valor, o caminho é **emitir uma cobrança nova**, com o valor e o vencimento certos, a partir do mesmo lançamento no Financeiro.

{: .warning }
> **Cobrança já paga não pode ser cancelada**
>
> Antes de cancelar, o aplicativo confere a situação atual no Asaas. Se o morador já pagou, o cancelamento é **recusado** — a devolução, se for o caso, é tratada fora do aplicativo. Se a consulta não responder, o cancelamento também é recusado: sem confirmação do estado atual, o aplicativo não cancela nada.

{: .note }
> **Cancelamento é um de cada vez**
>
> Não existe cancelamento em lote nesta versão, nem estorno ou devolução pelo aplicativo, nem reemissão automática — depois de cancelar, emitir de novo continua sendo uma ação sua.

## O que o morador recebe

O morador **não precisa fazer nada no V3RCondo** para pagar. Ele recebe uma **página de cobrança** onde escolhe como quer pagar: **boleto, Pix ou cartão**. A escolha é dele, na hora de pagar.

Além disso, o responsável pela unidade recebe **avisos por e-mail**:

| Aviso | Quando |
|---|---|
| **Cobrança emitida** | Assim que a cobrança sai, com valor, vencimento, **código Pix copia-e-cola**, **linha digitável** do boleto e o link da página de cobrança |
| **Vence em breve** | Com a antecedência configurada pelo condomínio |
| **Vence hoje** | No dia do vencimento |
| **Venceu** | No dia seguinte ao vencimento |
| **Continua em aberto** | A cada 7 dias depois disso, **até um limite**: no máximo 4 avisos de vencida e nunca além de 30 dias do vencimento. Passado o limite, o assunto deixa de ser tratado por e-mail de cobrança e passa para a [Inadimplência](/modulos/inadimplencia/), com aviso formal e acordo |

Todos os avisos trazem o Pix, a linha digitável e o link da fatura, para a pessoa conseguir pagar no momento em que lê.

{: .important }
> **Ninguém é avisado sem conferir antes**
>
> Antes de cada envio, o aplicativo consulta a situação real da cobrança no Asaas. Cobrança **paga, cancelada ou removida não gera aviso nenhum** — inclusive quando o desfecho aconteceu fora do V3RCondo. Se a consulta não responder ou trouxer uma situação que não conhecemos, o aviso do dia é **suspenso** (a cobrança não é dada como paga, e a consulta se repete no dia seguinte).

{: .note }
> **O e-mail de cobrança não pode ser desligado**
>
> Nas preferências do morador ([Meu Perfil](/modulos/perfil/) → **Como sou avisado**), o assunto **Cobranças** permite ligar e desligar o aviso no celular, mas o **e-mail permanece sempre ligado** — e continua chegando mesmo que a pessoa desligue o interruptor geral **Receber e-mails**. O mesmo vale para acordos, aviso de inadimplência e convocação de assembleia: são comunicações financeiras e formais, com prazo e consequência. Quem não recebe o boleto não paga, e o prejuízo é dele e do condomínio.

## Quando o morador paga

O aplicativo **fica sabendo sozinho**, em poucos minutos — o síndico não precisa importar nada nem marcar nada como pago. Automaticamente:

- A cota é **baixada no Financeiro** com a **data real do pagamento**, não a data de hoje
- As **tarifas viram uma despesa** do condomínio, com a data do pagamento
- Se o morador pagou **com juros e multa**, a diferença entra como **receita**

É isso que faz o **saldo do aplicativo bater com o extrato da conta**.

### A composição do pagamento

Abra o lançamento da cota paga no Financeiro e você verá o bloco **Composição do pagamento**:

![Bloco "Composição do pagamento" no lançamento da cota paga: valor cobrado, tarifa do Asaas, uso da plataforma e líquido creditado, com a data do pagamento](/assets/screenshots/cobranca-12-composicao-pagamento.png)

- Valor cobrado e, quando diferente, o **valor efetivamente pago**
- **Juros e multa recebidos**, quando houver
- **Tarifa do Asaas** e **Uso da plataforma (V3RTECH)**, discriminados
- **Líquido creditado** na conta do condomínio
- Um caminho para abrir a cobrança que originou tudo isso

Na lista do Financeiro, esses lançamentos automáticos aparecem **recolhidos dentro da linha da cota** que os originou — clique para expandir. Eles continuam sendo lançamentos normais e entram em todas as somas, filtros, relatórios e exportações exatamente como qualquer outro.

![Lista do Financeiro com a linha da cota paga expandida, mostrando o lançamento de tarifas recolhido dentro dela](/assets/screenshots/cobranca-13-financeiro-linhas-recolhidas.png)

*Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

{: .note }
> **Tarifa e juros têm a data do pagamento**
>
> A cota tem a data de vencimento dela; a tarifa e os juros têm a **data do pagamento**. Quando o pagamento cai num mês diferente do vencimento, a tarifa aparece **sozinha** na lista daquele mês — não é defeito, é a data correta de cada lançamento.

## O resumo diário

Uma vez por dia, no fim do dia, **cada síndico ativo do condomínio** recebe **um único e-mail** com os pagamentos que entraram:

- Quantos pagamentos e o **total recebido**
- A lista **por unidade**, com o morador, o valor pago e a data
- O destaque de **juros e multa**, quando houver
- O **total de tarifas** do dia e o **valor líquido creditado** na conta

**Dia sem pagamento não gera e-mail.** Nenhum pagamento entra em dois resumos, e o que caiu depois do resumo de ontem entra no de hoje — nada se perde na virada do dia. O resumo serve para dar tranquilidade e visão geral; o Financeiro já mostra cada pagamento muito antes, porque a baixa acontece em poucos minutos.

Quem tem o **Telegram** conectado recebe o mesmo resumo por lá.

## Quanto custa

São **dois valores diferentes, de duas empresas diferentes**:

| Custo | Quem cobra | Quando |
|---|---|---|
| **Tarifa do Asaas** | O Asaas, em cada cobrança paga. O valor varia conforme o meio de pagamento e está na [página oficial de preços deles](https://www.asaas.com/precos) | Em cada cobrança **paga** |
| **Uso da plataforma (V3RTECH)** | R$ 1,00 por cobrança paga — o valor é combinado por condomínio e aparece na própria tela | Em cada cobrança **paga** |

**Cobrança emitida e não paga não gera custo nenhum**, nem do Asaas nem da V3RTECH.

No Financeiro, os dois entram numa **única despesa** cuja descrição discrimina quanto foi tarifa do Asaas e quanto foi uso da plataforma.

{: .note }
> **Por que não repetimos a tabela de tarifas do Asaas aqui**
>
> Tarifa de terceiro muda quando eles quiserem, e número copiado vira informação errada sem aviso. Confira sempre na fonte.

## O que ainda não existe

Para não haver surpresa, o que **não** está disponível nesta versão:

- **Parcelamento no cartão** — o morador paga o valor cheio
- **Saque pelo aplicativo** — a movimentação do dinheiro da conta é feita fora do V3RCondo
- **Escolher quais meios de pagamento aceitar** — o morador sempre vê boleto, Pix e cartão
- **Carnê em PDF** com vários meses
- **Repassar a tarifa do cartão ao morador** — a tarifa é sempre custo do condomínio

## Visão do condômino

O condômino **não acessa** a tela de Cobrança Automática — ela é exclusiva de quem administra o condomínio. Para o morador, tudo acontece por e-mail e na página de cobrança:

1. Ele recebe o e-mail com o Pix copia-e-cola, a linha digitável e o link
2. Abre a página de cobrança e escolhe **boleto, Pix ou cartão**
3. Paga; em poucos minutos a cota aparece baixada no extrato da unidade, em [Minha Área](/modulos/minha-area/)
