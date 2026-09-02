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

{: .warning }
> **Pix temporariamente instável em contas novas**
>
> O código Pix é gerado normalmente, mas bancos têm recusado a leitura na hora de pagar. O caso está em apuração com o Asaas, e ainda não sabemos a causa nem o prazo. **Boleto e cartão continuam funcionando normalmente.** Se um morador relatar que o Pix não é aceito pelo banco dele, oriente a pagar por boleto ou cartão enquanto o caso não é resolvido.

## Como funciona, em uma página

- Quem processa o pagamento é o **Asaas**, uma instituição de pagamento autorizada pelo Banco Central. É ele que emite o boleto e o Pix.
- A conta de cobrança é **do condomínio**, aberta em nome dele. **A V3RTECH não fica com o dinheiro em momento nenhum** — o valor da cota cai direto na conta do condomínio.
- A cobrança **sempre parte de um lançamento que já existe no Financeiro**. Nada é lançado em dobro.
- Enquanto a conta não estiver aprovada, **nada muda**: o síndico segue lançando a cota como faz hoje.

### Antes de abrir a conta: o Contrato de Prestação de Serviços precisa estar aceito

A conta de cobrança só pode ser aberta depois que o síndico aceitar, em nome do condomínio, o **Contrato de Prestação de Serviços** — o instrumento que autoriza a V3RTECH a operar a cobrança e a tratar os dados do condomínio para isso. Sem ele, a tela mostra o aviso abaixo no lugar do formulário de abertura:

![Aviso "Falta o Contrato de Prestação de Serviços" na tela de Cobrança automática, com botão para ler e aceitar](/assets/screenshots/cobranca-contrato-bloqueio.png)

