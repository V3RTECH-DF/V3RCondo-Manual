---
title: Minha Área
parent: Módulos
nav_order: 2
---

# Minha Área

A **Minha Área** é o espaço de autoatendimento para condôminos e síndicos. Os serviços da sua unidade ficam organizados em abas: **Solicitar Documentos e Serviços** (emitir e solicitar documentos, extrato da unidade e negociação de dívida), **Meus Documentos** (baixar os documentos que você emitiu ou recebeu) e, nos condomínios que usam a Cobrança Automática, **Minhas cobranças** (pagar as cobranças da sua unidade).

> Porteiros não têm acesso a este módulo.

---

## Como acessar

Clique em **Minha Área** no menu lateral (desktop) ou no menu inferior (mobile). O acesso está disponível para condôminos e síndicos. Se você é síndico e também mora no condomínio, verá aqui os dados da sua própria unidade.

---

## Aba "Solicitar Documentos e Serviços"

Reúne tudo o que o condômino pode **emitir, solicitar ou acessar** sobre a própria unidade. No computador aparece como uma lista; no celular, como cartões.

![Aba "Solicitar Documentos e Serviços" no computador — lista com Nada Consta, Quitação Anual (IR) com seletor de ano, Declaração de Débitos, Declaração de Residência, Certidão de Quitação (venda), Solicitar documento (Outros) e Extrato da Unidade, cada item com sua ação à direita](/assets/screenshots/102-minha-area-solicitar-lista.png)

No celular, os mesmos itens aparecem como cartões empilhados:

![Aba "Solicitar Documentos e Serviços" no celular — os documentos e serviços em cartões](/assets/screenshots/103-minha-area-solicitar-cards.png)

### Emitir documento na hora

Alguns documentos são gerados automaticamente, na hora, a partir dos dados da sua unidade:

| Documento | Para que serve | Plano |
|---|---|---|
| **Nada Consta** | Comprova que a unidade está sem débitos | Básico |
| **Quitação Anual (IR)** | Demonstrativo anual de pagamentos para o Imposto de Renda (você escolhe o ano) | Básico |
| **Declaração de Débitos** | Relação dos débitos em aberto da unidade | Pro |
| **Declaração de Residência** | Comprova o vínculo da unidade com o condomínio | Pro |
| **Certidão de Quitação (venda)** | Atesta quitação para escritura/venda do imóvel | Pro |

Clique em **Emitir** e o PDF é baixado na hora. Na Quitação Anual (IR), o seletor mostra apenas os anos em que há lançamentos da sua unidade. Documentos do plano **Pro** aparecem com cadeado quando o condomínio está no Básico. Se a unidade tiver débitos vencidos, o Nada Consta e a Certidão de venda não são emitidos — o app oferece a Declaração de Débitos no lugar.

Todo documento emitido traz um **código de verificação** e um **QR Code**: qualquer pessoa (banco, cartório) confere a autenticidade na página pública **app.v3rcondo.com.br/verificar**, sem ver seus dados financeiros. Documentos emitidos antes de agosto de 2026 trazem o endereço antigo (`v3rcondo.com.br/verificar`), que continua funcionando.

<!-- TODO captura: página /verificar com um documento válido -->

### Solicitar documento ao síndico (Outros)

Precisa de um documento personalizado que o app não gera automaticamente? Clique em **Solicitar** no item "Outros", descreva o que precisa (e anexe uma referência, se quiser). O síndico recebe o pedido, produz o documento e anexa o PDF — que aparece para você na aba **Meus Documentos**. Você acompanha o status e pode cancelar enquanto o pedido estiver "aguardando o síndico".

### Extrato da Unidade

Consulte o histórico completo de cobranças da sua unidade — taxas de condomínio, taxas extras e outros lançamentos.

![Extrato da Unidade com filtro por ano, cards de resumo, tabela de lançamentos e botões de exportação](/assets/screenshots/97-minha-area-extrato.png)

*Os dados financeiros apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

O cabeçalho da página exibe o nome e o CPF do condômino designado como **responsável pela unidade** (quando configurado pelo síndico). Essa informação também aparece no PDF exportado, facilitando o uso como comprovante formal ou para a declaração de imposto de renda.

**O que você encontra:**

- **Filtro por ano** — selecione o exercício desejado ou visualize todos os lançamentos de uma vez
- **Resumo financeiro** com quatro totalizadores:
  - Total cobrado no período
  - Total pago (em verde)
  - Em aberto — lançamentos ainda dentro do prazo
  - Em atraso — lançamentos vencidos sem pagamento
