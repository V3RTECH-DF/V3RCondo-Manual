---
title: Receber um morador novo
parent: Fluxos
nav_order: 3
---

# Receber um morador novo

## Por que isto importa

Um morador que chega e não consegue entrar no aplicativo, ou entra e não encontra a própria unidade, começa a relação com o V3RCondo pelo lado errado — e volta a procurar o síndico pelos mesmos canais de sempre (WhatsApp, papel no elevador) que o aplicativo deveria substituir. Cadastrar direito da primeira vez evita isso: a pessoa certa, na unidade certa, com o histórico da unidade já esperando por ela.

Há três portas de entrada diferentes, e escolher a certa evita retrabalho.

## Passo a passo

### 1. Escolha como o morador vai entrar

| Situação | Caminho |
|---|---|
| Você tem o e-mail da pessoa e quer cadastrar na hora | **Adicionar condômino diretamente** |
| Você está recebendo vários moradores de uma vez — mudança de gestão, condomínio novo | **Importar planilha** |
| O morador já tentou se cadastrar sozinho pelo app | **Aprovar a solicitação pendente** |

Todos os três caminhos ficam em [Configurações → Condôminos](/modulos/configuracoes/#aba-condôminos).

### 2a. Cadastro direto

Clique em **+ Adicionar condômino** e preencha nome completo, e-mail, unidade e título (Condômino, por padrão). O sistema cadastra a pessoa na hora e envia um e-mail de boas-vindas com instruções para definir a senha ou entrar com o Google.

### 2b. Importação por planilha

Clique em **Importar planilha**, baixe o modelo, preencha Nome, E-mail, Unidade e Título para cada morador e faça o upload. O sistema processa linha a linha, ignora e-mails já cadastrados e mostra um resumo com importados, ignorados e rejeitados — com o motivo de cada rejeição. Limite de 100 condôminos por importação; mais que isso, faça em duas levas.

### 2c. Solicitação do próprio morador

Quando alguém escolhe, na tela de cadastro do app, a porta **"Fui convidado para um condomínio"** e busca o seu condomínio pelo nome, a solicitação aparece **acima da lista**, em Configurações → Condôminos, esperando por você. Clique em **Aprovar** — ou **Rejeitar**, se a pessoa não for de fato do condomínio.

{: .tip }
> **Convite por e-mail é outro caminho, sem solicitação a aprovar**
>
> Se você já cadastrou a pessoa pelo caminho 2a com o e-mail correto, e ela recebe o convite e clica no link, o vínculo é feito automaticamente — não sobra solicitação pendente para aprovar.

### 3. Defina a unidade e o responsável

Uma unidade pode ter mais de um morador vinculado, mas só **um responsável** — é ele quem recebe notificações extrajudiciais e aparece nos documentos gerados para a unidade. Se o novo morador é quem deve constar como responsável, confirme isso em Configurações → Condôminos: o badge laranja **Responsável** marca quem está nessa posição hoje, e o botão **Transferir** troca para outra pessoa da mesma unidade quando for o caso.

### 4. O que o morador vê no primeiro acesso

Depois de criar a senha (ou entrar com o Google), o novo morador passa por até três telas, nesta ordem, antes de chegar ao Dashboard:

1. **Aceite dos Termos de Uso e da Política de Privacidade** — obrigatório, uma vez só (ou de novo, quando os documentos mudam de versão). Ver [Primeiros Passos — Aceitar os Termos de Uso](/guia/primeiros-passos/#aceitar-os-termos-de-uso-e-a-política-de-privacidade).
2. **Complete seu cadastro** — pede telefone e CPF/CNPJ, se algum estiver em branco. Não é obrigatório; **Agora não** adia, e a janela não insiste mais de uma vez por semana.
3. **Seleção de condomínio** — só aparece se a pessoa tiver vínculo com mais de um condomínio.

Daí em diante, o morador vê o Dashboard com o resumo da própria unidade, e o menu lateral sem os módulos exclusivos do síndico.

### 5. Confira que a pessoa enxerga a própria unidade

Peça ao morador para abrir **Minha Área → Extrato da Unidade** e confirmar que o histórico da unidade (ou "sem lançamentos ainda", se a unidade for nova) aparece corretamente. É a prova de que o vínculo unidade↔morador está certo — não apenas que a conta foi criada.

![Extrato da Unidade com o responsável pela unidade, os totais Cobrado, Pago, Em Aberto e Em Atraso, e a tabela de lançamentos por competência](/assets/screenshots/fluxo-receber-morador-01-extrato-unidade.png)

## Exemplo concreto

A unidade 302 do Edifício Aurora foi vendida. O síndico cadastra o novo morador em **+ Adicionar condômino** com o e-mail dele e a unidade **302**, e transfere o badge de **Responsável** da antiga proprietária para o novo morador. O morador recebe o e-mail de boas-vindas, define a senha, aceita os Termos de Uso, preenche o CPF na janela de cadastro completo, e já vê no Extrato da Unidade os lançamentos em aberto daquele mês.

## Dicas e armadilhas

- **Um e-mail errado no cadastro direto vira um convite que nunca chega.** Confira o e-mail antes de salvar — não há como o app avisar que a pessoa nunca recebeu nada.
- **Se a pessoa já morou no condomínio antes, cadastre de novo com o mesmo e-mail** em vez de tentar "reativar" de outro jeito: o vínculo anterior é reaproveitado automaticamente, sem duplicar cadastro nem perder histórico.
- **Solicitação pendente não vence sozinha.** Uma solicitação esquecida fica ali indefinidamente — vale conferir a lista de tempos em tempos, não só quando alguém reclama.

## Quando dá errado

| O que você vê | O que fazer |
|---|---|
| Morador diz que não recebeu o e-mail de boas-vindas | Confira o e-mail cadastrado em Configurações → Condôminos; se estiver certo, peça para checar a caixa de spam antes de recadastrar |
| Morador cadastrado, mas com a unidade vazia | Edite o membro (ícone de lápis) e preencha a unidade — sem ela, o morador não aparece nas listas por unidade nem no lançamento em lote |
| Duas pessoas aparecem como responsável pela mesma unidade | Não deveria acontecer — o sistema mantém sempre um único responsável por unidade; se você observar isso, é um comportamento a reportar |
| Solicitação de vínculo de alguém que não é do condomínio | Clique em **Rejeitar** — a pessoa não é cadastrada e pode tentar novamente com os dados certos |