{: .note }
> **Esse contrato é diferente do Termo de Autorização — Conta de Pagamento**
>
> Mais adiante nesta página, ao preencher os dados e confirmar a abertura, você vai encontrar um segundo aceite: o [Termo de Autorização — Conta de Pagamento](#autorizar-a-abertura-da-conta), específico da instituição de pagamento (Asaas). São dois documentos diferentes, para autorizações diferentes — o Contrato de Prestação de Serviços vem primeiro e é pré-requisito para chegar a este formulário.

O aceite do contrato se resolve em [Configurações → Condomínio](/modulos/configuracoes/), pelo cartão **Contrato de Prestação de Serviços** — clique em **Ler e aceitar o contrato** ali mesmo ou pelo atalho desta tela.

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
> O formulário pede apenas dados de cadastro. **Nenhum documento, foto ou selfie é enviado pelo aplicativo.** O envio da documentação acontece depois, direto no painel do Asaas — ver o próximo passo.

{: .tip }
> **O que separar antes de começar**
>
> Antes de confirmar o cadastro, a tela agora avisa quais documentos o Asaas vai pedir na sequência, para você já ter em mãos:
>
> - **Ata de eleição da diretoria vigente, registrada em cartório** — é o item que mais atrasa a aprovação. Ata sem registro em cartório é recusada, e registrar leva dias ou semanas
> - **Documento de identidade do síndico**, frente e verso
> - Uma **selfie** tirada na hora, para o reconhecimento facial — feito no painel do Asaas, não aqui
>
> Você pode confirmar o cadastro sem nada disso em mãos — o aviso é só para adiantar a providência. Ele continua visível enquanto a conta está em análise e some quando ela é aprovada.

### Autorizar a abertura da conta

Depois de preencher o formulário e antes de a conta ser aberta, aparece o **Termo de Autorização — Conta de Pagamento**, já preenchido com o que você acabou de digitar: o condomínio, o nome do titular e o CNPJ (ou CPF) informado.

<!-- PRINT: cobranca-18-termo-autorizacao — ver roteiro de capturas -->

O termo existe por exigência da instituição de pagamento: para que a V3RTECH possa abrir e operar a conta em nome do condomínio, o Asaas precisa da **autorização expressa do titular**. Sem ela, ninguém pode agir pela conta de outra pessoa.

O texto diz, em três blocos, o que você está autorizando e o que **não** está:

| Bloco | O que traz |
|---|---|
| **Você autoriza a V3RTECH a…** | Abrir a conta junto ao Asaas, emitir as cobranças a partir dos lançamentos que você registrar, consultar a situação cadastral e as cobranças para exibir aqui, e receber os avisos de pagamento |
| **Consentimento específico — chave Pix** | A criação de uma chave Pix aleatória da conta, sem a qual ela não emite nem recebe por Pix. A chave é da conta do titular, não da V3RTECH |
| **O que a V3RTECH não faz** | Não guarda o dinheiro, não movimenta saldo, não transfere, não saca, não encerra a conta por conta própria e não usa a conta para outra finalidade |

São **dois consentimentos separados**, cada um com sua caixa de seleção:

1. **Autorizo a abertura e a operação da conta de pagamento nos termos acima**
2. **Consinto com a criação da chave Pix aleatória da conta**

O botão **Aceitar e abrir a conta** só é liberado com **as duas** marcadas. Marcar uma só não vale — são autorizações de coisas diferentes.

{: .note }
> **Recusar não trava nada**
>
> O botão **Agora não** fecha o termo e volta para a tela. A conta simplesmente **não é aberta**, e o condomínio continua lançando e recebendo a cota exatamente como faz hoje, sem cobrança automática. Você pode voltar e aceitar quando quiser.

{: .warning }
> **Sem termo registrado, a conta não é aberta**
>
> O aceite é gravado **antes** da abertura, nunca depois. Se a gravação falhar, a tela avisa e a conta **não** é aberta — não existe conta aberta sem autorização registrada. E se você já aceitou a versão vigente do termo, ele não é pedido de novo, mesmo que uma tentativa anterior de abrir a conta tenha falhado.

### O registro do aceite vira documento

Ao confirmar, ficam registrados **a data e a hora**, **a versão do termo** e dados técnicos da sua conexão — o mesmo tipo de prova que qualquer aceite eletrônico exige.

Esse registro gera o **Termo de Autorização — Conta de Pagamento** como documento formal, com o mesmo tratamento dos demais documentos emitidos pelo V3RCondo: **código de verificação** e **QR Code**, que qualquer pessoa pode conferir na página pública de verificação sem precisar de senha. Como o termo é um documento do síndico, a verificação confirma a autenticidade **sem exibir dados da unidade**.

Uma vez emitido, o documento aparece em **Minha Área → Meus documentos e pedidos**, identificado como *Termo de Autorização — Conta de Pagamento*, com o código à vista e o botão de baixar em PDF — ver [Minha Área](/modulos/minha-area/). Ele é do síndico que aceitou: nenhum condômino o vê, e ele não está entre os documentos que se podem solicitar.

### Criar a senha no Asaas e enviar os documentos

Enviado o cadastro, o que falta acontece **do lado do Asaas**, fora do V3RCondo:

1. O Asaas escreve para o **e-mail cadastrado do condomínio** — o mesmo informado no formulário —, com um link para **criar a senha de acesso**. Esse link **expira em 10 minutos**; se o prazo passar, use **"Esqueci minha senha"** na tela de login do Asaas para gerar um novo
2. Com a senha criada, o acesso pede um **código enviado por SMS**
3. Já dentro do **painel do Asaas**, envie a documentação pedida — o envio inclui **reconhecimento facial**, feito lá

{: .warning }
> **Quem abre a conta precisa acessar a caixa de e-mail cadastrada**
>
> É para esse endereço que o Asaas manda o link de criação de senha. Sem acesso a ele, o cadastro trava depois de enviado — combine com quem cuida do e-mail do condomínio antes de começar.

{: .warning }
> **A ata precisa estar registrada em cartório**
>
> O Asaas exige a **ata de eleição da diretoria vigente, com registro em cartório**. Ata sem esse registro é recusada — e como registrar leva dias ou semanas, é o item que mais atrasa a aprovação. Providencie o registro com antecedência, antes mesmo de abrir a conta.

{: .warning }
> **Um documento recusado, todos de novo**
>
> Se qualquer documento for recusado, o Asaas pede **o envio de todos novamente** — não só o que foi recusado. Confira cada arquivo (nitidez, validade, dados legíveis) antes de enviar, para não ter que reenviar o que já estava certo.

### Acompanhar a aprovação

Depois de enviar, a tela passa a exibir o cartão **Situação da conta**, com dois indicadores:

| Indicador | O que significa |
|---|---|
| **Dados comerciais** | As informações do cadastro foram aceitas |
| **Documentação** | Os documentos exigidos pelo Asaas foram enviados e aprovados |

O cartão também mostra **desde quando o cadastro está com o Asaas** — a data e a hora do envio. É por ela que você avalia se a análise passou do razoável e vale procurar o Asaas.

![Cartão "Situação da conta" de uma conta em análise, com a data de envio do cadastro, os indicadores Dados comerciais e Documentação, e o botão Verificar agora](/assets/screenshots/cobranca-situacao-da-conta.png)

*Exemplo de uma conta em análise: os dados comerciais já foram aprovados e a documentação está com o Asaas. O identificador da conta exibido na imagem é fictício.*

Cada indicador aparece como **Pendente**, **Em análise**, **Aprovado** ou **Reprovado**. Use o botão **Verificar agora** para consultar o Asaas e atualizar a situação na hora.

### Você é avisado por e-mail a cada virada

Não é preciso ficar voltando à tela para saber como anda a análise. O síndico recebe um e-mail em cada um dos três momentos:

| Aviso | Quando | O que ele diz |
|---|---|---|
| **Cadastro enviado** | Assim que o cadastro vai para o Asaas | Que a análise depende deles, sem prazo prometido; e que criar a senha e enviar os documentos no painel do Asaas é o que mais costuma destravar |
| **Conta aprovada** | Quando o Asaas aprova | Que já dá para emitir a primeira cobrança e que a baixa no Financeiro passa a ser automática. Lembra também de **conferir o valor da cota das unidades antes de emitir** — unidade sem valor é pulada na geração mensal |
| **Cadastro recusado** | Quando o Asaas recusa | Que o cadastro foi recusado e que, enquanto não for corrigido e reenviado, o condomínio não emite cobrança. O **motivo** é informado pelo Asaas diretamente — o V3RCondo não o repassa |

Cada aviso traz um botão que leva direto à tela da Cobrança automática. A situação continua visível no painel a qualquer momento, e o cartão **Configuração inicial** do [Dashboard](/modulos/dashboard/) também acompanha essa linha.

{: .note }
> **Cada aviso sai uma vez só**
>
> Consultar a situação de novo, ou o app reconferir sozinho, não faz o e-mail sair outra vez.

{: .note }
> **Assim que a conta é aprovada, o canal de avisos se conecta sozinho**
>
> É esse canal que avisa o V3RCondo quando um morador paga — é o que permite a baixa automática no Financeiro. Você não precisa fazer nada: a conexão é feita assim que a conta existe — sem esperar a aprovação, porque é por esse mesmo canal que a aprovação chega — e, se por algum motivo ela não completar de primeira, uma verificação diária tenta de novo até dar certo.

{: .note }
> **Documento pendente ou recusado: quem avisa é o Asaas**
>
> O V3RCondo não lista documento a documento nem repassa o motivo de uma recusa — esse acompanhamento acontece direto no painel do Asaas, que é quem pede, recebe e avalia cada documento. Aqui você acompanha o resultado, pelo indicador **Documentação** acima.

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

{: .note }
> **Unidade sem valor de cota cadastrado é pulada, e a tela avisa na hora**
>
> Ao gerar a cota do mês, uma unidade sem **valor de cota configurado** em **Configurações → Unidades** não entra na geração. A tela informa, no momento, **quantas e quais unidades** ficaram de fora, com o caminho para cadastrar o valor que falta. O e-mail que chega depois ao síndico também nomeia as unidades — não é preciso caçar qual ficou sem cobrança.

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

Quem avisa o morador é o V3RCondo — todos os avisos que o Asaas manda por conta própria ficam **desligados**, sem exceção.

{: .note }
> **Não existe mais e-mail do Asaas com a linha digitável**
>
> Até pouco tempo havia uma exceção: o Asaas enviava, por conta própria, um e-mail com a linha digitável do boleto no dia do vencimento. Essa mensagem foi desligada. Hoje nenhum e-mail de cobrança — nosso ou do Asaas — sai com código de pagamento pronto.

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

### Quando o dinheiro fica disponível

Na coluna **Pagamento**, abaixo da data em que o morador pagou, a cobrança informa **quando aquele valor fica disponível na conta do condomínio**.

![Lista de cobranças com a data de pagamento e, abaixo, a indicação de quando o valor fica disponível](/assets/screenshots/cobrancas-disponibilidade.png)

*Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

- Quando o Asaas informa a **data exata**, ela aparece: *Disponível em 14/09/2026*
- Quando ainda não há data e o prazo é estimado pelo meio de pagamento, aparece o prazo aproximado, **marcado como estimativa**: *Disponível em cerca de 30 dias (estimativa)*
- Quando a cobrança já foi paga e o valor já está disponível, não há nada a avisar — a linha mostra só a data do pagamento

Os prazos típicos, por meio de pagamento:

| Meio | Quando o valor fica disponível |
|---|---|
| **Pix** | Praticamente na hora |
| **Boleto** | No próximo dia útil |
| **Cartão de crédito** | Cerca de **30 dias** |

{: .warning }
> **"Pagamento confirmado" e "dinheiro disponível" são coisas diferentes**
>
> A cota é baixada no Financeiro assim que o pagamento é confirmado — em minutos. Isso significa que o **morador pagou**, não que o dinheiro **já pode ser usado**. No cartão de crédito a diferença chega a um mês: a cota aparece paga hoje e o valor entra na conta só no mês que vem. Leve isso em conta antes de programar um pagamento contando com aquela entrada.

### Quando o Asaas discorda do que está aqui

Uma cobrança pode ser paga, cancelada ou apagada **direto no painel do Asaas**, sem passar pelo V3RCondo. Quando isso acontece, vale sempre o que o Asaas diz — é lá que a cobrança mora —, e a lista deixa isso explícito com um rótulo próprio: **Paga no Asaas**, **Cancelada no Asaas** ou **Removida no Asaas**.

Esse estado real é o que manda também nos **contadores e nos filtros**: procurar por "cancelada" encontra tanto o que foi cancelado aqui quanto o que foi cancelado lá.

### Cobrança excluída ou estornada no Asaas

Além de cancelar, dá para **excluir** ou **estornar** uma cobrança direto no painel do Asaas. O V3RCondo reage de um jeito diferente para cada caso:

- **Excluída no Asaas** — a cobrança deixa de existir lá. O V3RCondo passa a tratá-la como **cancelada**, e o lançamento do Financeiro que a originou **volta a ficar disponível** para uma nova emissão, do mesmo jeito que aconteceria com um cancelamento feito por aqui.
- **Estornada no Asaas** — o dinheiro **entrou e voltou**. A cota continua marcada como **paga no Financeiro**, porque o sistema nunca desfaz uma baixa sozinho quando o assunto é dinheiro. A cobrança fica sinalizada como estornada, e cabe ao síndico decidir: se quiser desfazer a baixa, use a ação **Reverter baixa**, no detalhe da cobrança.
- **Vencida no Asaas** — não exige nenhuma ação: o V3RCondo já identifica sozinho uma cobrança vencida pela data, então não há nada a sincronizar.

{: .warning }
> **Quando os dois lados se contradizem sobre dinheiro**
>
> Se uma cobrança foi excluída no Asaas mas está registrada como **paga** por aqui, o V3RCondo não corrige nada sozinho: marca a cobrança com um aviso de divergência, envia um e-mail ao síndico e espera a decisão dele — manter como paga ou reverter a baixa e cancelar. Contradição sobre dinheiro sempre pede uma pessoa decidindo, nunca uma correção automática.

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

Para pagar, o morador entra no V3RCondo com a própria senha e vai a **Minha Área → Minhas cobranças**, onde escolhe como quer pagar: **boleto, Pix ou cartão**. A escolha é dele, na hora de pagar.

Além disso, o responsável pela unidade recebe **avisos por e-mail**:

| Aviso | Quando |
|---|---|
| **Cobrança emitida** | Assim que a cobrança sai, no formato "Sua cota da unidade [nome] **com vencimento em** [data]" — a data já vem identificada como vencimento, não solta — mais um link que leva ao aplicativo, nunca um código de pagamento pronto |
| **Vence em breve** | Com a antecedência configurada pelo condomínio |
| **Vence hoje** | No dia do vencimento |
| **Venceu** | No dia seguinte ao vencimento |
| **Continua em aberto** | A cada 7 dias depois disso, **até um limite**: no máximo 4 avisos de vencida e nunca além de 30 dias do vencimento. Passado o limite, o assunto deixa de ser tratado por e-mail de cobrança e passa para a [Inadimplência](/modulos/inadimplencia/), com aviso formal e acordo |
| **Pagamento confirmado** | Assim que o pagamento é reconhecido. Traz unidade, valor pago, vencimento, data do pagamento e a **forma de pagamento** usada, e diz que não há mais nada a pagar naquela cobrança |
| **Cobrança cancelada** | Quando a cobrança deixa de valer. O texto muda conforme o motivo (ver abaixo) |

**Nenhum aviso de cobrança traz código Pix, linha digitável de boleto ou link de fatura.** O único link que os avisos carregam é o que leva ao aplicativo — a pessoa entra com a própria senha, confere a cobrança em **Minhas cobranças** e escolhe ali como pagar. Os avisos de confirmação e de cancelamento trazem o mesmo tipo de botão, **Ver minhas cobranças**.

{: .important }
> **Nenhum aviso do V3RCondo leva código de pagamento**
>
> Nem por e-mail, nem por Telegram, na emissão ou em qualquer lembrete: o V3RCondo nunca envia código Pix, linha digitável de boleto ou link de fatura pronto para pagar. Chegou uma cobrança do condomínio com um código desses embutido? Não é nossa — desconfie e avise o síndico antes de pagar. Além do risco de fraude, é uma questão de privacidade: o link de fatura do Asaas abre **sem senha**, e quem o receber — mesmo por engano — vê nome, documento e valor devido de outra pessoa.

### Quando uma cobrança deixa de valer

O morador é avisado, e o aviso não afirma o que o aplicativo não sabe:

| Situação | O que o morador lê |
|---|---|
| O condomínio cancelou a cobrança | **“Uma cobrança sua foi cancelada”** — o boleto, o Pix e a fatura não valem mais; se ainda houver o que pagar, uma nova cobrança será emitida e ele recebe o aviso normalmente |
| A cobrança foi excluída no provedor | **“Uma cobrança sua deixou de valer”** — não pode mais ser paga; em caso de dúvida sobre o motivo, falar com o síndico |
| Havia pagamento e ele foi desfeito | **“Um pagamento seu foi desfeito e a cobrança foi cancelada”** — o aplicativo **não afirma** o que houve com o valor e orienta procurar o síndico, que tem acesso ao extrato da conta de cobrança |

Em todos os três, a mesma orientação: **não pagar de novo**, porque a cobrança não vale mais.

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
- **Creditado na conta do condomínio** — o valor que de fato entra, com a taxa da plataforma **já descontada**
- A data em que foi pago
- Um caminho para abrir a cobrança que originou tudo isso

{: .note }
> **A última linha é o que entra na conta**
>
> A taxa da plataforma é descontada na própria cobrança, junto com a tarifa do Asaas. Antes, a soma exibida não fechava com o extrato porque a taxa da plataforma aparecia discriminada mas não era subtraída do total apresentado. Hoje o número da linha **Creditado na conta do condomínio** é o que você confere no extrato.

### De onde veio o pagamento

Logo abaixo da composição, o bloco **Origem do pagamento** diz como aquela cota foi liquidada:

- A frase **“Liquidado pelo Asaas · Pix”** (ou Boleto, Cartão de crédito, Cartão de débito, Transferência bancária, Dinheiro), seguida da data do pagamento
- O **identificador da cobrança no Asaas**, com um botão para copiar — é o que você usa para localizar o lançamento no extrato do Asaas

<!-- PRINT: cobranca-17-origem-do-pagamento — ver roteiro de capturas -->

{: .note }
> **Quando o meio não é informado**
>
> Quem escolhe como pagar é o morador, na página de cobrança, e o meio só é conhecido quando o pagamento entra. Se o provedor não informar, a frase diz **“meio não informado”** — nunca um meio inventado. Cobranças pagas antes desta versão ficam assim, e está certo: não há como descobrir depois o que não foi registrado na hora.

Essa mesma informação aparece na **Prestação de Contas**, junto de cada lançamento pago por cobrança — ver [Relatórios](/modulos/relatorios/).

**Lançamento pago à mão não mostra origem nenhuma.** Sem cobrança eletrônica por trás, não há meio a informar, e o bloco simplesmente não aparece — em vez de um espaço vazio.

Na lista do Financeiro, esses lançamentos automáticos aparecem **recolhidos dentro da linha da cota** que os originou — clique para expandir. Eles continuam sendo lançamentos normais e entram em todas as somas, filtros, relatórios e exportações exatamente como qualquer outro.

![Lista do Financeiro com a linha da cota paga expandida, mostrando o lançamento de tarifas recolhido dentro dela](/assets/screenshots/cobranca-13-financeiro-linhas-recolhidas.png)

*Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

{: .note }
> **Tarifa e juros têm a data do pagamento**
>
> A cota tem a data de vencimento dela; a tarifa e os juros têm a **data do pagamento**. Quando o pagamento cai num mês diferente do vencimento, a tarifa aparece **sozinha** na lista daquele mês — não é defeito, é a data correta de cada lançamento.

## O resumo diário

Todo dia às **7h (horário de Brasília)**, **cada síndico ativo do condomínio** recebe **um único e-mail** com os pagamentos que entraram desde o resumo anterior:

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
| **Uso da plataforma (V3RTECH)** | Um valor fixo por cobrança paga, **combinado com o seu condomínio** — ele aparece na própria tela de Cobrança automática, antes de você aderir e sempre que quiser conferir | Em cada cobrança **paga** |

**Cobrança emitida e não paga não gera custo nenhum**, nem do Asaas nem da V3RTECH.

No Financeiro, os dois entram numa **única despesa** cuja descrição discrimina quanto foi tarifa do Asaas e quanto foi uso da plataforma.

{: .note }
> **Por que não repetimos a tabela de tarifas do Asaas aqui**
>
> Tarifa de terceiro muda quando eles quiserem, e número copiado vira informação errada sem aviso. Confira sempre na fonte.

## Com quem falar: Asaas ou V3RTECH

Quem processa o pagamento é o Asaas, e isso aparece de forma explícita: o **selo do Asaas** acompanha as telas da cobrança — o painel de apresentação, o cadastro da conta, a situação da conta, os documentos, o detalhe da cobrança e a área do morador — e também os **e-mails da operação financeira**. Clicar no selo abre o site oficial deles.

<!-- PRINT: cobranca-19-selo-e-suporte — ver roteiro de capturas -->

Junto do selo fica o bloco **Suporte sobre a operação financeira**, com os canais do Asaas alcançáveis direto da tela: **0800 009 0037** e **contato@asaas.com.br**. No celular, tocar no telefone abre a discagem e tocar no e-mail abre o aplicativo de e-mail.

A divisão é esta, e vale a pena guardá-la:

| Assunto | Com quem falar |
|---|---|
| **Operação financeira** — liquidação, quando o dinheiro cai, estorno, bloqueio, dados da conta de pagamento, documentos do cadastro | **Asaas** — 0800 009 0037 ou contato@asaas.com.br |
| **Uso do aplicativo** — como emitir, o que a tela mostra, lançamento, relatório, morador, configuração | **Suporte da V3RTECH** |

{: .note }
> **Por que não somos nós no assunto do dinheiro**
>
> A conta de pagamento é do condomínio e quem a opera é a instituição de pagamento. Estorno, bloqueio e prazo de liquidação são decisões e prazos **deles** — repassar o pedido por nós só acrescentaria um intermediário e um dia de espera. O caminho mais curto é falar direto com quem resolve.

Os mesmos canais aparecem nos e-mails de cobrança, de conta de pagamento e no resumo diário, no rodapé, para você não precisar voltar ao aplicativo só para achar um telefone.

## O que ainda não existe

Para não haver surpresa, o que **não** está disponível nesta versão:

- **Parcelamento no cartão** — o morador paga o valor cheio
- **Saque pelo aplicativo** — a movimentação do dinheiro da conta é feita fora do V3RCondo
- **Escolher quais meios de pagamento aceitar** — o morador sempre vê boleto, Pix e cartão
- **Carnê em PDF** com vários meses
- **Repassar a tarifa do cartão ao morador** — a tarifa é sempre custo do condomínio

## Visão do condômino

O condômino **não acessa** a tela de Cobrança Automática — ela é exclusiva de quem administra o condomínio. O que ele tem é a aba **Minhas cobranças**, em [Minha Área](/modulos/minha-area/), mais os avisos por e-mail:

1. Ele recebe o e-mail com o valor, o vencimento e um link para o aplicativo — nunca um código de pagamento pronto
2. Entra com a própria senha, abre a aba **Minhas cobranças** e escolhe **boleto, Pix ou cartão**
3. Paga; em poucos minutos a cota aparece baixada no extrato da unidade, e ele recebe o aviso de **pagamento confirmado**

{: .note }
> **Quanto tempo até constar pago**
>
> Tanto na tela quanto no e-mail de emissão, o morador lê o mesmo aviso: **Pix e cartão costumam ser reconhecidos em minutos; boleto depende do banco processar e pode levar até o dia útil seguinte — e não é para pagar de novo antes disso.** É um texto só, escrito em um lugar só, justamente para a tela e o e-mail nunca dizerem coisas diferentes.