- **Tabela detalhada** com competência, descrição, valor, vencimento, data de pagamento e status
- **Exportação em CSV** — baixe o extrato para usar em planilhas ou na declaração de imposto de renda. Disponível para todos os planos
- **Exportação em PDF** *(plano Pro)* — gera um documento formal com cabeçalho do condomínio, identificação do responsável pela unidade, tabela de resumo e listagem completa dos lançamentos. No plano Básico, o botão aparece com cadeado e mensagem explicativa

**Competência e vencimento são colunas diferentes**

A coluna **Competência** diz **a que mês aquela cobrança se refere**; a coluna
**Vencimento**, **quando ela tinha de ser paga**. As duas podem divergir — a taxa de
agosto pode vencer em setembro —, e é isso que a tabela mostra.

![Extrato da unidade com as colunas Competência, Descrição, Valor, Vencimento, Pagamento e Status](/assets/screenshots/condomino-extrato-competencia.png)

*Os dados financeiros apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

{: .note }
> **Corrigido**
>
> Por um período a coluna Competência repetia a data de vencimento, o que embaralhava
> a leitura de quem tinha cobranças com vencimento fora do mês de referência. Hoje ela
> mostra a competência de verdade.

**Status dos lançamentos:**

| Status | Significado |
|--------|-------------|
| Pago | Pagamento registrado pelo síndico |
| Pendente | Ainda dentro do prazo de vencimento |
| Em atraso | Prazo vencido sem registro de pagamento |

---

### Negociar dívida *(plano Pro)*

{: .note }
> **Disponível apenas no plano Pro**
>
> Esta seção aparece somente para condomínios no plano Pro e apenas quando há lançamentos de inadimplência vencidos vinculados à sua unidade.

Condôminos com débitos em atraso podem iniciar um acordo de parcelamento diretamente pelo app, sem precisar contatar o síndico. Basta acessar **Minha Área → Negociar dívida** quando a seção estiver disponível.

**Como funciona o fluxo:**

1. **Selecione os débitos** — a tabela lista os lançamentos vencidos elegíveis com checkbox para seleção individual. Marque os débitos que deseja incluir no acordo.
2. **Confira o cálculo automático** — com base nos parâmetros definidos pelo síndico, o sistema calcula a multa (%) sobre o total selecionado e os juros de mora mensais (%) proporcionais ao tempo de atraso de cada lançamento.
3. **Escolha o número de parcelas** — o seletor exibe as opções disponíveis. Opções que resultariam em parcelas abaixo do valor mínimo configurado pelo síndico aparecem desabilitadas.
4. **Revise o resumo financeiro:**

    | Campo | Descrição |
    |---|---|
    | Dívida selecionada | Soma dos lançamentos marcados |
    | Multa | Percentual aplicado sobre a dívida |
    | Juros estimados | Calculado por mês de atraso de cada lançamento |
    | Total acordado | Soma de dívida + multa + juros |
    | Valor por parcela | Total acordado dividido pelo número de parcelas |

5. **Confirme o acordo** — leia o aviso legal de reconhecimento da dívida e clique em **Confirmar Acordo**. O síndico recebe uma notificação por e-mail e Telegram com os detalhes do acordo.

{: .warning }
> **Antes de confirmar**
>
> Ao confirmar o acordo você reconhece formalmente a dívida e se compromete com o parcelamento. O acordo não pode ser desfeito pelo condômino após a confirmação — apenas o síndico pode cancelá-lo pelo módulo Financeiro.

---

### Meus acordos *(plano Pro)*

Exibe todos os acordos de parcelamento existentes para a sua unidade — tanto os iniciados pelo próprio condômino quanto os criados pelo síndico.

![Seção Meus acordos com accordion expandido mostrando tabela de parcelas e botão Baixar PDF](/assets/screenshots/98-minha-area-acordos.png)

*Os dados financeiros apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

Cada acordo aparece em um card com as informações principais: valor total, número de parcelas, status e data de criação. O botão **Baixar PDF** está disponível em cada card para salvar o comprovante do acordo.

{: .note }
> **Ações disponíveis apenas para o síndico**
>
> Os botões de cancelar acordo e marcar parcelas como pagas não aparecem nesta visão — essas ações são exclusivas do síndico, acessíveis pelo módulo Financeiro.

---

## Aba "Meus Documentos"

Lista todos os documentos da sua unidade para baixar — tanto os **automáticos** que você emitiu quanto os **manuais** que o síndico entregou. Cada item mostra o tipo, a data, o **código de verificação** e um botão para **baixar** (ou re-baixar) o PDF. Pedidos ainda em andamento aparecem com o status: *aguardando síndico*, *em análise*, *concluído* ou *recusado* (com o motivo).

