---
title: Configurações
parent: Módulos
nav_order: 14
---

# Configurações

{: .warning }
> **Acesso restrito**
>
> O módulo de Configurações é exclusivo para **síndicos**.

O módulo reúne todas as opções de gestão do condomínio, organizadas em
seis abas.

{: .note }
> **Procurando as preferências de notificação?**
>
> Elas saíram das Configurações e agora ficam em
> [**Meu Perfil**](/modulos/perfil/), no cartão **Como sou avisado** — assim
> todo usuário, síndico ou condômino, alcança as suas.

![Aba Condomínio com dados cadastrais e card do plano atual](/assets/screenshots/73-config-condominio.png)

## Aba Condomínio

Exibe e permite editar os dados cadastrais:

- **Nome do Condomínio** — obrigatório
- **Endereço Completo** — logradouro e número
- **Cidade e Estado**
- **CNPJ** — cadastro nacional do condomínio
- **Quantidade de unidades** — exibido em **modo leitura**: reflete a contagem de unidades cadastradas na aba **Unidades** e é o que define o preço do plano Pro. Use o atalho **Gerenciar unidades** para ajustar
- **Logo do Condomínio** — PNG ou JPG até 2 MB. A logo aparece na sidebar
  ao lado do nome e também no cabeçalho da ata gerada pelo sistema. Sem logo
  cadastrada, a ata sai com a marca do V3RCondo

- **Fuso horário** — selecione o fuso horário do condomínio entre os 14 fusos brasileiros disponíveis (padrão: Brasília, UTC−3). A configuração afeta como datas e horários são exibidos em todo o aplicativo — Dashboard, Financeiro, Tarefas, Assembleias, Compras e Fale com o Síndico — e também nos **documentos gerados** (edital de convocação, ata), nos **e-mails** e nas **notificações**. O horário impresso em um documento é o mesmo que aparece na tela

Clique em **Salvar alterações** para confirmar.

### Contrato de Prestação de Serviços

Logo abaixo dos dados cadastrais, um cartão mostra a situação do **Contrato de Prestação de Serviços** — o instrumento entre o condomínio e a V3RTECH, aceito pelo **síndico em nome do condomínio**.

{: .note }
> **Não confunda com os Termos de Uso**
>
> São dois aceites diferentes. Os **Termos de Uso** e a **Política de Privacidade** são aceitos por **cada pessoa** que usa o aplicativo — síndico, condômino ou porteiro —, no primeiro acesso e sempre que a versão muda. Já o **Contrato de Prestação de Serviços** é aceito **uma única vez**, pelo síndico, em nome do condomínio. O condômino nunca vê esse aceite nem precisa fazer nada a respeito. Veja [Primeiros Passos](/guia/primeiros-passos/) para o aceite individual.

**Quando o contrato já foi aceito**, o cartão mostra o selo **Aceito**, a versão do contrato, a data e a hora do aceite e o nome de quem aceitou, além do botão **Baixar o contrato em PDF** — disponível a qualquer momento.

![Cartão do Contrato de Prestação de Serviços com status Aceito, versão, data e botão de baixar em PDF](/assets/screenshots/config-contrato-aceito.png)

**Enquanto o contrato ainda não foi aceito**, o cartão explica o que está pendente e mostra o botão **Ler e aceitar o contrato**:

![Cartão do Contrato de Prestação de Serviços pendente, com aviso e botão Ler e aceitar](/assets/screenshots/config-contrato-pendente.png)

{: .warning }
> **O que fica bloqueado até o aceite — e o que não fica**
>
> Sem o contrato aceito, a única coisa indisponível é **abrir a conta de cobrança automática** no módulo [Cobrança automática](/modulos/cobranca-automatica/). Todo o resto continua funcionando normalmente: os condôminos seguem usando o aplicativo sem qualquer restrição, e um condomínio que já tenha a conta de cobrança aberta continua operando. O motivo do bloqueio: é esse contrato que autoriza a V3RTECH a tratar os dados do condomínio e a operar a cobrança automática em nome dele — sem ele, essa autorização não existe.

