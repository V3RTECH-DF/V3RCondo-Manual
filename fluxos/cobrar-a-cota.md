---
title: Cobrar a cota do mês
parent: Fluxos
nav_order: 1
---

# Cobrar a cota do mês

## Por que isto importa

A cota é a receita que sustenta o condomínio todo mês, e é também o lançamento que mais se repete no Financeiro. Feita à mão, ela é oito, vinte ou cem lançamentos idênticos — um por unidade, todo mês, o mesmo risco de esquecer uma ou de digitar o valor errado. Configurada uma vez, ela passa a se gerar sozinha, no dia certo, com o valor certo de cada unidade — e, para quem já tem a Cobrança Automática, o boleto e o Pix saem no mesmo instante, sem o síndico tocar em nada.

Este fluxo é o que amarra três telas que, sozinhas, não contam a história inteira: a taxa configurada em **Configurações**, o lançamento que nasce no **Financeiro**, e a cobrança que sai pela **Cobrança Automática**.

## Antes de começar — configure uma vez

Três coisas precisam estar prontas antes do primeiro ciclo. Depois de configuradas, você não mexe nelas de novo todo mês.

1. **A taxa mensal de cada unidade**, em [Configurações → Unidades](/modulos/configuracoes/#aba-unidades-síndico). Dá para definir uma por uma ou em lote (taxa fixa ou reajuste percentual).
2. **A categoria da taxa condominial**, marcada em [Configurações → Categorias → Financeiro](/modulos/configuracoes/#a-categoria-da-taxa-condominial). Condomínio criado recentemente já nasce com a categoria **Taxas de condomínio** marcada; condomínio mais antigo pode precisar marcar isso à mão.
3. **A aba [Cobranças & Acordos](/modulos/configuracoes/#aba-cobranças--acordos-síndico)**, em Configurações: escolha a categoria de cobrança (a mesma do passo 2), o dia de vencimento, e — se quiser — uma conta bancária padrão para os lançamentos gerados.

O cartão **Configuração inicial**, no topo do [Dashboard](/modulos/dashboard/#configuração-inicial-síndico--condomínio-novo), lista esses mesmos passos com atalho direto para cada um, em condomínios criados a partir de 13/08/2026.

{: .warning }
> **Unidade sem taxa configurada não gera cota nenhuma — e não avisa na hora**
>
> A geração mensal pula, em silêncio, toda unidade sem valor de cota definido. A tela mostra quais unidades ficaram de fora só depois de gerar, e o e-mail que chega ao síndico também nomeia cada uma. Revisite o passo 1 sempre que cadastrar uma unidade nova.

## Passo a passo

### 1. Deixe o app gerar a cota sozinho, ou gere você mesmo este mês

Com **Gerar automaticamente** ligado em Configurações → Cobranças & Acordos, os lançamentos da cota nascem sozinhos no dia configurado, sem você fazer nada.

Precisa gerar o mês corrente na hora — por exemplo, porque acabou de ativar a geração automática e o dia já passou? Na mesma aba, clique em **Gerar agora**, escolha **Mês atual**, **Próximo mês** ou um mês específico, e confirme.

{: .tip }
> **Use este caminho para a cota do mês — não o Lançamento em lote**
>
> O Financeiro também tem um [**Lançamento em lote por unidade**](/modulos/financeiro/#lançamento-em-lote-por-unidade-síndico), mais flexível: qualquer categoria, qualquer vencimento, valores editáveis na hora. Ele serve bem para uma **taxa extra** ou uma cobrança pontual — mas só o caminho de **Cobranças & Acordos** está ligado à emissão automática das cobranças pelo Asaas, descrita no próximo passo. Gerando a cota do mês pelo Lançamento em lote, você ainda vai precisar emitir cada cobrança à mão, uma por uma, na Cobrança automática.

### 2. Se o condomínio tem Cobrança Automática aprovada, o boleto e o Pix saem sozinhos

Condomínio com a [conta de cobrança aprovada](/fluxos/abrir-conta-de-cobranca/) não precisa de mais nenhum passo: no mesmo instante em que os lançamentos da cota são gerados — pelo cron do dia configurado ou pelo **Gerar agora** —, as cobranças correspondentes são emitidas no Asaas, e cada morador recebe o e-mail com boleto, Pix e o link para pagar. Veja o detalhe completo em [Cobrança Automática — Emissão automática no ciclo mensal](/modulos/cobranca-automatica/#emissão-automática-no-ciclo-mensal-síndico).

### 3. Sem Cobrança Automática, a cota fica no Financeiro para você dar baixa

Condomínio sem a conta aprovada continua exatamente como sempre operou: a cota nasce como lançamento em aberto no Financeiro, o morador paga por fora (transferência, depósito, dinheiro), e você [registra a baixa](/modulos/financeiro/#ver-os-detalhes-de-um-lançamento) — um lançamento por vez ou em lote, pela [ação **Dar baixa**](/modulos/financeiro/#ações-em-lote-síndico) — quando o pagamento chegar. O morador ainda recebe um aviso por e-mail com o valor e o vencimento da cota, só que sem link de pagamento pronto.

### 4. Confira que saiu certo

- No **Financeiro**, filtre por **Competência** = o mês gerado: o número de lançamentos deve bater com o número de unidades ativas.
- Com Cobrança Automática, abra **Cobrança automática → Cobranças** e confira o contador **Emitida**: deve ser igual ao número de lançamentos gerados, menos as falhas — cada falha vem com o motivo no detalhe da cobrança.
- Se algum morador reclamar que não recebeu nada, confira primeiro se a unidade dele tem CPF do responsável cadastrado — é a causa mais comum de uma cobrança individual falhar sem derrubar as demais.

![Cobrança automática — aba Cobranças com os contadores Emitida, Paga, Vencida, Aguardando confirmação, Cancelada e Falha na emissão, e a lista de cobranças por unidade logo abaixo](/assets/screenshots/fluxo-cobrar-cota-01-contadores-emitidas.png)

## Exemplo concreto

O Residencial Vale do Cedro tem 8 unidades e vencimento configurado para todo dia 10. No dia 10, o app gera 8 lançamentos de R$ 420,00 — um por unidade — na categoria **Taxas de condomínio**, com competência do mês corrente. Como a conta de cobrança está aprovada, as 8 cobranças são emitidas no mesmo instante: cada morador recebe "Sua cota de outubro está disponível", com boleto e Pix. O síndico não precisa abrir o aplicativo nesse dia.

## Dicas e armadilhas

- **Configure a taxa mensal antes do primeiro ciclo, não depois.** Corrigir uma unidade esquecida depois que ela já foi pulada significa lançar a cota daquele mês à mão, fora do ciclo.
- **"Gerar agora" nunca duplica.** Rodar de novo no mesmo mês, por engano ou para conferir, não cria lançamento repetido — o app reconhece que a categoria já tem cobrança daquele mês e não faz nada.
- **Ligue "Notificar condôminos"** (na mesma aba de Cobranças & Acordos, junto com "Gerar automaticamente") se quiser que o morador seja avisado assim que a cota é lançada. O aviso sai dos dois jeitos: pelo ciclo automático e pelo "Gerar agora" — quem decide é essa chave, não a forma como a cota foi gerada.

## Quando dá errado

| O que você vê | O que fazer |
|---|---|
| Botão **Gerar agora** desabilitado | Falta escolher a **Categoria de cobrança** em Configurações → Cobranças & Acordos — sem ela, não há em que lançamento basear a cota |
| "0 lançamentos gerados", mesmo com o botão liberado | As cobranças daquele mês já existem — confira no Financeiro pela competência antes de supor que algo falhou |
| Uma unidade específica não recebeu a cobrança do Asaas | Confira o CPF do responsável em Configurações → Condôminos → Unidades; é a causa mais comum de falha isolada |
| Dashboard mostra "Cobrança automática — em análise no Asaas" | A conta de cobrança ainda não foi aprovada; as cotas continuam sendo lançadas normalmente, só sem boleto/Pix — ver [Abrir a conta de cobrança](/fluxos/abrir-conta-de-cobranca/) |
