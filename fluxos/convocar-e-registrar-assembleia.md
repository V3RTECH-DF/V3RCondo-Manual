---
title: Convocar e registrar uma assembleia
parent: Fluxos
nav_order: 6
---

# Convocar e registrar uma assembleia

## Por que isto importa

Uma assembleia mal documentada — pauta incompleta, quórum sem registro, ata que ninguém lembra de publicar — é fonte de questionamento depois, às vezes anos depois, quando a decisão precisa ser defendida perante um condômino ou a Justiça. O V3RCondo cobre o ciclo inteiro, de propósito, para que o registro fique completo sem depender da memória de quem conduziu a reunião: convocação formal, lista de presença, deliberação item a item, e ata redigida com apoio de IA a partir do que foi de fato registrado durante a condução.

**Plano Pro.** Este fluxo inteiro é exclusivo do plano Pro.

## Passo a passo

### 1. Crie a assembleia e monte a pauta

Em **Assembleias → + Nova assembleia**, preencha título, tipo (Ordinária ou Extraordinária), data, hora e local — físico ou link de videoconferência, se for virtual. Salvar cria a assembleia como **Rascunho**, editável à vontade enquanto não for publicada.

Na seção **Pauta**, adicione cada item com título, descrição e tipo (Informativo, Votação, Discussão ou Assunto geral). É **agora**, ainda em rascunho, que todo item precisa entrar — a tela de condução, no dia da assembleia, só lista e edita os itens que já existem; não dá para criar item novo durante a reunião. Ver [Assembleias — Montar a pauta](/modulos/assembleias/#montar-a-pauta).

{: .note }
> **O total de unidades para o quórum é travado na criação do rascunho**
>
> É a contagem de unidades cadastradas no momento em que você clicou em **Salvar** que vale para o quórum desta assembleia — e ela não muda depois, mesmo que o condomínio cadastre ou remova unidades antes de publicar o edital. Cadastre as unidades certas **antes** de criar o rascunho.

### 2. Publique o edital

Com a pauta completa, clique em **Publicar edital**. O V3RCondo gera o PDF de convocação, envia por e-mail a todos os condôminos, dispara uma notificação interna, e o status muda para **Edital publicado**.

{: .warning }
> **Depois de publicar, os dados não podem mais ser editados**
>
> Confira a pauta com calma antes deste clique — é aqui, não na condução, que ela precisa estar fechada.

### 3. No dia, abra a assembleia e registre o quórum

Clique em **Iniciar assembleia** e preencha o painel de abertura: quem preside a mesa, quem é o secretário, e o **quórum** — quantas unidades estão presentes e se o quórum foi atingido, conforme a convenção do seu condomínio. Confirme em **Abrir assembleia**; o status muda para **Em andamento**.

A lista de presença já vem gerada com todos os membros ativos, marcados como presentes por padrão — ajuste quem realmente está lá, a modalidade (presencial ou remoto) e adicione convidados externos, se houver.

### 4. Conduza a pauta e registre as deliberações

Para cada item, avance o status (**Pendente → Em discussão → Concluído**) e escreva as anotações do secretário — são elas que vão alimentar a redação da ata. Item de votação concluído abre o formulário de deliberação: tipo (aclamação, contagem de votos ou sem votação), resultado e a decisão tomada em texto livre.

{: .tip }
> **Quanto mais detalhada a anotação, melhor a ata**
>
> A IA que redige a ata trabalha a partir do que o secretário escreveu durante a condução. Registrar só "aprovado" deixa a ata genérica; registrar o que foi discutido, quem se manifestou e por quê dá à IA o material para uma ata que de fato representa a reunião.

### 5. Encerre a assembleia

Clique em **Encerrar assembleia** — disponível também no rodapé, útil em pautas longas. É irreversível: depois de encerrada, a assembleia não pode ser reaberta, então confirme que todas as deliberações foram registradas antes deste clique.

### 6. Gere a ata

Ao encerrar, o app pergunta se você quer gerar a ata com IA — ou você acessa essa opção depois, a qualquer momento, na assembleia encerrada. Preencha, se quiser, as **observações para a geração** (uma ressalva de um condômino, ênfase num ponto específico) e clique em **Solicitar geração**. O processo roda em segundo plano; você recebe uma cópia por e-mail quando estiver pronta.

Com a ata pronta, você tem três caminhos: **Publicar ata**, **Regenerar com ajustes** (descreva o que precisa mudar) ou **Lançar ata própria** (fazer upload de um PDF elaborado fora do sistema).

### 7. Publique a ata

Clique em **Publicar ata**. Todos os condôminos recebem um e-mail com o link para download, a ata fica disponível em Documentos → Assembleias, e você recebe um e-mail com a ata mais uma seção de **itens de governança** sugeridos pela IA — tarefas, prazos e comunicados recomendados a partir do que foi decidido.

### 8. Avalie o registro em cartório

Depois de publicar, o app lembra: verifique se a ata precisa ser registrada em cartório. Se precisar, reúna o edital, as evidências de publicação, a lista de presença, a ata e o requerimento de registro.

## Exemplo concreto

O síndico do Residencial Vale do Cedro cria a AGO 2026 com três itens de pauta — prestação de contas, eleição do Conselho Fiscal e aprovação de taxa extra para pintura — e publica o edital 20 dias antes da data marcada. No dia, abre a assembleia com 32 das 40 unidades presentes (quórum atingido), conduz os três itens registrando votos e anotações, encerra, e gera a ata com IA. Revisa o PDF, publica, e o app já sugere, entre os itens de governança, criar uma tarefa para abrir a cotação da pintura aprovada.

## Dicas e armadilhas

- **Assunto que surgiu de última hora entra como "Assunto geral" — mas ainda em rascunho.** Se a pauta já foi publicada, não há como acrescentar item novo; ele fica para a próxima assembleia.
- **Só a ata mais recente fica na lista de documentos, enquanto não publicada.** Regenerar com ajustes substitui a versão anterior — a ata já publicada, essa sim, permanece como registro oficial.
- **A IA redige, você revisa.** O aviso do próprio app é claro: revise o documento antes de publicar oficialmente — a IA trabalha com o que foi registrado, mas a responsabilidade pela ata final é sua.

## Quando dá errado

| O que você vê | O que fazer |
|---|---|
| Botão **Publicar edital** recusa a ação | A pauta está vazia — cadastre ao menos um item antes de publicar |
| Precisou corrigir algo depois de publicar o edital | Não é possível editar; se o erro for grave, cancele a assembleia (só funciona em Rascunho ou Edital publicado, antes de iniciar) e crie uma nova |
| Tentou cancelar uma assembleia já iniciada | Não é permitido — o cancelamento só existe até o status **Em andamento** começar |
| Ata gerada não representa bem a reunião | Use **Regenerar com ajustes**, descrevendo especificamente o que precisa mudar — as observações da geração anterior já vêm preenchidas para você complementar |
| Esqueceu de publicar a ata | Ela continua disponível na assembleia encerrada, esperando por você — não há prazo para publicar depois de gerada |