Clicando em **Ler e aceitar o contrato**, abre uma janela com o resumo do que está sendo aceito e um link para ler o contrato na íntegra. Marque a declaração de que você é o síndico e aceita o contrato em nome do condomínio, e confirme.

![Janela de aceite do Contrato de Prestação de Serviços, com o resumo, o link para o texto completo e a declaração a marcar](/assets/screenshots/config-contrato-dialogo-aceite.png)

Ao confirmar, ficam registrados a **data e a hora**, a **versão do contrato**, **quem aceitou** e o **endereço de rede apurado pelo nosso servidor**. O sistema gera um **PDF verificável**, com código e QR Code, conferível a qualquer momento na página pública de verificação — e envia uma cópia por **e-mail ao síndico**. O documento fica disponível para download neste mesmo cartão, a qualquer momento.

{: .tip }
> **Se algo falhar no meio do caminho**
>
> A tela avisa na hora, e **nada fica registrado pela metade** — não existe um aceite "meio feito". Basta tentar de novo, ali mesmo ou depois, pela pendência.

Enquanto o contrato estiver pendente, o síndico também vê um aviso no topo do [Painel](/modulos/dashboard/), com o atalho **Ocultar por 30 dias** — que apenas adia o lembrete, sem resolver a pendência: ele volta a aparecer depois desse prazo.

### Plano e assinatura

Na coluna direita da aba Condomínio, o card **Seu Plano** exibe o plano atual,
o status do pagamento e a data da próxima cobrança. A partir daqui você
pode assinar o plano Pro ou gerenciar a assinatura existente.

O preço do Pro é calculado pela **quantidade de unidades cadastradas** (aba
Unidades): ao assinar, o sistema já mostra a **faixa e o valor** correspondentes
ao seu condomínio, sem você escolher o tamanho. **Cadastre as unidades antes de
assinar** — sem unidades cadastradas, a assinatura fica bloqueada e o botão vira
**Cadastrar unidades**. Condomínios com mais de 200 unidades são atendidos sob
consulta (**Fale conosco**).

### Parceiros do Condomínio

Abaixo do card de plano, a seção **Parceiros do Condomínio** centraliza os
contatos institucionais fixos do condomínio — profissionais e empresas com
relacionamento contínuo, como contador, advogado e administradora.

Tipos de parceiro disponíveis:

- **Contador / Escritório Contábil**
- **Advogado / Escritório Jurídico**
- **Administradora**
- **Segurança**
- **Empresa de Elevadores**
- **Bombeiros / AVCB**
- **Limpeza e Conservação**
- **Zeladoria**
- **Outro** — com rótulo personalizado

Para cada parceiro é possível registrar: empresa, nome do contato, CNPJ,
telefone, e-mail e observações.

![Seção Parceiros do Condomínio com cards de contatos institucionais](/assets/screenshots/74-config-parceiros.png)

Clique em **+ Adicionar parceiro** para
cadastrar um novo contato, ou no ícone de lápis (✎) ao lado de um parceiro
existente para editar ou excluir. Ao excluir, o parceiro sai da lista do
condomínio, mas o cadastro **fica guardado** — dá para recuperar com a nossa
ajuda se tiver sido engano.

![Modal de cadastro de parceiro do condomínio](/assets/screenshots/75-config-parceiro-modal.png)

{: .tip }
> **Diferença entre Parceiros e Fornecedores**
>
> **Parceiros** são contatos institucionais permanentes (contador, advogado,
> administradora). **Fornecedores** são empresas contratadas para serviços
> pontuais (elétrica, pintura, jardinagem). Use módulos separados para manter
> a organização.

## Aba Condôminos

Lista os membros do condomínio com: nome, e-mail, unidade, papel e título.
Use o filtro para visualizar apenas síndicos ou apenas condôminos, e o filtro de
situação (**Todos**, **Ativos**, **Inativos**) para escolher quem aparece na lista.
Cada membro exibe um badge de situação — **Ativo** (verde) ou **Inativo** (cinza).
O condômino designado como **responsável** pela unidade aparece com um badge laranja "Responsável" — ele é o destinatário das notificações extrajudiciais.

