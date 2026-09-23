---
title: Contratar uma obra ou compra
parent: Fluxos
nav_order: 8
---

# Contratar uma obra ou compra

## Por que isto importa

Uma obra ou compra maior — pintura da fachada, troca de bomba, reforma do playground — costuma gerar a pergunta mais desconfortável que um síndico recebe: "por que esse fornecedor e não outro, e por que esse valor?". Registrar o processo inteiro no V3RCondo — os orçamentos recebidos, qual foi aprovado e por quê, cada despesa paga — transforma essa pergunta em uma resposta de dois cliques, em vez de uma reconstituição de memória ou de e-mails espalhados.

## Passo a passo

### 1. Registre a necessidade

Em **Compras e Serviços → + Nova Compra**, preencha título, descrição, categoria e, se já tiver uma referência, o valor estimado. O status nasce como **Planejada**.

### 2. Colete orçamentos

Na página de detalhe da compra, clique em **+ Adicionar Orçamento** para cada proposta recebida: fornecedor (busque um já cadastrado, ou cadastre na hora), valor, prazo de execução, data e observações. Anexo do orçamento em PDF é recurso do plano Pro.

{: .tip }
> **Cadastrar o fornecedor aqui já alimenta o módulo Fornecedores**
>
> Ao salvar um orçamento com os dados de um fornecedor novo, o sistema cadastra automaticamente em [Fornecedores](/modulos/fornecedores/), evitando duplicata por e-mail ou CPF/CNPJ — você não precisa cadastrar duas vezes.

### 3. Aprove um orçamento

Com os orçamentos na mesa, clique em **Aprovar** no que for escolhido — os demais são rejeitados automaticamente. O fornecedor e o valor aprovados ficam em destaque no cabeçalho da compra, e o **valor estimado** passa a refletir esse valor.

### 4. Acompanhe a execução

Conforme a obra avança, mude o status para **Em Andamento** e use as duas seções de acompanhamento:

- **Documentos e Anexos** — fotos do ambiente antes, notas de material, fotos da obra em andamento, contratos. Upload de novos arquivos é recurso do plano Pro; a visualização vale para todos os planos.
- **Anotações do síndico** — registre decisões e ocorrências: troca de fornecedor, imprevisto, prazo renegociado. Essas anotações alimentam diretamente o relatório de execução do passo 6 — quanto mais contexto aqui, mais completo o relatório.

### 5. Registre cada despesa paga

Na seção **Despesas**, clique em **+ Adicionar despesa** para cada pagamento: descrição, categoria financeira, valor, vencimento, conta bancária e, se já foi pago, marque **Marcar como pago**. Cada despesa registrada aqui **cria automaticamente o lançamento correspondente no Financeiro** — não é preciso lançar duas vezes. O total acumulado aparece no cabeçalho da compra, com o comparativo **Total gasto vs. Orçado** assim que o valor final estiver preenchido.

### 6. Conclua e gere o relatório de execução

Marque a compra como **Concluída** e clique em **Gerar relatório da obra**. Preencha observações e orientações para a IA (imprevistos, mudanças de escopo) e marque se quer enviar também para condôminos e para o Conselho Fiscal — o relatório sempre vai por e-mail para os síndicos, independentemente dessas marcações.

O relatório traz resumo executivo, o processo de cotação com o comparativo entre orçamentos aprovados e rejeitados, a execução financeira por categoria e as considerações finais, construídas a partir das suas anotações durante a obra.

### 7. Revise e publique

Enquanto o relatório está pronto para revisão, o botão mostra **Visualizar rascunho** — abra o PDF, confira, e só então clique em **Publicar**, que distribui aos destinatários marcados no passo 6.

![Detalhe de uma compra concluída, com o comparativo Estimado e Final no cabeçalho e os orçamentos recebidos abaixo](/assets/screenshots/fluxo-obra-01-total-gasto-vs-orcado.png)

## Exemplo concreto

O síndico do Edifício Aurora registra "Pintura da fachada" como nova compra, recebe três orçamentos, aprova o de R$ 18.400,00 com prazo de 20 dias, e acompanha a execução anotando "atraso de 3 dias por chuva" e "troca de tinta por indisponibilidade do fornecedor" ao longo do mês. Registra duas despesas — sinal e saldo — cada uma virando lançamento automático no Financeiro. Ao concluir, gera o relatório marcando envio para condôminos, revisa o rascunho e publica: os moradores recebem o PDF com o comparativo de orçamentos e o relato da obra, sem o síndico escrever nada a mais.

## Dicas e armadilhas

- **Anote durante a obra, não no fim.** O relatório de execução é só tão bom quanto as anotações registradas ao longo do caminho — reconstituir tudo na hora de concluir é o trabalho que esta seção existe para evitar.
- **O valor estimado trava depois de um orçamento aprovado.** Se o custo mudar por imprevisto, use o **valor final**, que continua editável a qualquer momento — não tente forçar o estimado para refletir a realidade.
- **Excluir um anexo ou orçamento pede confirmação — leia antes de confirmar.** O arquivo sai da lista da compra, mas fica guardado; dá para recuperar com a nossa ajuda, se tiver sido engano.

## Quando dá errado

| O que você vê | O que fazer |
|---|---|
| Botão de upload em Documentos e Anexos aparece bloqueado | Recurso do plano Pro — a visualização continua disponível no Básico |
| Excluiu uma despesa por engano | O lançamento correspondente no Financeiro também é removido junto — se precisar recuperar, é o mesmo caminho de recuperação de um lançamento excluído |
| Relatório saiu genérico, sem detalhe da obra | Regenere preenchendo (ou reforçando) o campo de observações, e confira se as anotações do síndico foram registradas durante a execução — é delas que a IA parte |
| Precisa corrigir algo depois de publicar o relatório | Não há edição do PDF publicado; ajuste as observações ou anotações e gere uma nova versão para republicar |
