---
title: Assistente por Mensagem (Telegram)
parent: Módulos
nav_order: 7.5
---

# Assistente por Mensagem (Telegram)

{: .warning }
> **Plano Pro**
>
> Falar com o V3RCondo pelo Telegram é um recurso do **plano Pro** — para o
> síndico e, quando ele habilitar, para o condômino também. Cada papel tem a
> sua própria franquia mensal, e elas não se misturam: **50 mensagens por
> mês, por condomínio**, para o síndico (ampliável por pacote ou recarga); e
> **20 mensagens por mês, por condômino**, própria e sem compra. No plano
> Básico, o Telegram continua disponível — mas só para **receber avisos**
> (veja [Notificações](/modulos/notificacoes/)), não para falar com o bot.

Além de abrir o aplicativo, você pode falar com o V3RCondo pelo **Telegram**:
o síndico pode perguntar o saldo em caixa, lançar uma despesa a partir da
foto de um boleto ou dar baixa num pagamento; o condômino pode consultar a
segunda via do próprio boleto, a situação da própria unidade, as próprias
reservas e solicitações — tudo puxando conversa com o bot, do celular, sem
precisar abrir o navegador. É útil quando você está fora de casa, numa
reunião com um fornecedor, ou só quer resolver algo rápido sem esperar o
aplicativo carregar.