![Aba Condôminos com lista de membros ativos, badges de responsável, ícone de editar perfil e botão Transferir](/assets/screenshots/config-condominos-editar.png)

*Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

**Adicionar um condômino diretamente:** clique em **+ Adicionar condômino**,
preencha o nome completo, e-mail, unidade (opcional) e título (opcional:
Síndico, Subsíndico, Contador, Conselho Fiscal) e clique em **Adicionar**. O sistema
cadastra o membro imediatamente e envia um e-mail de boas-vindas com
instruções para definir a senha ou entrar com o Google.

![Modal de adição direta de condômino com campos de nome, e-mail, unidade e título](/assets/screenshots/77-config-condomino-modal.png)

*Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

**Editar dados de um membro:** clique no ícone de lápis (✎) ao lado do membro para abrir o drawer **Editar Membro**. O síndico pode editar:

![Drawer Editar Membro com campos de Nome, Unidade, Título e dados pessoais incluindo CPF ou CNPJ, RG, Telefone, Profissão, Instagram, LinkedIn e aniversário — o campo CPF ou CNPJ preenchido com um CNPJ alfanumérico fictício mostra a máscara aplicada](/assets/screenshots/config-editar-membro-cpf-cnpj-01.png)

- **Nome** — nome completo do membro
- **Unidade** — unidade à qual o membro pertence
- **Título** — Síndico, Subsíndico, Contador, Conselho Fiscal ou Condômino
- **CPF ou CNPJ** — use CPF quando a unidade estiver em nome de uma pessoa, e
  CNPJ quando estiver em nome de uma empresa. A máscara acompanha o que você
  digita e aceita o **CNPJ alfanumérico** (formato novo da Receita, com letras).
  É o documento que aparece na cobrança e nos documentos gerados para essa
  unidade
- **RG**
- **Telefone**
- **Profissão**
- **Instagram** e **LinkedIn** — links de perfil
- **Dia e Mês de aniversário**

Clique em **Salvar** para confirmar. Ao promover um membro para Síndico, o sistema exibe um aviso de que o condomínio passará a ter mais de um síndico — o papel do síndico atual não é alterado automaticamente. Ao alterar o próprio papel para um título sem permissão de síndico, o sistema exibe um aviso de confirmação, pois o acesso de síndico será removido imediatamente após salvar.

**Transferir responsabilidade:** quando um condômino responsável por uma unidade tem pelo menos outro membro na mesma unidade, o botão **Transferir** aparece ao lado do badge "Responsável". Clique nele para selecionar o novo responsável e confirmar a transferência — o sistema garante que sempre haverá exatamente um responsável por unidade.

![Modal de transferência de responsabilidade com seletor de novo responsável](/assets/screenshots/95-configuracoes-transferir-responsavel.png)

*Os dados pessoais apresentados nesta imagem são fictícios e foram utilizados apenas para fins ilustrativos.*

### Desativar, reativar e excluir um condômino

São duas ações diferentes, para situações diferentes.

**Desativar é uma pausa.** O condômino continua na lista, marcado como **Inativo**,
e perde o acesso ao aplicativo naquele condomínio. Use quando a pessoa pode voltar —
um morador que viajou, uma unidade temporariamente desocupada, um cadastro que
você quer congelar sem perder de vista. Clique no ícone de **desativar** na linha
do membro e confirme.

{: .note }
> **Desativar corta o acesso de verdade**
>
> A desativação sempre tirou a pessoa do aplicativo, mas alguns conteúdos do
> condomínio — **arquivos** e **categorias** — continuavam alcançáveis por quem
> já estava desativado. Não é mais o caso: quem está **Inativo** perde o acesso
> a tudo do condomínio, inclusive esses. Se você desativou alguém contando com
> isso, agora vale o que a tela diz.

**Reativar devolve o acesso.** Um membro inativo mostra o ícone verde de
**reativar** — clique nele e a pessoa volta a ser Ativa, com acesso restaurado.
Se a lista estiver filtrada por **Ativos**, troque o filtro para **Inativos** ou
**Todos** para encontrá-lo.

