---
title: O que o síndico não deve mexer no painel do Asaas
parent: Módulos
nav_order: 3.65
---

# O que o síndico não deve mexer no painel do Asaas

Quem abre a [conta de cobrança](/fluxos/abrir-conta-de-cobranca/) ganha acesso a um **painel próprio do Asaas** — a instituição de pagamento que processa boleto, Pix e cartão em nome do condomínio. É uma conta de pagamento completa, com bem mais opções do que o V3RCondo usa: transferências, extrato, chaves de API, configuração de integrações.

Essa amplitude é útil para acompanhar o dinheiro, mas também deixa ao alcance da mão três configurações que **sustentam a integração com o V3RCondo** — mexer nelas não avisa que vai quebrar algo aqui. Esta página existe para isso: dizer o que evitar, por quê, e o que fazer se acontecer mesmo assim.

{: .note }
> **Confirmado com o suporte do Asaas em 22/09/2026.** Os três pontos abaixo não são suposição nossa — foram respondidos por escrito, depois de perguntarmos especificamente sobre cada um.

## 1. Não mexa nas chaves de API

**O que acontece se você mexer:** trocar ou revogar a chave de acesso da conta derruba a comunicação entre o Asaas e o V3RCondo até alguém colar a chave nova aqui dentro. Enquanto isso durar, o condomínio **para de emitir cobrança nova**, e os pagamentos que já entraram **param de ser reconhecidos** — o morador paga, mas o V3RCondo não fica sabendo, e a cota continua aparecendo em aberto.

**Por que isso existe:** o titular da conta — o condomínio, por meio do síndico — é quem gerencia as próprias chaves de API no painel do Asaas. É assim para qualquer conta de pagamento, e o V3RCondo não tem como impedir o acesso a essa tela: só usa a chave que existe.

**O que fazer se aconteceu:** se você gerou uma chave nova, revogou a antiga, ou simplesmente não sabe se mexeu em algo ali, volte ao [Dashboard](/modulos/dashboard/) do V3RCondo. Se a chave parou de funcionar, o cartão de configuração mostra a linha **"Cobrança automática — falta reconectar a chave"**, com o botão **Reconectar**: gere uma chave nova no painel do Asaas, cole no campo indicado, e a integração volta a funcionar — sem precisar abrir a conta de novo.

## 2. Não edite nem remova webhooks

**O que acontece se você mexer:** o webhook é o canal por onde o Asaas avisa o V3RCondo, em tempo real, que um morador pagou. Apagá-lo — ou editá-lo para outro endereço — corta esse aviso: o pagamento continua acontecendo normalmente do lado do Asaas, mas o V3RCondo **nunca fica sabendo**. A cota do morador continua marcada como em aberto, ele aparece como devedor mesmo tendo pago, e ninguém percebe até o morador reclamar — ou até o síndico, olhando o extrato da conta de cobrança, notar um pagamento que o Financeiro não registrou.

**Por que isso existe:** o painel do Asaas **não distingue** o webhook criado pela integração do V3RCondo de um webhook criado à mão por qualquer outra finalidade — o nosso aparece na lista igual a qualquer outro, editável e removível, sem nenhuma marca. Não há como o Asaas proteger algo que não sabe identificar como "não mexa aqui".

**O que fazer se aconteceu:** entre em contato com o **suporte da V3RTECH** assim que perceber — antes de tentar recriar o webhook você mesmo. Recriar com o endereço ou a configuração errada tem o mesmo efeito de não ter webhook nenhum, só que parece resolvido.

## 3. Durante a análise cadastral, a saída fica bloqueada — não é defeito

Enquanto a conta de cobrança está em análise (documentação em conferência, dados comerciais em validação), duas coisas ficam temporariamente indisponíveis, mesmo com tudo certo do lado do condomínio:

- **A transferência do dinheiro para fora da conta** fica bloqueada.
- **A emissão de nota fiscal** fica suspensa.

**Cobrança e recebimento continuam funcionando normalmente** — o morador paga, a cota é baixada, o dinheiro entra na conta do condomínio. O que trava é só a saída.

**Não é motivo para abrir chamado.** É o comportamento esperado durante a análise, e some sozinho quando ela termina. Se precisar transferir ou emitir nota fiscal com urgência durante esse período, é ao Asaas que se recorre — ver os contatos abaixo — não a um ajuste no V3RCondo, porque a decisão não é nossa.

## Com quem falar

A mesma divisão que vale para o dia a dia da Cobrança Automática vale aqui: assunto de conta, chave, webhook, transferência e nota fiscal é com o **Asaas** — **0800 009 0037** ou **contato@asaas.com.br**. Assunto de como o V3RCondo usa esses dados é com o **suporte da V3RTECH**. Mais sobre essa divisão em [Cobrança Automática — Com quem falar](/modulos/cobranca-automatica/#com-quem-falar-asaas-ou-v3rtech).

{: .tip }
> **A régua mais simples**
>
> Se a tela do Asaas pedir para você criar, editar ou apagar alguma coisa que **não** seja enviar um documento pedido na abertura da conta, pare e pergunte à V3RTECH antes de confirmar. O painel é deles, mas a pergunta "isso vai quebrar alguma coisa aqui?" é nossa para responder.