O assistente age **com as mesmas permissões que você já tem** no aplicativo
— ele não abre uma porta nova, só encurta o caminho para o que você já
poderia fazer pela tela. Por isso esta página tem duas trilhas: leia a que
corresponde ao seu papel — [Para o síndico](#para-o-síndico) ou
[Para o condômino](#para-o-condômino).

## Para o síndico

## Antes de começar

1. **Conecte o Telegram.** Em **Meu Perfil › Telegram**, clique em
   **Conectar**, envie `/start` para o bot **@V3RCondoBot** e volte ao
   aplicativo — o cartão passa a mostrar *Conectado*.
2. **Ligue "Permitir ações por mensagem".** Esse interruptor fica desligado
   por padrão e é diferente de só *receber avisos*: ele autoriza o bot a
   **consultar e gravar** informações a seu pedido. Antes de ligar, o
   aplicativo mostra um aviso explicando o que muda — leia antes de
   confirmar. Você pode desligar a qualquer momento, e o efeito é imediato.

   ![Cartão de conexão com o Telegram em Meu Perfil, mostrando o status Conectado e o interruptor Permitir ações por mensagem ligado](/assets/screenshots/perfil-telegram-01.png)

   *Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*
3. **Confira a franquia.** Em **Configurações → Seu Plano**, o card mostra
   quantas mensagens já foram usadas no mês — por exemplo, *"7 de 50
   mensagens neste mês · renova em 01/10/2026"*. É a mesma contagem que o
   bot usa para decidir se atende ou não.

   ![Card Seu Plano, em Configurações, com a linha Ações pelo Telegram mostrando quantas mensagens já foram usadas no mês e a data de renovação](/assets/screenshots/config-plano-telegram-01.png)

   {: .tip }
   > **A franquia acabou? Dá para ampliar**
   >
   > Clicando em **Mensagens do assistente**, no mesmo card, você contrata um
   > pacote mensal (que soma mensagens todo mês) ou compra uma recarga avulsa
   > (pagamento único, válida por 12 meses). Veja como funciona em
   > [Mensagens do assistente](/modulos/configuracoes/#mensagens-do-assistente).

{: .note }
> **Nem toda conversa consome a franquia**
>
> A franquia conta **mensagens interpretadas** — o pedido em si. Tocar num
> botão de confirmação, responder a uma pergunta do bot, escolher uma opção
> ou receber um aviso de erro nosso **não** consome mensagem. Veja a lista
> completa mais abaixo, em [O que conta na franquia](#o-que-conta-na-franquia).

## Em qual condomínio o bot está trabalhando

Se você administra só um condomínio no Pro, o bot já sabe qual é. Se
administra mais de um, ele pergunta antes de fazer qualquer coisa, com um
botão para cada condomínio — **tocar num nome não gasta franquia**.

A escolha vale por **2 horas** sem você mandar mensagem; depois disso o bot
pergunta de novo, para não agir no condomínio errado por engano. Duas formas
de trocar antes das 2 horas:

- **Cite o nome do condomínio na própria frase** — "quanto tem em caixa no
  Jardim das Flores?" já resolve, sem perguntar.
- **Peça para trocar** — "trocar de condomínio" (ou variações como "mudar
  de condomínio", "outro condomínio") mostra os botões de novo, a qualquer
  momento.

![Bot perguntando em qual condomínio trabalhar, com um botão para cada condomínio que você administra](/assets/screenshots/telegram-condominio-01.png)

{: .warning }
> **Lançou no condomínio errado?**
>
> A confirmação, antes de gravar, sempre mostra o nome do condomínio na
> primeira linha. É o momento de conferir — depois de confirmado, a
> correção é pelo aplicativo, como qualquer lançamento.

## O que você pode perguntar

Fale como falaria com uma pessoa — o bot entende o pedido, não um comando
fixo. Alguns exemplos:

| Você pergunta | O bot responde |
|---|---|
| "Quanto tem em caixa?" | Saldo de cada conta bancária e o total |
| "Quem está devendo?" | Inadimplência por unidade |
| "O que vence essa semana?" | Lançamentos em aberto com vencimento no período — não inclui o que já venceu, a não ser que você peça "vencidos" |
| "Como está a unidade 302 em setembro?" | Situação da unidade numa competência: pago, em aberto ou vencido |
| "Tem solicitação em aberto?" | Solicitações de moradores ainda não resolvidas |
| "Quais as reservas da próxima semana?" | Reservas de áreas comuns no período |
| "Quanto entrou e saiu esse mês?" | Resumo do período — entradas, saídas e resultado |
| "Tem tarefa atrasada?" | Tarefas em aberto, marcando as atrasadas |
| "Qual o telefone do eletricista?" | Contatos do condomínio e fornecedores cadastrados que casam com a busca |

![Resposta do bot a "quanto tem em caixa?", mostrando o saldo de cada conta e o total](/assets/screenshots/telegram-saldos-01.png)

![Resposta do bot a "o que vence nos próximos 7 dias?", listando os lançamentos em aberto no período](/assets/screenshots/telegram-vencimentos-01.png)

{: .note }
> **"O que vence" e "vencidos" não são a mesma coisa**
>
> Por padrão, "o que vence" mostra só o que ainda não venceu, dos próximos 7
> dias. Para incluir o que já passou do vencimento, peça explicitamente —
> "o que venceu" ou "o que está vencido".

### Continuar a conversa sem repetir tudo

Depois de uma consulta, você pode só trocar um detalhe — o bot entende que
é a mesma pergunta, com outro alvo, **sem gastar franquia de novo**:

- Você: "quanto tem em caixa no Jardim das Flores?"
- Bot: responde os saldos.
- Você: "e no Vila Nova?"
- Bot: repete a mesma consulta, agora no Vila Nova — sem acionar a
  inteligência artificial de novo.

Funciona para trocar o condomínio ou o período ("e no mês passado?", "e no
mês que vem?"). **Não funciona para gravação** — lançar e dar baixa sempre
pedem o pedido completo de novo, nunca repetem uma gravação anterior por
continuação.

## Lançar uma despesa ou receita

Você pode descrever o lançamento em texto, mandar uma **foto** do boleto ou
comprovante, ou enviar o **PDF** do documento — o bot lê os dados impressos
(valor, vencimento e uma descrição) e usa como ponto de partida.

**Exemplo, por texto:**

> Você: "lançar uma despesa de manutenção do elevador, R$ 850, vencimento
> dia 20"
>
> Bot: "Qual é a categoria desse lançamento?" (com botões: Manutenção,
> Limpeza, Segurança, Energia, Água, Outras despesas)
>
> Você: toca em **Manutenção**
>
> Bot:
> *Vou gravar este lançamento:*
> *• Condomínio: Jardim das Flores*
> *• Tipo: Saída*
> *• Descrição: manutenção do elevador*
> *• Valor: R$ 850,00*
> *• Vencimento: 20/09/2026*
> *• Categoria: Manutenção*
> *• Conta bancária: Principal*
> *• Situação: a pagar*
> *Confirma? Vale por 15 minutos.*

Toque em **Confirmar** (ou responda "sim") para gravar, ou **Cancelar** (ou
"não") para descartar — nada é gravado até você confirmar.

**Exemplo, por foto de boleto:**

Mande a foto e, se quiser, uma legenda como "lance essa despesa". O bot lê
o valor, o vencimento e monta uma descrição a partir do documento, chega à
mesma confirmação acima e **anexa o comprovante ao lançamento** — você não
precisa anexar depois pelo aplicativo.

![Bot perguntando a categoria do lançamento depois de ler um PDF, com a categoria sugerida pelo documento aparecendo primeiro entre os botões](/assets/screenshots/telegram-categoria-01.png)

![Confirmação do lançamento com todos os campos preenchidos a partir do PDF — condomínio, valor, vencimento e categoria escolhida](/assets/screenshots/telegram-lancamento-confirmacao-01.png)

![Bot confirmando que o lançamento foi criado e que o comprovante foi anexado a ele](/assets/screenshots/telegram-lancamento-criado-01.png)

### O que o bot sempre pergunta, e o que ele assume

- **Categoria — sempre perguntada quando você não diz.** O bot nunca
  escolhe a categoria sozinho, nem quando o documento traz uma pista clara
  (por exemplo, uma conta de água). A pista lida no documento aparece
  **primeiro** na lista de botões, mas quem escolhe é você. Se o condomínio
  ainda não tem nenhuma categoria de entrada ou de saída cadastrada, o bot
  avisa e pede para cadastrar pelo aplicativo antes — sem gravar nada.
- **Conta bancária — usa a conta padrão quando você não diz.** Se o
  condomínio tem mais de uma conta e nenhuma é a padrão, o bot pergunta.
- **Unidade — só quando você diz.** O bot nunca deduz a unidade a partir de
  um nome impresso no boleto. Se você não mencionar unidade e a categoria
  não exigir uma (categorias de inadimplência exigem), o lançamento fica
  **sem unidade** — que é a opção correta na maioria dos lançamentos gerais
  do condomínio.
- **"Já paguei"** — diga isso na hora do pedido ("já paguei ontem", "paguei
  dia 10") e o lançamento já nasce **pago**, com a data informada. Sem essa
  informação, o lançamento nasce a pagar.

{: .warning }
> **A confirmação vale 15 minutos**
>
> Depois desse prazo, o pedido expira e o botão de confirmar para de
> funcionar — o bot avisa "esse pedido já foi concluído ou expirou" e nada
> é gravado. Peça de novo.

## Dar baixa (marcar como pago)

Diga o que basta para encontrar o lançamento — descrição, unidade,
competência ou valor:

> Você: "dar baixa no boleto da Claro, paguei hoje"

Se houver um único lançamento em aberto compatível, o bot já mostra a
confirmação. Se houver mais de um parecido, ele lista em **botões** para
você escolher qual:

> Bot: "Encontrei mais de um lançamento em aberto. Qual deles?"
> [Conta de telefone — R$ 189,90 — venc. 10/09]
> [Conta de internet — R$ 145,00 — venc. 12/09]

Depois de escolher (ou se só havia um), a confirmação mostra o lançamento e
pede o mesmo **Confirmar / Cancelar** de qualquer gravação.

![Confirmação de baixa, mostrando o lançamento encontrado, o valor e a data de pagamento informada](/assets/screenshots/telegram-baixa-confirmacao-01.png)

![Bot confirmando que a baixa foi registrada](/assets/screenshots/telegram-baixa-registrada-01.png)

## Se uma pergunta aparecer no meio do caminho

O bot só pergunta o que falta para completar o pedido — nunca reinicia a
conversa. Responder a pergunta **completa** o pedido de onde ele parou, e
**não conta de novo na franquia**. A qualquer momento, diga "cancelar" (ou
responda "não") para descartar o que estava em andamento — o rascunho é
apagado de verdade, não fica marcado como cancelado em lugar nenhum.

Se você mandar algo que claramente é **outro pedido** no meio de uma
pergunta pendente (por exemplo, começar com "lançar…" ou "quanto tem…"
enquanto o bot esperava uma categoria), o bot descarta o pedido anterior,
avisa que descartou, e atende o novo.

![Confirmação de lançamento com todos os campos preenchidos, antes de tocar em Cancelar](/assets/screenshots/telegram-confirmacao-completa-01.png)

![Bot confirmando que o pedido foi cancelado e que nada foi gravado](/assets/screenshots/telegram-cancelado-01.png)

## Mensagens de voz

Você pode falar em vez de digitar — envie um áudio pelo Telegram como
faria numa mensagem de voz normal. O bot ouve, entende o pedido e segue o
mesmo fluxo de qualquer outra mensagem (pergunta o que falta, pede
confirmação para gravar, e assim por diante).

## Arquivos que o bot não lê

Hoje o bot lê **foto**, **PDF** e **áudio**. Qualquer outro tipo de arquivo
— planilha, documento de texto, vídeo — é **recusado com aviso**, nunca
ignorado em silêncio:

> "Não consigo ler esse tipo de arquivo. Me mande uma foto, um PDF ou
> escreva os dados em texto."

![Bot avisando que não conseguiu ler um arquivo de texto enviado, e pedindo foto, PDF ou os dados digitados](/assets/screenshots/telegram-arquivo-nao-suportado-01.png)

Essa recusa **não consome franquia** — a limitação é nossa, não sua.
Arquivo grande demais (acima de 10 MB) recebe aviso parecido, também sem
gastar mensagem.

## O que conta na franquia

| Conta como mensagem | Não conta |
|---|---|
| Um pedido novo (consulta, lançamento ou baixa) interpretado pelo bot | Tocar em **Confirmar**, **Cancelar** ou numa opção de botão |
| — | Responder a uma pergunta do bot que já estava em andamento |
| — | Escolher o condomínio nos botões |
| — | Continuar uma consulta anterior ("e no mês passado?") |
| — | Arquivo recusado (tipo não suportado ou grande demais) |
| — | Erro ou indisponibilidade nossa (falha ao interpretar, ao consultar, etc.) |
| — | Pedido que expirou ou toque duplicado num botão já usado |

Em resumo: você paga franquia pelo **pedido em si**, não pela conversa
inteira em volta dele.

## Segurança e privacidade

- **Nada é gravado sem você confirmar.** Toda gravação — lançar ou dar
  baixa — passa pela tela de confirmação com todos os campos, e só grava
  depois do seu "Confirmar".
- **O bot só faz o que você já pode fazer pelo aplicativo.** As permissões
  são as mesmas do seu papel — ele não amplia o que você pode ver ou
  alterar.
- **Fica tudo registrado.** Toda gravação feita pelo assistente aparece na
  trilha de auditoria do condomínio com o **seu nome** como autor e o canal
  **Telegram** identificado — do mesmo jeito que uma alteração feita pela
  tela.
- **Desligar o interruptor interrompe na hora.** Com "Permitir ações por
  mensagem" desligado, o bot só responde que a opção está desligada — não
  consulta nem grava nada, mesmo que você mande um pedido.
- **O conteúdo da conversa não fica guardado depois de atender o pedido.**
  Para entender a mensagem, o texto (ou a foto, o PDF ou o áudio) é enviado
  a um provedor de inteligência artificial, que não usa esse conteúdo para
  treinar modelos — o V3RCondo não mantém esse conteúdo depois de responder.

## Dicas e armadilhas

- **Diga a unidade só quando o lançamento for de uma unidade específica.**
  Deixar o bot "adivinhar" a partir de um nome impresso no boleto é
  exatamente o que ele **não** faz — e é assim que se evita lançamento
  preso à unidade errada.
- **Confira o resumo antes de confirmar**, especialmente o condomínio e o
  valor. Depois de confirmado, corrigir é como corrigir qualquer
  lançamento: pelo aplicativo.
- **Frases curtas funcionam melhor que uma lista de instruções.** "lançar
  taxa de jardinagem, R$ 400, vencimento dia 5" resolve mais rápido que uma
  explicação longa.
- **A franquia é por condomínio, não por pessoa.** Se mais de um síndico ou
  subsíndico usa o bot no mesmo condomínio, as mensagens de todos somam na
  mesma conta de 50.

## Quando dá errado

| O bot diz | O que significa | O que fazer |
|---|---|---|
| "Não reconheci esta conversa. Conecte o Telegram no seu perfil…" | Sua conta do Telegram não está vinculada ao seu usuário no V3RCondo | Conecte em **Meu Perfil › Telegram** |
| "As ações por mensagem estão desligadas…" | O interruptor **Permitir ações por mensagem** está desligado | Ligue em **Meu Perfil › Telegram** — o app pode continuar usado normalmente enquanto isso |
| "As ações por mensagem fazem parte do plano Pro…" | O condomínio não está no Pro (ou você não tem papel com ações disponíveis) | Assine o Pro em **Configurações → Condomínio**, ou continue usando o aplicativo normalmente |
| "Vocês já usaram as 50 mensagens do mês…" (com um link) | A franquia (e eventual pacote ou recarga) do condomínio acabou | Toque no link para abrir **Mensagens do assistente** e contratar um pacote ou uma recarga, ou use o aplicativo até a franquia renovar — a data aparece na própria mensagem |
| "Esse pedido já foi concluído ou expirou." | Você confirmou depois dos 15 minutos, ou tocou de novo num botão já usado | Peça de novo |
| "Não entendi o pedido…" | O bot não conseguiu associar sua frase a nenhuma das ações que ele faz | Tente reformular, ou veja a lista de exemplos acima |
| "Não consigo ler esse tipo de arquivo…" | O arquivo enviado não é foto, PDF nem áudio | Mande em um desses formatos, ou escreva os dados em texto |
| "Não consigo processar sua mensagem agora. Tente de novo em instantes." | Falha temporária nossa ao interpretar a mensagem | Tente de novo em alguns instantes — não consumiu sua franquia |
| "Só atendo em conversa privada. Me chame direto, sem grupo." | Você mandou a mensagem num grupo do Telegram, não na conversa direta com o bot | Fale com o **@V3RCondoBot** diretamente, fora de grupos |

## Para o condômino

Você também pode falar com o V3RCondo pelo Telegram — mas só sobre a **sua
própria unidade**: sua segunda via, sua situação de pagamento, suas
reservas, os avisos do mural e suas solicitações. É útil para conferir o
boleto do mês sem abrir o aplicativo, ou para ver se uma reserva foi
aprovada enquanto você está na rua.

O condômino **não lança nem dá baixa em nada** pelo Telegram — essas ações
continuam sendo só do síndico, mesmo que você peça. O bot também não
consulta dados de outras unidades nem do condomínio como um todo: ele só
enxerga o que já é seu dentro do aplicativo.

### Antes de começar

1. **O síndico precisa habilitar o recurso primeiro.** Enquanto ele não
   liberar o assistente para os condôminos, em **Mensagens do assistente**
   (veja [Para o síndico](#para-o-síndico), acima), o interruptor no seu
   perfil fica indisponível — veja [Quando dá errado](#quando-dá-errado-1),
   abaixo.
2. **Conecte o Telegram.** Em **Meu Perfil › Telegram**, clique em
   **Conectar**, envie `/start` para o bot **@V3RCondoBot** e volte ao
   aplicativo — o cartão passa a mostrar *Conectado*.
3. **Ligue "Permitir ações por mensagem".** O aplicativo mostra o aviso do
   que muda antes de você confirmar — leia antes de ligar. Você pode
   desligar a qualquer momento, e o efeito é imediato.

   ![Cartão de conexão com o Telegram em Meu Perfil de um condômino, mostrando o status Conectado, o interruptor Permitir ações por mensagem e a franquia do mês](/assets/screenshots/perfil-telegram-condomino-01.png)

   *Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

{: .note }
> **Se você participa de mais de um condomínio**
>
> O bot pergunta em qual condomínio trabalhar antes de responder, do mesmo
> jeito descrito em [Em qual condomínio o bot está
> trabalhando](#em-qual-condomínio-o-bot-está-trabalhando) — só que a lista
> mostra apenas os condomínios em que o síndico já habilitou o assistente
> para os condôminos.

### O que você pode perguntar

| Você pergunta | O bot responde |
|---|---|
| "Manda a segunda via do meu boleto" | Cobranças em aberto da sua unidade: valor, vencimento, link da fatura, linha digitável e Pix copia e cola |
| "Como está minha unidade?" | Situação de pagamento da sua unidade: o que está em aberto, vencido ou foi pago recentemente |
| "Quais são minhas reservas?" | Suas próprias reservas futuras de áreas comuns |
| "Tem aviso novo no mural?" | Avisos recentes do mural do condomínio — os mesmos que o síndico vê |
| "Como estão minhas solicitações?" | Suas solicitações em aberto |

**Exemplo concreto:**

> Você: "manda a segunda via do meu boleto"
>
> Bot:
> *Suas cobranças em aberto*
> *• R$ 480,00 — vencimento 10/10/2026*
> *Fatura: https://…*
> *Linha digitável: `85670000...`*
> *Pix copia e cola: `00020126...`*

Se a sua unidade não tiver cobrança em aberto, o bot responde "Você não tem
cobranças em aberto" — e essa resposta **conta na franquia**, porque a
mensagem foi interpretada mesmo sem achar nada.

{: .note }
> **Falar é o mesmo que consultar pelo aplicativo**
>
> As respostas vêm exatamente da mesma informação que aparece em [Minha
> Área](/modulos/minha-area/) e nas demais telas do condômino — o bot não
> enxerga nada a mais nem a menos do que você já vê logado.

### Franquia própria, sem compra

Diferente da franquia do síndico, a sua é **pessoal**: **20 mensagens por
mês**, por condômino, incluídas no plano Pro do condomínio. Ela:

- **não soma com a de outros condôminos** nem com a franquia do
  condomínio — cada condômino tem a própria conta de 20;
- **não tem pacote nem recarga.** Esgotada, você espera a renovação do mês
  seguinte; não há botão de comprar mais;
- **conta só o pedido interpretado**, do mesmo jeito descrito para o
  síndico em [O que conta na franquia](#o-que-conta-na-franquia): tocar em
  um botão, responder a uma pergunta pendente ou receber um erro nosso não
  consome mensagem.

Para conferir quantas você já usou no mês, veja o cartão **Telegram**, em
**Meu Perfil** — a contagem aparece ali, logo abaixo do interruptor.

### O que o condômino não pode fazer

O bot recusa qualquer pedido de gravação ou de gestão vindo de um
condômino — lançar, dar baixa, editar cadastro de outra pessoa, ver
inadimplência do condomínio inteiro — mesmo que o pedido seja claro:

> Você: "lança uma despesa de R$ 100 de material de limpeza"
>
> Bot avisa que, por mensagem, você só faz consultas, e que para essa ação
> é preciso usar o aplicativo.

Essas ações continuam existindo — só não pelo Telegram. Abra o aplicativo
para fazer o que o bot recusou.

### Dicas e armadilhas

- **Frases curtas funcionam melhor.** "segunda via do meu boleto" resolve
  mais rápido que uma pergunta longa.
- **Pergunta fora do que o bot faz também conta na franquia.** Se você
  pedir algo que ele não entende, a mensagem foi interpretada mesmo sem
  resultado — reformule antes de repetir, para não gastar franquia à toa.
- **A franquia não se acumula de um mês para o outro.** Mensagem não usada
  em setembro não vira duas em outubro.

### Dúvidas frequentes

**O síndico vê as mensagens que eu mando para o bot?**
Não. A trilha do condômino é separada da do síndico: o bot só enxerga as
suas próprias informações, e o síndico não recebe nem lê o conteúdo das
suas conversas.

**Minha franquia soma com a do condomínio?**
Não. São duas contas separadas — a sua, de 20 mensagens, e a do
condomínio, de 50. Uma acabar não afeta a outra.

**Posso pedir ao bot para lançar ou cancelar algo por mim?**
Não — condômino não grava nada pelo Telegram. O bot recusa e indica o
aplicativo, mesmo que você repita o pedido de outro jeito.

### Quando dá errado {#quando-dá-errado-1}

| O bot diz | O que significa | O que fazer |
|---|---|---|
| "O síndico do seu condomínio ainda não liberou o assistente por mensagem para os condôminos." | O condomínio não tem **Mensagens do assistente → Permitir o assistente por mensagem para os condôminos** ligado | Peça ao síndico para habilitar, ou continue usando o aplicativo normalmente |
| "Não reconheci esta conversa. Conecte o Telegram no seu perfil…" | Sua conta do Telegram não está vinculada ao seu usuário no V3RCondo | Conecte em **Meu Perfil › Telegram** |
| "As ações por mensagem estão desligadas…" | O interruptor **Permitir ações por mensagem** está desligado no seu perfil | Ligue em **Meu Perfil › Telegram** |
| "Você já usou as 20 mensagens do mês. Elas renovam em…" | Sua franquia pessoal acabou | Espere a renovação (a data vem na própria mensagem), ou use o aplicativo |
| "Seu cadastro ainda não tem unidade vinculada. Fale com o síndico." | Sua conta de condômino não está vinculada a nenhuma unidade | Peça ao síndico para vincular sua unidade em **Configurações → Condôminos** |
| "Por mensagem, você pode fazer consultas. Para \[ação\], use o aplicativo." | Você pediu algo que só o síndico pode fazer | Abra o aplicativo para essa ação |
| "Não entendi o pedido…" | O bot não conseguiu associar sua frase a nenhuma das consultas que ele faz | Reformule, ou veja a lista de exemplos acima |
| "Esse pedido já foi concluído ou expirou." | Você tocou de novo num botão já usado | Peça de novo |
| "Não consigo processar sua mensagem agora. Tente de novo em instantes." | Falha temporária nossa ao interpretar a mensagem | Tente de novo em alguns instantes — não consumiu sua franquia |
| "Só atendo em conversa privada. Me chame direto, sem grupo." | Você mandou a mensagem num grupo do Telegram, não na conversa direta com o bot | Fale com o **@V3RCondoBot** diretamente, fora de grupos |

## Glossário

**Franquia** — o limite de mensagens interpretadas pelo bot por mês. Existem
**duas**, independentes: a do **condomínio** (síndico), de **50 mensagens**,
ampliável por pacote mensal ou recarga avulsa em [Mensagens do
assistente](/modulos/configuracoes/#mensagens-do-assistente); e a do
**condômino**, pessoal, de **20 mensagens**, sem pacote nem recarga. As duas
reiniciam automaticamente todo mês.

**Pedido pendente** — um lançamento ou baixa que o bot já entendeu e está
aguardando sua confirmação (ou uma resposta a uma pergunta) antes de
gravar. Expira em 15 minutos. *(Só se aplica ao síndico — o condômino não
grava nada.)*

**Ações por mensagem** — o interruptor, em **Meu Perfil › Telegram**, que
autoriza o bot a consultar (e, para o síndico, também gravar) a seu pedido.
Diferente de *receber avisos*, que é só entrega de notificações (veja
[Notificações](/modulos/notificacoes/)).
