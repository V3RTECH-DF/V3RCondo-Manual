---
title: Dashboard
parent: Módulos
nav_order: 1
---

# Dashboard

O Dashboard é a tela inicial do V3RCondo. Ao fazer login, você encontra aqui um resumo rápido da situação do seu condomínio.

![Dashboard do síndico com cards financeiros, gráfico de barras e tarefas urgentes](/assets/screenshots/10-dashboard-sindico.png)

## Aviso de contrato pendente *(síndico)*

Enquanto o condomínio não tiver o **Contrato de Prestação de Serviços** aceito, o síndico vê uma faixa no topo do Painel, acima de qualquer outro conteúdo.

![Faixa no topo do Painel avisando que o contrato de serviço ainda não foi aceito, com os botões Ler e aceitar e Ocultar por 30 dias](/assets/screenshots/painel-contrato-pendente.png)

A faixa deixa claro que **nada expira e nada é cobrado** por causa disso — só a abertura da conta de cobrança automática fica indisponível até o aceite. Dois botões:

- **Ler e aceitar** — abre a janela de aceite do contrato, a mesma do cartão **Contrato de Prestação de Serviços** em [Configurações → Condomínio](/modulos/configuracoes/), onde a pendência é resolvida de fato;
- **Ocultar por 30 dias** — apenas **adia** a faixa; não resolve a pendência, e ela volta a aparecer sozinha depois desse prazo.

Esse aviso é só para o síndico. O condômino não vê nada a respeito — o contrato é assunto entre o síndico e a V3RTECH, em nome do condomínio.

## Configuração inicial *(síndico — condomínio novo)*

Quem acabou de criar o condomínio encontra no topo do Dashboard o cartão **Configuração inicial**: a lista do que ainda falta para o condomínio operar, cada item com o atalho que leva direto ao lugar de resolver.

A ideia é simples: as pendências que só aparecem quando você tropeça nelas — a cota que não foi gerada porque a unidade estava sem valor, o lançamento em lote que abre com a lista de categorias vazia — passam a estar ditas de saída, em um lugar só.

<!-- PRINT: setup-01-cartao-configuracao-inicial — ver roteiro de capturas -->

### O que a lista cobra

| Item | Por que importa | Botão |
|---|---|---|
| **Dados do condomínio** | Endereço e fuso horário — é o fuso que define o que vence hoje e a hora dos avisos | Preencher |
| **Unidades** | Sem unidades cadastradas o condomínio não gera cobrança nem controla inadimplência | Cadastrar unidades |
| **Valor da cota das unidades** | A geração mensal pula toda unidade sem valor de cota — e não avisa depois | Definir cotas |
| **Categoria da taxa condominial** | Sem ela, o lançamento em lote abre com a lista de categorias vazia | Escolher categoria |
| **Condôminos** | Importe a planilha ou cadastre um a um | Cadastrar condôminos |
| **Conta bancária** | Opcional. Serve para conciliar o extrato com os lançamentos | Cadastrar conta |
| **Cobrança automática** | Boleto e Pix emitidos pelo Asaas, com baixa automática no Financeiro. Opcional | Conhecer e abrir conta |

Acima da lista, uma barra de progresso mostra **quantos passos de sete** já estão concluídos, com o botão **Continuar de onde parei** — ele leva ao primeiro passo que ainda não foi resolvido nem pulado.

São os sete itens da tabela acima, na mesma ordem — **o Valor da cota das unidades entra na contagem**, logo depois de Unidades, que é de onde ele depende. Ele é o único passo **sem o botão Pular**: sair da lista, ele sai sozinho, quando **todas** as unidades tiverem valor definido. É deliberado — unidade sem valor de cota é pulada na geração mensal em silêncio, e esse é justamente o passo que não pode sumir do radar.

{: .note }
> **Nada aqui é marcado à mão**
>
> A conclusão de cada item é lida da situação real do condomínio. Cadastrou as unidades, o item sai da lista sozinho; apagou a última, ele volta. Não existe caixinha para marcar.

### Pular, tirar da lista e trazer de volta

São duas ações diferentes, e a diferença importa:

- **Pular** — o item **continua na lista**, agora com a marca **Pulado**. Use quando você vai resolver depois e não quer perder de vista. O **Valor da cota das unidades** não tem esse botão, pelo motivo dito acima.
- **Não vamos usar** (o **✕** ao lado do botão) — o item **sai da lista**. Use para o que o condomínio decidiu não adotar. Só alguns itens aceitam isso: **Condôminos**, **Conta bancária** e **Cobrança automática**. O que é estrutural — dados do condomínio, unidades, cota e categoria da taxa — não sai da lista, porque sem eles o condomínio não funciona.

