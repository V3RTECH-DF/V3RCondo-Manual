---
title: Abrir a conta de cobrança
parent: Fluxos
nav_order: 5
---

# Abrir a conta de cobrança

## Por que isto importa

A partir do momento em que a conta de cobrança está aprovada, o boleto e o Pix da cota saem sozinhos todo mês, e a baixa no Financeiro acontece sem ninguém precisar conferir nada à mão — é o que torna possível o fluxo [Cobrar a cota do mês](/fluxos/cobrar-a-cota/). Mas a abertura em si tem duas autorizações formais, documentos que precisam estar prontos com antecedência, e uma aprovação que depende de terceiro — o Asaas, a instituição de pagamento. Saber a ordem certa evita a espera mais comum: mandar o cadastro e descobrir só depois que faltava a ata registrada em cartório.

## Passo a passo

### 1. Aceite o Contrato de Prestação de Serviços — pré-requisito

Antes de qualquer outra coisa, o síndico precisa aceitar, em nome do condomínio, o **Contrato de Prestação de Serviços**, em [Configurações → Condomínio](/modulos/configuracoes/#contrato-de-prestação-de-serviços). Sem ele, a tela de Cobrança automática mostra só o aviso do que falta, no lugar do formulário de abertura.

{: .note }
> **Não é o mesmo aceite dos Termos de Uso**
>
> Este contrato é diferente do Termos de Uso que cada pessoa aceita no primeiro acesso, e diferente também do Termo de Autorização que vem no passo seguinte. Ver [Configurações — Contrato de Prestação de Serviços](/modulos/configuracoes/#contrato-de-prestação-de-serviços).

### 2. Separe os documentos antes de começar o cadastro

O passo que mais atrasa a aprovação é a **ata de eleição da diretoria vigente, registrada em cartório** — ata sem esse registro é recusada, e registrar leva dias ou semanas. Tenha em mãos, ou a caminho, antes de prosseguir:

- Ata de eleição registrada em cartório
- Documento de identidade do síndico, frente e verso
- Acesso à caixa de e-mail cadastrada do condomínio — é para lá que o Asaas manda o link de criar senha, e ele expira em 10 minutos

### 3. Preencha o cadastro

Em **Cobrança automática**, preencha o formulário **Dados para abrir a conta**: quem é o titular (condomínio ou pessoa física), nome/razão social, CNPJ ou CPF, e-mail, celular, faturamento mensal estimado e endereço. Nenhum documento é enviado por aqui — isso acontece depois, direto no painel do Asaas.

### 4. Aceite o Termo de Autorização — Conta de Pagamento

Depois de preencher, aparece o **Termo de Autorização — Conta de Pagamento**, com dois consentimentos separados: autorizar a abertura e operação da conta, e consentir com a criação da chave Pix. As duas caixas precisam estar marcadas — marcar só uma não libera o botão **Aceitar e abrir a conta**. Ver o texto completo em [Cobrança Automática — Autorizar a abertura da conta](/modulos/cobranca-automatica/#autorizar-a-abertura-da-conta).

### 5. Crie a senha no Asaas e envie a documentação

O que falta acontece do lado do Asaas, fora do V3RCondo:

1. O Asaas envia, ao e-mail cadastrado, um link para **criar a senha** — válido por **10 minutos**.
2. O acesso pede um **código por SMS**.
3. Dentro do painel do Asaas, envie a documentação pedida, incluindo o **reconhecimento facial**.

### 6. Acompanhe a aprovação

Volte à tela de Cobrança automática quando quiser conferir: o cartão **Situação da conta** mostra três indicadores — **Dados comerciais**, **Documentação** e **Dados bancários** — cada um como Pendente, Em análise, Aprovado ou Reprovado. Você também recebe um e-mail em cada uma das três viradas (cadastro enviado, conta aprovada, cadastro recusado), então não precisa ficar voltando à tela por conta própria.

### 7. Confirme que está pronto para cobrar

Com a conta aprovada, a tela passa a mostrar três abas — **Cobranças**, **Emitir** e **Ajustes**. Isso é a confirmação: se essas três abas apareceram, a conta está operacional e o próximo [ciclo de cota](/fluxos/cobrar-a-cota/) já vai emitir cobranças automaticamente.

![Cobrança automática com as três abas Cobranças, Emitir e Ajustes, a confirmação de que a conta está aprovada e operacional](/assets/screenshots/fluxo-abrir-conta-01-tres-abas.png)

### 8. Leia o que não mexer no painel do Asaas

A conta aprovada vem com acesso a um painel próprio do Asaas, bem mais amplo do que o V3RCondo usa. Antes de explorar esse painel, leia [O que o síndico não deve mexer no painel do Asaas](/modulos/asaas-painel/) — chave de API e webhook são duas configurações que sustentam esta integração sem que o painel avise disso.

## Exemplo concreto

O síndico do Edifício Aurora já tem a ata de eleição registrada em cartório e o CPF em mãos. Ele aceita o Contrato de Prestação de Serviços, preenche o cadastro da conta, marca os dois consentimentos do Termo de Autorização e confirma. No dia seguinte, recebe o e-mail "Cadastro enviado" — cria a senha no Asaas, confirma pelo SMS, e envia a ata, o RG e a selfie no painel deles. Quatro dias depois, chega o e-mail "Conta aprovada", e as três abas — Cobranças, Emitir, Ajustes — aparecem na tela.

## Dicas e armadilhas

- **Registre a ata em cartório antes de começar o cadastro**, não depois de ser recusada. É o item que mais atrasa a aprovação, e o atraso é medido em dias ou semanas, não em horas.
- **Um documento recusado obriga a reenviar todos, não só o que falhou.** Confira nitidez, validade e legibilidade de cada arquivo antes de enviar, para não ter que repetir o que já estava certo.
- **Recusar o Termo de Autorização não trava nada.** O botão **Agora não** simplesmente fecha o termo — o condomínio continua lançando e recebendo a cota como sempre fez, e você pode voltar e aceitar quando quiser.
- **Abrir a conta é opcional.** Nada obriga o condomínio a ter Cobrança Automática — sem ela, o [fluxo de cobrar a cota](/fluxos/cobrar-a-cota/) continua funcionando, só sem boleto e Pix automáticos.

## Quando dá errado

| O que você vê | O que fazer |
|---|---|
| Tela mostra só o aviso do Contrato de Prestação de Serviços | Aceite o contrato em Configurações → Condomínio antes de tentar abrir a conta |
| Link de criar senha expirou | Use **"Esqueci minha senha"** na tela de login do Asaas para gerar um novo link |
| E-mail "Cadastro recusado" | O motivo vem do Asaas diretamente — o V3RCondo não o repassa; corrija o que foi apontado e reenvie |
| Indicador **Dados comerciais** aparece com aviso de vencido | As informações comerciais vencem por tempo; volte ao cadastro e atualize o que for pedido |
| Passaram-se muitos dias sem nenhuma virada de status | Confira se a documentação foi de fato enviada dentro do painel do Asaas — é lá que o processo acontece, o V3RCondo só espelha o resultado |