{: .note }
> **Para o síndico, entra aqui também o termo da conta de cobrança**
>
> O **Termo de Autorização — Conta de Pagamento**, aceito na abertura da conta de cobrança, aparece nesta lista com o mesmo código de verificação e o mesmo botão de baixar dos demais documentos. Ele é do síndico que aceitou — nenhum condômino o vê, e ele não está entre os documentos que se podem solicitar. Ver [Cobrança Automática](/modulos/cobranca-automatica/).

<!-- TODO captura: aba "Meus Documentos" com o histórico de emissões/solicitações -->

---

## Aba "Minhas cobranças"

Reúne as cobranças da **sua unidade** e é por onde você paga. A aba aparece apenas nos condomínios que usam a [Cobrança Automática](/modulos/cobranca-automatica/) com a conta já aprovada — nos demais, ela não existe.

![Aba Minhas cobranças com o aviso do topo, uma cobrança em aberto marcada como Vencida com o botão Pagar e o histórico com cobranças pagas e canceladas](/assets/screenshots/condomino-minhas-cobrancas.png)

*Os dados financeiros apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

No alto da aba fica sempre o mesmo lembrete: **só aparecem aqui as cobranças já emitidas pelo síndico**. Ele está ali de propósito — ver a lista vazia não quer dizer que você não deve nada, quer dizer que o condomínio ainda não emitiu aquela cobrança.

{: .note }
> **Agora são as suas cobranças de verdade**
>
> Por um período esta aba mostrou **dados de demonstração** — valores e vencimentos de exemplo, iguais para todo mundo. Hoje ela lê as cobranças reais da sua unidade: o Pix, o boleto e a fatura são os do seu condomínio, e o pagamento vale.

A tela tem dois blocos:

- **Em aberto** — o que ainda há para pagar. Cada cobrança mostra o **valor**, o **vencimento**, a sua **unidade**, o selo de situação e o botão **Pagar**
- **Histórico** — as cobranças já encerradas (pagas, canceladas). Clique em qualquer uma para ver o detalhe

### Pagar

Clique em **Pagar** e escolha entre as formas disponíveis naquela cobrança:

| Forma | O que aparece |
|---|---|
| **Pix** | O **QR Code** e o código copia-e-cola, com botão de copiar |
| **Boleto** | A **linha digitável**, com botão de copiar, e **Abrir boleto** para o PDF |
| **Fatura** | O botão **Abrir fatura**, que reúne as formas de pagamento liberadas pelo condomínio |

No rodapé, o prazo de reconhecimento: **Pix e cartão costumam ser reconhecidos em minutos; boleto depende do banco processar e pode levar até o dia útil seguinte.** Enquanto isso, **não pague de novo**.

{: .note }
> **Reconhecido é quando a cobrança consta paga**
>
> É disso que o prazo acima fala: o momento em que a cobrança aparece como quitada para você e para o síndico. Assim que isso acontece, você recebe o e-mail de **pagamento confirmado** e a cobrança passa para o **Histórico**.

### Cobrança já paga

Abrindo uma cobrança do Histórico que já foi paga, no lugar das formas de pagamento aparece o aviso de que ela **já consta como paga** (com a data) e que não há nada a pagar, mais o botão **Ver comprovante na fatura**.

### Não vejo uma cobrança que eu esperava

Só aparecem aqui as cobranças **já emitidas pelo síndico**. Se você tem uma cota em aberto e não vê nada, o condomínio ainda não emitiu a cobrança daquele lançamento — o lançamento em si continua visível no **Extrato da Unidade**.

{: .warning }
> **Consulta que falha não vira “você não deve nada”**
>
> Se a consulta não responder, a tela diz **“Não deu para carregar suas cobranças”** e oferece **Tentar de novo**, deixando claro que isso não significa que não há o que pagar. Lista vazia e falha de carregamento são coisas diferentes, e a tela nunca troca uma pela outra.

---

## Perguntas frequentes

**Não vejo nenhuma cobrança no meu extrato. O que pode ser?**
Pode ser que o síndico ainda não tenha vinculado sua unidade aos lançamentos financeiros. Entre em contato com a administração pelo módulo **Fale com o Síndico**.

**Posso ver o extrato de outras unidades?**
Não. Cada condômino visualiza apenas os lançamentos da sua própria unidade.

**O extrato está incorreto. Como corrijo?**
O extrato reflete os lançamentos registrados pelo síndico. Em caso de divergência, entre em contato pela função **Fale com o Síndico**.
