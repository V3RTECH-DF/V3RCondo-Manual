---
title: Notificações
parent: Módulos
nav_order: 7
---

# Notificações

{: .warning }
> **Envio de e-mails — Plano Pro**
>
> O envio de notificações por e-mail é um recurso do **plano Pro**. No plano Básico, o módulo está disponível apenas para visualizar o histórico.

O módulo de Notificações permite ao síndico enviar comunicados por e-mail para os condôminos — seja para todos de uma vez, para unidades específicas ou para um condômino individual.

![Formulário de envio de notificação com campos de título, mensagem e destinatários](/assets/screenshots/36-notificacoes-form.png)

## Enviar uma notificação *(síndico — plano Pro)*

O formulário de envio fica no topo da página. Preencha:

1. **Título** — assunto da notificação (obrigatório)
2. **Mensagem** — corpo do comunicado (obrigatório)
3. **Destinatários** — escolha entre:
    - *Todos os condôminos* — envia para todos os membros ativos
    - *Unidades específicas* — selecione uma ou mais unidades
    - *Condômino individual* — selecione um condômino pelo nome
4. **Agendar envio** — ative para definir data e horário futuros. Deixe desativado para enviar imediatamente.

Clique em **Enviar agora** para disparar a notificação.

## Histórico de notificações

Abaixo do formulário, a seção **Histórico** lista todas as notificações enviadas com: Título, Destinatários, Data e Status. O status **Enviado** confirma que a notificação foi processada.

Para excluir uma notificação do histórico, clique no ícone de lixeira e confirme. A notificação sai do histórico e o **registro fica guardado** — mas o que já foi enviado ao morador não volta atrás.

### Cancelar um envio agendado

Um comunicado agendado para uma data futura pode ser cancelado antes de sair: use **Cancelar envio agendado** na linha do histórico.

O cancelamento agora **pede confirmação** — antes acontecia no primeiro clique, sem pergunta. A caixa avisa que o aviso não será enviado na data marcada e que **não dá para reagendá-lo por aqui**: se você ainda quiser avisar os moradores, terá de criar um comunicado novo.

![Histórico de notificações enviadas com status](/assets/screenshots/37-notificacoes-historico.png)

## Notificações via Telegram *(Básico e Pro)*

Além do e-mail, as notificações do V3RCondo podem ser entregues no **Telegram**. Para receber, conecte sua conta ao bot **@V3RCondoBot** em [Meu Perfil](/modulos/perfil/), no cartão **Como sou avisado**.

Eventos que geram notificação no Telegram (quando conectado):

- Avisos do mural
- Documentos publicados
- Comunicados enviados pelo síndico
- Respostas no Fale com o Síndico
- Reservas (confirmação, aprovação, recusa, cancelamento)
- Assembleias (edital publicado, ata disponível, cancelamento)
- Relatórios de compras
- Lembretes de cadastro incompleto

As notificações chegam em paralelo ao e-mail — quem não tiver o Telegram conectado não é afetado.

## O que cada pessoa escolhe receber

As preferências ficam em [Meu Perfil](/modulos/perfil/), no cartão **Como sou
avisado** — cada usuário, síndico ou condômino, ajusta as próprias. As escolhas
valem para o **condomínio ativo**; quem participa de mais de um troca o
condomínio no topo da tela para ajustar os outros.

Hoje você controla:

| Controle | O que faz |
|---|---|
| **Push neste aparelho** | Liga o aviso na tela do celular ou do navegador. Vale por aparelho, e tem botão para testar na hora |
| **Cobranças → E-mail** | Aviso de cobrança emitida, com Pix, boleto e link da fatura. Sempre ligado — sem ele você pode perder o vencimento da sua cota |
| **Cobranças → Push** | Aviso no celular quando a cobrança sai e nos lembretes de vencimento. Não afeta os e-mails |
| **Cobranças → Resumo diário de pagamentos** | Só para quem administra um condomínio. Um e-mail por dia com os pagamentos que entraram — valor recebido, juros e tarifas. Vale para **todos** os condomínios que você administra, e é **independente do Push**: desligar o aviso no celular não desliga mais este resumo |
| **Comunicados gerais** | Entra ou sai da lista de destinatários dos comunicados do síndico |
| **Mural de avisos** | Aviso quando um aviso novo é publicado no mural |
| **Documentos** | Aviso quando um documento novo é publicado |
| **Tarefas** | Lembrete no dia do vencimento das tarefas em que você está envolvido |
| **Receber e-mails** | Interruptor geral dos e-mails dos assuntos acima |
| **Telegram** | Conecta ou desconecta a conta do bot @V3RCondoBot |
| **Resumo por e-mail** | Frequência do panorama periódico: diário, semanal ou desativado |

{: .note }
> **A que horas os avisos saem**
>
> Os lembretes automáticos — de **assembleia**, de **reserva** e de **tarefa** — e o
> **resumo diário** de quem administra o condomínio saem sempre de manhã, no
> **horário de Brasília**: o resumo diário de pagamentos às **7h**, o lembrete de
> tarefa por volta das **7h50**, o de reserva às **8h10** e o de assembleia às
> **8h20**. Antes eles chegavam de madrugada, o que fazia o aviso ser visto só na
> manhã seguinte e, no caso do lembrete de véspera, tarde demais.

{: .note }
> **Dois resumos diferentes, dois controles diferentes**
>
> O **Resumo diário de pagamentos** (dentro de Cobranças, só para quem
> administra um condomínio) e o **Resumo por e-mail** (panorama geral do
> condomínio) são controles independentes — desligar um não afeta o outro.

{: .warning }
> **O que chega mesmo com o e-mail desligado**
>
> **Cobrança, acordos, aviso de inadimplência e convocação de assembleia** são
> comunicações financeiras e formais, com prazo e consequência. Elas continuam
> saindo por e-mail mesmo que o interruptor **Receber e-mails** esteja
> desligado.

{: .note }
> **O Telegram segue os assuntos, não o interruptor de e-mail**
>
> Se você desligar o e-mail, continua recebendo pelo Telegram os assuntos que
> deixou ligados. Para parar de receber por lá, desconecte o Telegram no perfil.

## Visão do condômino

Condôminos acessam o módulo apenas para visualizar o **histórico de comunicados recebidos**. O formulário de envio não está disponível para este perfil.
