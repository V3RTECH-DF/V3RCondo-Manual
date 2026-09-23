---
title: Prestar contas do mês
parent: Fluxos
nav_order: 2
---

# Prestar contas do mês

## Por que isto importa

Prestar contas é uma obrigação do síndico, e é também o que sustenta a confiança do condomínio na sua gestão. Feita mês a mês, ela é rápida e ninguém questiona um número: o histórico está todo lançado, conciliado e à mão. Deixada para o fim do ano ou para quando alguém pede, ela vira um trabalho de reconstituição — comprovante por comprovante — bem mais caro do que fechar um mês de cada vez.

Este fluxo parte do princípio de que o mês já foi bem cuidado no dia a dia: lançamentos registrados, baixas feitas, extrato conferido (ver [Conferir o extrato e conciliar](/fluxos/conferir-extrato-e-conciliar/)). Prestar contas é a etapa final, não o momento de arrumar a casa.

## Passo a passo

### 1. Feche o mês no Financeiro antes de gerar o documento

Antes de gerar a prestação, dê uma última passada pelo [Financeiro](/modulos/financeiro/): confira se todos os lançamentos do mês têm baixa e comprovante, e se o [saldo de cada conta bate com o extrato](/fluxos/conferir-extrato-e-conciliar/). A prestação de contas é fotografia do que está lançado — o que faltar lançar não aparece nela.

### 2. Gere a prestação de contas

Em **Relatórios → [Prestação de Contas](/modulos/relatorios/#prestação-de-contas)**, escolha o período — **Mês** é o uso mais comum aqui — e, se tiver algum documento complementar (uma ata, um ofício, uma planilha), anexe-o antes de gerar, com um rótulo identificando o que é.

Clique em **Gerar prestação**. O documento é montado em segundo plano — você recebe um e-mail quando estiver pronto, sem precisar ficar na tela esperando.

{: .note }
> **Escolhendo o ano corrente em vez do mês**
>
> Se preferir gerar a prestação do ano inteiro, saiba que o mês em curso **não entra** — a tela avisa que o documento vai só até o último mês fechado. O mês corrente entra na prestação seguinte, quando fechar.

### 3. Revise antes de publicar

O documento reúne o resultado do período (receitas, despesas e transferências), a movimentação por conta, a situação da inadimplência e os comprovantes anexados aos lançamentos — tudo num PDF só. Abra e confira os números batem com o que você já sabe do mês antes de publicar: depois de publicado, é isso que os condôminos vão ler.

{: .warning }
> **Sem a categoria da cota configurada, a inadimplência do período não aparece — nem como zero**
>
> Se [Configurações → Categorias → Financeiro](/modulos/configuracoes/#a-categoria-da-taxa-condominial) ainda não tem uma categoria marcada como a taxa condominial, a prestação registra a inadimplência como **"não apurada"**, em vez de mostrar que está tudo em dia. Um "zero" ali seria uma afirmação falsa — não há como o documento saber. Marque a categoria e gere o documento de novo.

### 4. Publique

Clique em **Publicar**. A partir daí, os condôminos passam a ver e baixar a prestação — na própria aba de Relatórios e em [Minha Área](/modulos/minha-area/). Mudou de ideia ou achou um erro depois de publicar? Você pode **despublicar** ou **excluir** a qualquer momento e gerar de novo.

### 5. Confira que os condôminos enxergam

Peça a alguém do Conselho Fiscal — ou entre você mesmo com outra conta — para confirmar que o documento aparece em Minha Área. É a prova de que a publicação chegou, e não só que o botão foi clicado.

<!-- PRINT: fluxo-prestar-contas-01-documento-publicado — ver roteiro de capturas -->

## Exemplo concreto

Fechado setembro no Financeiro — 42 lançamentos, todos com baixa e comprovante, extrato conciliado —, o síndico do Edifício Aurora gera a Prestação de Contas de **Mês: Setembro/2026**, anexa a ata da reunião do Conselho Fiscal que revisou os números, e publica. No dia seguinte, o Conselho Fiscal confirma que consegue baixar o PDF pela própria conta.

## Dicas e armadilhas

- **Gere cedo no mês seguinte, não no fim do trimestre.** Cada mês fechado sozinho é rápido de conferir; três meses empilhados multiplicam o trabalho de achar o que não bate.
- **Comprovantes valem mais anexados no lançamento do que soltos depois.** A prestação reúne automaticamente os comprovantes já vinculados aos lançamentos do período — quem anexa no dia a dia (ver [Registrar um lançamento](/modulos/financeiro/#registrar-um-lançamento-síndico)) não precisa caçar arquivo na hora de gerar o documento.
- **Publicar não é a única forma de mostrar transparência, mas é a mais barata.** Uma vez publicada, a prestação fica disponível sem você precisar enviar nada manualmente a cada condômino.

## Quando dá errado

| O que você vê | O que fazer |
|---|---|
| Inadimplência marcada como "não apurada" | Falta marcar a categoria da taxa condominial em Configurações → Categorias → Financeiro; gere o documento de novo depois de corrigir |
| Números do documento não batem com o que você esperava | Volte ao Financeiro e confira lançamentos sem baixa, ou o extrato ainda não conciliado daquele mês — a prestação reflete exatamente o que está lançado |
| Condômino diz que não consegue ver a prestação | Confira se ela foi de fato **publicada** (não basta ter sido gerada) — o status aparece na própria aba de Relatórios |
| Precisa corrigir algo depois de publicado | Despublique, corrija a causa no Financeiro, gere de novo e publique novamente — não há edição direta do PDF já publicado |
