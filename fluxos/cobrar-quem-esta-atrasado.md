---
title: Cobrar quem está atrasado
parent: Fluxos
nav_order: 7
---

# Cobrar quem está atrasado

## Por que isto importa

Inadimplência que não é tratada com um processo claro tende a duas coisas ruins: virar constrangimento pessoal entre síndico e vizinho, ou se acumular até um valor que ninguém mais consegue pagar de uma vez. O V3RCondo trata isso como uma escada, não como um evento único — do lembrete automático mais leve até a notificação formal e o parcelamento, cada degrau dá ao morador uma chance de resolver antes do próximo.

**A notificação extrajudicial e o acordo de parcelamento são recursos do plano Pro.** No Básico, você visualiza quem está devendo, mas as ações de recuperação ficam bloqueadas.

## Passo a passo

### 1. Antes de tudo, os lembretes automáticos já estão cobrando

Se a unidade tem cobrança emitida pela [Cobrança Automática](/modulos/cobranca-automatica/), o morador já recebe uma sequência de avisos por e-mail sem você precisar fazer nada: antes do vencimento (conforme a antecedência configurada), no dia do vencimento, e a cada 7 dias depois de vencida — até 4 avisos, nunca além de 30 dias de atraso. Só depois desse limite o assunto passa a ser tratado como inadimplência formal. Veja a tabela completa em [Cobrança Automática — O que o morador recebe](/modulos/cobranca-automatica/#o-que-o-morador-recebe).

Isso significa: **não duplique o trabalho do sistema.** Cheque a Inadimplência antes de notificar alguém que talvez só esteja nos primeiros dias de atraso, ainda dentro da sequência automática.

### 2. Veja quem está devendo

Abra **Inadimplência → aba Inadimplentes**. A lista mostra as unidades com lançamentos vencidos e não pagos, com o total inadimplente no topo.

{: .warning }
> **Categoria da cota não configurada faz esta tela não apurar nada**
>
> Sem a categoria marcada em [Configurações → Categorias → Financeiro](/modulos/configuracoes/#a-categoria-da-taxa-condominial), a tela avisa que a inadimplência **não pôde ser apurada** — não mostra zero. Se a lista aparece vazia sem explicação, confira essa configuração primeiro.

### 3. Notifique formalmente

Expanda a unidade devedora, marque os lançamentos e clique em **Notificar** — individual, unidade por unidade, ou **Notificar em lote**, para várias de uma vez. Escolha o canal: e-mail, e-mail + Telegram, ou apenas gerar o PDF para download. O documento traz a tabela de débitos, o prazo para regularização e um código de referência para rastreio. Ver [Inadimplência — Notificar devedores](/modulos/inadimplencia/#notificar-devedores-notificação-extrajudicial-pro).

### 4. Ofereça um acordo de parcelamento

Se o morador procurar você para negociar, ou se você preferir oferecer o parcelamento diretamente: na unidade devedora, clique em **Gerar Acordo**, selecione as dívidas que entram na negociação, defina o número de parcelas (1 a 36) e, se quiser, um desconto. Confira o resumo e confirme — o sistema move as dívidas originais para o estado "em acordo" (elas saem da lista de inadimplência, mas não são apagadas) e cria as parcelas novas, já com desconto, como um PDF de acordo com atestação eletrônica.

{: .tip }
> **O morador também pode iniciar sozinho**
>
> Se a **negociação self-service** estiver ativa (parâmetros em [Configurações → Cobranças & Acordos](/modulos/configuracoes/#parâmetros-de-acordo-self-service-plano-pro)), o condômino propõe e fecha o próprio parcelamento pela **Minha Área → Negociar dívida**, sem depender de você — nas mesmas regras e com a mesma quebra automática por descumprimento descritas abaixo.

### 5. Acompanhe o acordo até o fim

Na aba **Acordos**, todos os acordos do condomínio ficam visíveis — inclusive os que já quitaram a dívida inteira da unidade. Conforme o morador paga, expanda o acordo e **Marque como pago** cada parcela. Quando a última é paga, o acordo vira **Concluído** e as dívidas originais são quitadas de vez.

### 6. Saiba o que fazer se o acordo quebrar

Se a unidade acumular **duas parcelas vencidas sem pagamento**, o sistema quebra o acordo sozinho, todo dia: o morador perde o desconto, tudo o que já pagou é abatido do valor original, e a dívida volta a aparecer na Inadimplência com o saldo correto. Você recebe uma notificação quando isso acontece — não precisa ficar conferindo. Um atraso pontual de uma parcela **não** quebra o acordo; ele continua Ativo.

## Exemplo concreto

A unidade 12B do Vale do Cedro deve R$ 1.000,00 de duas cotas vencidas. O síndico gera um acordo com 20% de desconto — R$ 800,00 em 8 parcelas de R$ 100,00. O morador paga 3 parcelas e para. Na segunda parcela vencida sem pagamento, o acordo quebra automaticamente: o desconto some (volta a dever R$ 1.000,00), os R$ 300,00 já pagos são abatidos, e a unidade reaparece na Inadimplência devendo R$ 700,00 — com os R$ 300,00 continuando registrados nas datas em que entraram.

![Aba Acordos da Inadimplência com um acordo no status Quebrado, expandido mostrando a tabela de parcelas](/assets/screenshots/fluxo-atrasados-01-acordo-quebrado.png)

## Dicas e armadilhas

- **Não notifique quem ainda está na janela dos lembretes automáticos.** Confira o histórico de avisos da cobrança antes de partir para a notificação formal — evita cobrar duas vezes pela mesma coisa, de formas diferentes.
- **Perder o desconto ao quebrar o acordo é intencional**, não um bug: é o incentivo para cumprir. Explique isso ao morador na hora de oferecer o parcelamento, para não parecer punição arbitrária depois.
- **Uma unidade que fechou acordo sai da lista de Inadimplentes, mas a dívida não sumiu** — ela está "em acordo". Se você está procurando uma unidade que devia e não a encontra mais na lista, confira a aba Acordos antes de supor que ela quitou.

## Quando dá errado

| O que você vê | O que fazer |
|---|---|
| Tela de Inadimplência diz "não pôde ser apurada" | Marque a categoria da taxa condominial em Configurações → Categorias → Financeiro |
| Total de inadimplência caiu sem ninguém ter pago | Confira se alguma categoria financeira foi excluída recentemente — lançamentos de categoria excluída deixam de contar |
| Acordo quebrou e o morador contesta | Abra o acordo: cada pagamento fica registrado na data em que entrou, e o valor devido é sempre a dívida original menos o total já pago — mostre o extrato do acordo como prova |
| Notificação extrajudicial não chegou ao morador | Confira o canal escolhido (e-mail, e-mail + Telegram) e se o **responsável pela unidade** está correto em Configurações → Condôminos — só ele recebe a notificação |