**Excluir é a saída definitiva.** O condômino sai da lista e perde o acesso, mas
**continua em tudo que já foi registrado**: presença em assembleias, atas,
cobranças, acordos e solicitações. O histórico do condomínio não é reescrito.
A opção de excluir aparece para membros **inativos** — desative primeiro, depois
exclua. Clique no ícone de lixeira e confirme.

{: .tip }
> **Se a pessoa voltar a morar no condomínio**
>
> Basta cadastrá-la de novo, pelo **+ Adicionar condômino** ou pela importação
> em planilha, usando o mesmo e-mail. O vínculo anterior é reaproveitado: não
> há cadastro duplicado e o histórico continua no lugar.

{: .note }
> A exclusão funciona para qualquer condômino, inclusive quem já participou de
> assembleias, tem cobranças lançadas ou acordos registrados.

**Importar planilha de condôminos:** clique em **Importar planilha** para
cadastrar vários condôminos de uma vez. Baixe o modelo, preencha com Nome,
E-mail, Unidade e Título e faça o upload. O sistema processa linha a linha,
ignora e-mails já cadastrados e exibe um resumo com importados, ignorados e
rejeitados (com o motivo). Limite de 100 condôminos por importação — se
houver mais, realize importações em lote.

![Tela de importação de planilha de condôminos](/assets/screenshots/78-config-importar-planilha.png)

**Solicitações pendentes:** solicitações de vínculo enviadas pelos próprios
moradores aparecem acima da lista. O síndico pode **Aprovar** ou **Rejeitar**
cada solicitação.

## Aba Unidades *(síndico)*

Lista todas as unidades ativas do condomínio (registro canônico de unidades do condomínio — é também a contagem usada para calcular o preço do plano Pro) e permite configurar a **taxa mensal** de cada uma, individualmente ou em lote.

![Aba Unidades com lista de unidades, filtro rápido e tabela de taxas mensais](/assets/screenshots/98-config-unidades.png)

| Coluna | Descrição |
|---|---|
| **Unidade** | Identificação da unidade (ex.: 101, Bloco A Apto 3) |
| **Taxa Mensal (R$)** | Valor configurado ou "—" se ainda não definido |
| **Ações** | Ícone de lápis para definir ou alterar o valor individualmente |

### Edição individual

Clique no **lápis** ao lado de uma unidade (a dica mostra **Editar taxa**), informe o valor em reais e clique em **Salvar**. Para remover a taxa configurada, deixe o campo em branco e salve. A confirmação aparece dizendo qual unidade foi atualizada.

{: .note }
> **Voltou a funcionar**
>
> Por um período a edição individual não estava operando, e corrigir a taxa de **uma** unidade só dependia de recorrer à aplicação em lote. O lápis está normalizado.

### Filtro rápido

Acima da tabela, os botões **Todas / Sem taxa / Com taxa** filtram as unidades exibidas. Trocar o filtro limpa a seleção atual.

### Aplicação em lote

Para configurar a taxa de várias unidades de uma vez:

1. **Selecione as unidades** marcando os checkboxes à esquerda de cada linha. O checkbox no cabeçalho da tabela seleciona ou deseleciona todas as unidades visíveis. Quando apenas algumas estão marcadas, o checkbox do cabeçalho exibe um estado intermediário (traço).
2. Ao selecionar ao menos uma unidade, a **barra de ação em lote** aparece acima da tabela, indicando quantas unidades estão selecionadas e oferecendo um botão **Desmarcar** para limpar a seleção.
3. Escolha o modo de aplicação:

    - **Taxa fixa (R$):** define o mesmo valor para todas as unidades selecionadas. Se o valor informado for zero, um aviso em destaque informa que a taxa será *removida* dessas unidades.

    ![Barra de ação em lote com modo Taxa fixa e 3 unidades selecionadas](/assets/screenshots/99-config-unidades-selecao-taxa-fixa.png)

    - **Reajuste (%):** aplica um percentual sobre a taxa atual de cada unidade selecionada. Use valores positivos para aumento e negativos para desconto (ex.: `-5` para 5% de desconto). Unidades sem taxa configurada são automaticamente ignoradas e listadas no diálogo de confirmação.

    ![Barra de ação em lote com modo Reajuste % e campo de percentual](/assets/screenshots/100-config-unidades-selecao-reajuste.png)

