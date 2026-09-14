---
title: Assistente por Mensagem (Telegram)
parent: Módulos
nav_order: 7.5
---

# Assistente por Mensagem (Telegram)

{: .warning }
> **Plano Pro**
>
> Consultar e lançar pelo Telegram é um recurso do **plano Pro**, com uma
> franquia de **50 mensagens por mês** por condomínio. No plano Básico, o
> Telegram continua disponível — mas só para **receber avisos** (veja
> [Notificações](/modulos/notificacoes/)), não para agir por mensagem.

Além de abrir o aplicativo, você pode falar com o V3RCondo pelo **Telegram**:
perguntar o saldo em caixa, ver quem está devendo, lançar uma despesa a
partir da foto de um boleto ou dar baixa num pagamento — tudo puxando
conversa com o bot, do celular, sem precisar abrir o navegador. É útil
quando você está fora de casa, numa reunião com um fornecedor, ou só quer
resolver algo rápido sem esperar o aplicativo carregar.

O assistente age **com as mesmas permissões que você já tem** no aplicativo
— ele não abre uma porta nova, só encurta o caminho para o que você já
poderia fazer pela tela.

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
| "Vocês já usaram as 50 mensagens do mês…" | A franquia do condomínio acabou | Use o aplicativo até a franquia renovar — a data aparece na própria mensagem |
| "Esse pedido já foi concluído ou expirou." | Você confirmou depois dos 15 minutos, ou tocou de novo num botão já usado | Peça de novo |
| "Não entendi o pedido…" | O bot não conseguiu associar sua frase a nenhuma das ações que ele faz | Tente reformular, ou veja a lista de exemplos acima |
| "Não consigo ler esse tipo de arquivo…" | O arquivo enviado não é foto, PDF nem áudio | Mande em um desses formatos, ou escreva os dados em texto |
| "Não consigo processar sua mensagem agora. Tente de novo em instantes." | Falha temporária nossa ao interpretar a mensagem | Tente de novo em alguns instantes — não consumiu sua franquia |
| "Só atendo em conversa privada. Me chame direto, sem grupo." | Você mandou a mensagem num grupo do Telegram, não na conversa direta com o bot | Fale com o **@V3RCondoBot** diretamente, fora de grupos |

## Glossário

**Franquia** — o limite de mensagens interpretadas pelo bot por mês, por
condomínio. Reinicia automaticamente na data de renovação mostrada em
**Configurações → Seu Plano**.

**Pedido pendente** — um lançamento ou baixa que o bot já entendeu e está
aguardando sua confirmação (ou uma resposta a uma pergunta) antes de
gravar. Expira em 15 minutos.

**Ações por mensagem** — o interruptor, em **Meu Perfil › Telegram**, que
autoriza o bot a consultar e gravar a seu pedido. Diferente de *receber
avisos*, que é só entrega de notificações (veja
[Notificações](/modulos/notificacoes/)).
