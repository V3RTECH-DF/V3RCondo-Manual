---
title: Conferir o extrato e conciliar
parent: Fluxos
nav_order: 4
---

# Conferir o extrato e conciliar

## Por que isto importa

Dar baixa num lançamento confirma que o dinheiro entrou ou saiu — mas não confirma que aquele lançamento é, **de fato**, a mesma transação que aparece no extrato do banco. Duas pessoas podem ter dado baixa em lançamentos parecidos por engano, um pagamento pode ter caído em outra conta, uma tarifa pode nunca ter sido lançada. Conferir contra o extrato é a segunda checagem — a que o Conselho Fiscal e o contador esperam encontrar pronta na hora de revisar as contas.

Há dois caminhos, e a escolha depende do que você tem em mãos: o **arquivo** do extrato (OFX ou CSV), ou só o **número** do saldo, de um extrato impresso ou em PDF.

## Passo a passo

### 1. Você tem o arquivo do extrato? Importe e concilie transação a transação

No [Financeiro → Importar extrato](/modulos/financeiro/#conciliar-com-o-extrato-bancário-síndico--plano-pro):

1. Clique em **Importar extrato**, escolha a conta de destino e envie o arquivo OFX ou CSV.
2. O app compara cada linha com os lançamentos daquela conta: **casa sozinho** quando só há um candidato compatível, **pede para você decidir** quando há mais de um ou o valor é parecido mas não idêntico, e **vira lançamento novo** quando não há nada parecido.
3. Revise as pendências e confirme cada uma.
4. Clique em **Concluir importação**.

Cada lançamento conciliado ganha o selo **Conciliado com o extrato**, visível no [detalhe do lançamento](/modulos/financeiro/#ver-os-detalhes-de-um-lançamento) — uma marca separada da situação **Pago**: um lançamento pode estar pago e ainda não conciliado, e é exatamente essa combinação que interessa ao Conselho Fiscal no fechamento do mês.

{: .tip }
> **Reimportar o mesmo arquivo é seguro**
>
> Uma linha já registrada numa importação anterior não entra de novo. Pode reimportar um período inteiro sem medo de duplicar.

### 2. Sem o arquivo? Use o caça-diferenças

Quando você só tem o extrato impresso, em PDF, ou simplesmente sabe o saldo que o banco mostra, não precisa do arquivo para conferir. No [Financeiro](/modulos/financeiro/), clique na lupa 🔍 ao lado da conta e use o **[Caça-diferenças](/modulos/caca-diferencas/)**:

1. Informe o **saldo do banco** e a **data** desse saldo.
2. O app calcula a diferença entre o que ele tem registrado e o que você informou.
3. Sem diferença, aparece **"Tudo batendo ✅"**. Com diferença, o app lista as hipóteses mais prováveis — duplicata, lançamento que explica o valor, lançamento na conta errada, valor quase igual (tarifa, IOF) — da mais provável para a menos provável.
4. Aplique a correção sugerida em cada hipótese e veja a diferença recalcular na hora, até zerar.

### 3. Confira o resultado

Depois de conciliar (ou zerar a diferença pelo caça-diferenças), confirme que o saldo do painel **Contas**, no topo do Financeiro, bate com o saldo real do extrato na mesma data. É essa comparação — não a tela dizendo "importação concluída" — que prova que o mês fechou certo.

![Painel do Caça-diferenças com o saldo do banco informado, a diferença zerada e a mensagem "Tudo batendo — buraco fechou"](/assets/screenshots/fluxo-conciliar-01-tudo-batendo.png)

## Exemplo concreto

O síndico do Residencial Aurora recebe o extrato de setembro em PDF do banco, sem conseguir baixar o OFX. Em vez de tentar converter o arquivo, ele abre o Caça-diferenças da conta corrente, informa o saldo de R$ 24.680,00 do dia 30/09, e o app aponta uma diferença de R$ 45,00 — uma tarifa bancária nunca lançada. Ele cria o lançamento sugerido, já pré-preenchido com o valor, e a diferença zera.

## Dicas e armadilhas

- **Pagamento fora da data do vencimento também é reconhecido na importação** — uma conta que vence dia 10 e é paga dia 25 casa normalmente. Não é preciso ajustar nada para isso.
- **Conciliar dá baixa com a data do extrato, mesmo que o lançamento já estivesse marcado como pago com outra data.** É a data real do dinheiro se movendo que prevalece — a correção aparece no resumo da importação.
- **Desfazer uma conciliação não desfaz a baixa.** Use quando a conciliação casou com o lançamento errado; o lançamento continua pago, só perde a marca de conferido.
- **Cobranças legitimamente repetidas** (a mesma taxa em várias unidades, por exemplo) não são confundidas com duplicata pelo caça-diferenças — ele já sabe separar as duas situações.

## Quando dá errado

| O que você vê | O que fazer |
|---|---|
| Uma linha do extrato "vira lançamento novo" que você não esperava | Confira se não é um lançamento que já existe com data ou valor bem diferente do esperado — decida importar como novo ou ignorar a linha |
| O caça-diferenças mostra "Procure no extrato" | Nenhuma hipótese automática explica a diferença — provavelmente falta lançar algo (uma tarifa, um débito ainda não registrado); o app já indica o valor exato a procurar |
| Saldo continua sem bater depois de conciliar tudo | Confira se a data do saldo informado é a mesma da conferência — saldo de datas diferentes nunca vai bater |
| Conciliou o lançamento errado por engano | Abra o detalhe do lançamento e clique em **Desfazer conciliação** — a baixa continua, só a marca de conferido some |