4. Clique em **Aplicar**. Um diálogo de confirmação exibe uma prévia das alterações — incluindo exemplos de cálculo no modo reajuste e a lista de unidades que serão ignoradas — antes de gravar.

### Criar várias unidades de uma vez

O botão **Gerar unidades em lote** cria as unidades a partir de um padrão, em vez de uma a uma. Escolha entre **Faixa numérica** (101 a 104) e **Bloco × Faixa** (A-101, A-102, B-101…), informe prefixo, sufixo e quantos dígitos usar, e confira a **prévia** — ela mostra quantas serão criadas e quantas já existem. Unidades já cadastradas são ignoradas.

O formulário também pede a **Taxa mensal das unidades criadas (R$) — opcional**: o valor informado é aplicado a **todas** as unidades criadas naquele momento. Deixando em branco, você define a taxa depois, unidade a unidade.

{: .tip }
> **Preencha a taxa já na criação**
>
> É o caminho mais curto para deixar o condomínio pronto para cobrar: a geração mensal **pula toda unidade sem valor de cota**, e não avisa depois. Unidades com valores diferentes entre si continuam sendo resolvidas pela edição individual ou pela aplicação em lote.

O diálogo **Cadastrar unidade**, para criar uma unidade avulsa, também aceita a **Taxa mensal (R$) — opcional** no mesmo momento do cadastro.

{: .note }
> **Para que serve esse campo?**
>
> A taxa mensal por unidade é usada como valor padrão ao gerar cobranças em lote no módulo Financeiro e na geração mensal automática. Configure antes de usar o lançamento em lote para não precisar preencher o valor manualmente para cada unidade.

## Aba Cobranças & Acordos *(síndico)*

Configura a geração automática de cobranças mensais do condomínio.

| Campo | Descrição |
|---|---|
| **Categoria de cobrança** | Categoria financeira que será usada nos lançamentos gerados (ex.: "Taxa de Contribuição") |
| **Conta bancária padrão** *(opcional)* | Conta bancária vinculada às cobranças geradas. Se definida, toda cobrança mensal — automática ou pelo Lançamento em Lote — já nasce ligada a essa conta, sem precisar editar uma a uma. Deixe em branco para não vincular nenhuma conta (comportamento anterior). As contas disponíveis vêm da aba **Contas Bancárias** |
| **Dia de vencimento** | Dia do mês em que as cobranças vencem (1 a 31). Em meses com menos dias, o sistema ajusta automaticamente para o último dia do mês |
| **Antecedência do aviso** | Quantos dias antes do vencimento o síndico recebe um lembrete para revisar as cobranças |
| **Gerar automaticamente** | Quando ativado, o sistema gera os lançamentos por unidade no dia calculado, sem necessidade de ação manual |
| **Notificar condôminos** | Quando ativado (junto com "Gerar automaticamente"), os condôminos recebem uma notificação ao ter a cobrança lançada |

![Aba Cobranças & Acordos: categoria e conta bancária padrão, dia de vencimento, geração automática e parâmetros de acordo](/assets/screenshots/101-config-cobranças.png)

Clique em **Salvar configurações** para confirmar.

{: .note }
> **Geração manual**
>
> Mesmo com a geração automática desativada, o botão **Gerar agora** permite disparar a criação das cobranças manualmente. Ao clicar, um diálogo apresenta três opções de mês antes de confirmar: **Mês atual** (padrão), **Próximo mês** e **Escolher mês** (seletor livre). O mês selecionado define a competência e o vencimento dos lançamentos gerados.

{: .tip }
> **Sem duplicatas**
>
> O sistema verifica se as cobranças do mês atual já foram geradas antes de agir. Se já existirem lançamentos daquela categoria para o mês, a ação é ignorada silenciosamente — sem duplicatas.