O que foi tirado da lista não desaparece: no rodapé do cartão aparece o contador **“*n* item(ns) que você tirou da lista”**. Clique para abrir e use **Voltar para a lista** em qualquer um deles.

**O cartão some sozinho** quando não sobra nada — nem pendência, nem item tirado da lista. Não é preciso fechá-lo.

### A linha da Cobrança automática muda de texto conforme o andamento

É a única linha que depende de um terceiro, o Asaas, e o cartão deixa isso explícito em vez de cobrar de você algo que não está na sua mão:

| Situação | O que o cartão diz | Ação |
|---|---|---|
| Conta ainda não aberta | **Cobrança automática** | Conhecer e abrir conta |
| Cadastro enviado, em análise | **Cobrança automática — em análise no Asaas**, com a data do envio | Nenhuma. O botão aparece como **Aguardando**, desabilitado, com a etiqueta **Com o Asaas** |
| Cadastro recusado | **Cobrança automática — cadastro recusado**, com o motivo informado por eles | Corrigir e reenviar |
| Falta reconectar a chave de acesso | **Cobrança automática — falta reconectar a chave** | Reconectar |
| Conta aprovada | A linha desaparece | — |

Essa linha aparece para **qualquer condomínio** com conta de cobrança em andamento, mesmo os mais antigos — deixar a conta pela metade sem ninguém avisando seria exatamente o silêncio que o cartão existe para evitar.

{: .note }
> **Só para condomínios criados a partir de 13 de agosto de 2026**
>
> Os passos de configuração aparecem apenas em condomínios criados a partir dessa data. Quem já está rodando há meses não é cobrado por uma lista de coisas que já resolveu do seu jeito. A linha da **conta de cobrança**, essa sim, vale para todos.

{: .note }
> **Se a consulta falhar, o cartão diz que falhou**
>
> No lugar da lista aparece **“Não deu para conferir a configuração”**, com o botão **Tentar de novo**. Uma consulta que não respondeu nunca é apresentada como “está tudo certo”.

## Resumo financeiro

Três cards no topo exibem os dados do mês atual:

- **Saldo do Mês** — resultado do período (entradas menos saídas)
- **Total de Entradas** — soma de todas as receitas recebidas no mês
- **Total de Saídas** — soma de todas as despesas pagas no mês

## Fluxo de Caixa

O gráfico de barras mostra a evolução mensal das **entradas** (verde escuro) e **saídas** (vermelho) nos últimos 6 meses. Use-o para identificar tendências e comparar o desempenho financeiro ao longo do tempo.

## Tarefas Urgentes *(síndico — plano Pro)*

Exibe as tarefas com prazo vencido ou classificadas como prioridade **Alta**. Cada item mostra o título da tarefa, o prazo e o nível de urgência. O número em laranja ao lado de "Tarefas" no menu lateral indica quantas tarefas urgentes estão pendentes.

{: .note }
> **Condôminos**
>
> Esta seção **não aparece** para condôminos — o módulo de Tarefas é exclusivo para síndicos com plano Pro.

## Avisos Recentes

Exibe os posts mais recentes do Mural do condomínio, com categoria, título e data de publicação. Tanto síndicos quanto condôminos visualizam os mesmos avisos.

## Últimos Documentos

Lista os documentos mais recentemente disponibilizados no condomínio, com nome e data de upload. Clique em qualquer item para ir diretamente ao módulo de Documentos.

![Seções inferiores do Dashboard: avisos recentes e últimos documentos](/assets/screenshots/11-dashboard-sindico-inferior.png)

## Diferenças entre perfis

|  | Síndico | Condômino |
|---|---|---|
| Configuração inicial | ✅ Em condomínio novo, até resolver a lista | ❌ Não aparece |
| Resumo financeiro | ✅ | ✅ |
| Fluxo de caixa | ✅ | ✅ |
| Tarefas urgentes | ✅ Vê tarefas pendentes | ❌ Não aparece |
| Avisos recentes | ✅ | ✅ |
| Últimos documentos | ✅ | ✅ |
| Menu lateral | Todos os módulos | Sem Tarefas e Configurações |