{: .warning }
> **Configure as unidades antes**
>
> Para que o valor de cada cobrança seja preenchido automaticamente, configure a taxa mensal por unidade em **Configurações → Unidades** antes de ativar a geração automática.

### Parâmetros de Acordo Self-Service *(plano Pro)*

Define as condições do acordo quando o próprio condômino inicia o parcelamento por Minha Área.

| Campo | Padrão | Descrição |
|---|---|---|
| **Multa sobre o débito (%)** | 2,00% | Percentual aplicado sobre o total dos débitos selecionados |
| **Juros de mora mensais (%)** | 1,00% | Percentual ao mês aplicado por mês de atraso em cada lançamento |
| **Máximo de parcelas permitidas** | 12 | Teto de parcelas que o condômino pode escolher |
| **Valor mínimo por parcela (R$)** | R$ 50,00 | Opções com valor de parcela abaixo deste limite não são oferecidas |

Clique em **Salvar parâmetros** para confirmar. Os valores entram em vigor imediatamente para novos acordos — acordos já criados não são afetados.

## Aba Categorias

Gerencia as categorias de cada módulo, organizadas em 7 sub-abas:

![Aba Categorias com sub-abas por módulo](/assets/screenshots/80-config-categorias.png)
**Financeiro**, **Tarefas**, **Compras e Serviços**, **Documentos**,
**Mural**, **Fornecedores** e **Itens**.

Selecione a sub-aba do módulo desejado. Para cada categoria é possível:

- **Adicionar** — clique em **+ Nova Categoria**
- **Editar** — clique no ícone de lápis
- **Excluir** — clique no ícone de lixeira (com confirmação)

Os botões ficaram **maiores** e o de excluir foi **afastado** do de editar, para reduzir o toque errado no celular.

### A categoria da taxa condominial

Na sub-aba **Financeiro**, uma categoria pode ser marcada como **“É a taxa condominial (cota) das unidades”**. Lançamentos dessa categoria são vinculados a uma unidade, entram no **lançamento em lote da cota** e contam na **inadimplência**.

O indicador se chamava antes *“Considerar no cálculo de inadimplência”*, o que descrevia só metade do efeito e escondia o principal: **sem nenhuma categoria marcada, o lançamento em lote abre com a lista de categorias vazia** e não há como lançar a cota do mês.

{: .note }
> **Condomínio novo já nasce com ela**
>
> A categoria **Taxas de condomínio** é criada junto com o condomínio e **já vem marcada** como a taxa condominial. Não é mais preciso descobrir esse ajuste depois de esbarrar na lista vazia. Condomínios criados antes continuam como estão — se o seu não tem nenhuma categoria marcada, marque uma aqui.

### O que acontece ao excluir uma categoria

Não é igual em todas as sub-abas, e a caixa de confirmação agora diz exatamente o que vai acontecer em cada caso. Leia antes de confirmar:

| Sub-aba | O que acontece ao excluir |
|---|---|
| **Financeiro** | A categoria sai da lista, mas o **registro fica guardado** e os lançamentos antigos continuam com ela. Nada no histórico é reescrito |
| **Itens** | A categoria sai da lista e deixa de ser oferecida em itens novos. O **registro fica guardado** |
| **Tarefas** | A categoria é **excluída permanentemente** |
| **Compras e Serviços** | A categoria é **excluída permanentemente** |
| **Documentos** | A categoria é **excluída permanentemente** |
| **Mural** | A categoria é **excluída permanentemente** |
| **Fornecedores** | A categoria é **excluída permanentemente** |

{: .warning }
> **"Permanentemente" quer dizer permanentemente**
>
> Nas cinco sub-abas marcadas acima, a categoria some de vez — não fica arquivada e **não há como recuperá-la**, nem com a nossa ajuda. Se a intenção é apenas parar de usá-la, prefira renomeá-la ou simplesmente deixar de oferecê-la em registros novos.

{: .tip }
> **E se eu excluir alguma coisa por engano?**
>
> Fora dessas cinco listas de categoria, quase tudo no V3RCondo é guardado quando você exclui — lançamento financeiro, aviso do mural, tarefa, compra, item do condômino, parceiro. O registro sai das listas e dos relatórios, mas continua lá, e **dá para recuperar com a nossa ajuda** se tiver sido engano. Fale com o suporte informando o que foi excluído e quando.
>
> **Exceção: documentos das categorias Relatórios, Compras e Serviços, Manutenção e Outros.** Nessas quatro, excluir um arquivo é definitivo — ver [Documentos](/modulos/documentos/). Atas de assembleia e comprovantes financeiros continuam recuperáveis.

{: .tip }
> **Categorias financeiras**
>
> A sub-aba Financeiro divide as categorias em quatro grupos: **Receita**,
> **Despesa**, **Ambos** e **Transferência**. O grupo Transferência reúne
> categorias usadas para classificar transferências entre contas (ex: Fundo
> de Reserva, Reserva para equipamentos). Informe o tipo ao criar uma nova
> categoria.

![Sub-aba Financeiro mostrando os quatro grupos — Receita, Despesa, Ambos e Transferência](/assets/screenshots/config-categorias-quatro-tipos.png)

{: .note }
> **A categoria Reservas tem o tipo travado**
>
> A categoria **Reservas** recebe as taxas pagas nas [reservas de áreas e
> itens](/modulos/nosso-condominio/), na aba Reservas, então ela precisa
> continuar aceitando receita. Ao editá-la, o campo Tipo aparece bloqueado, com a
> explicação na tela — e não é possível mudá-la para Despesa nem Transferência.
> O nome continua livre para editar.
>
> ![Modal de edição da categoria Reservas com o campo Tipo bloqueado e a explicação](/assets/screenshots/config-categoria-reservas-bloqueada.png)

{: .tip }
> **Categorias de Itens**
>
> As categorias padrão de Itens (**Pet**, **Veículo**, **Vaga de garagem**)
> não podem ser excluídas. Categorias personalizadas só podem ser excluídas
> se não houver itens vinculados a elas.

## Aba Contas Bancárias

Lista as contas bancárias com: nome, banco, agência, conta e saldo inicial.
Quando informados, o **código do banco** aparece entre parênteses ao lado do
nome do banco e o **dígito** aparece junto do número da conta. A conta marcada
como **Padrão** é pré-selecionada automaticamente em novos lançamentos.

![Aba Contas Bancárias com lista de contas e indicação de conta padrão](/assets/screenshots/82-config-contas.png)

Na coluna de ações, os botões ficaram **maiores** e o de excluir foi **afastado** do de editar — no celular, o toque errado entre dois ícones colados era fácil demais.

Para adicionar uma nova conta, clique em **Adicionar conta** e preencha:

1. **Nome da conta** — ex: "Conta Inter", "Fundo de Reserva" (obrigatório)
2. **Banco** — nome do banco
3. **Código** *(opcional)* — o código de 3 dígitos do banco, aquele que aparece no extrato (ex: 237)
4. **Agência** — número da agência
5. **Conta** — número da conta
6. **Dígito** *(opcional)* — o dígito verificador da conta, o número depois do traço
7. **Tipo de conta** *(opcional)* — Conta corrente ou Conta poupança; deixe em "Não informado" se preferir
8. **Titular da conta** *(opcional)* — o nome como está registrado no banco
9. **Saldo inicial** — saldo na data de implantação (padrão: 0,00)
10. **Data do saldo inicial** — data de referência do saldo
11. **Conta padrão** — ative para pré-selecionar em novos lançamentos

{: .note }
> **Os campos novos são opcionais**
>
> Código do banco, dígito, tipo de conta e titular podem ficar em branco. As contas que você já cadastrou continuam válidas do jeito que estão — não é preciso voltar e completar nada. Preencher ajuda a identificar a conta com precisão quando o dado é usado fora do aplicativo.

![Modal de cadastro de nova conta bancária com todos os campos](/assets/screenshots/83-config-conta-modal.png)
