# Requisitos funcionais

Os requisitos abaixo foram extraídos exclusivamente do documento de elicitação. Quando o comportamento geral está identificado, mas suas condições ainda não foram definidas, a pendência é indicada nas observações e rastreada em `duvidas-e-lacunas.md`.

## RF-01 — Consultar eventos disponíveis

**Descrição:**  
O sistema deverá permitir ao participante visualizar os eventos disponíveis em um único local.

**Fonte:**  
Entrevista com Participantes, item 1: “Gostaria de visualizar todos os eventos disponíveis em um único lugar.”

**Observações:**  
O significado de “disponíveis” e as informações que devem aparecer na consulta ainda precisam ser definidos (DL-01).

## RF-02 — Realizar inscrição

**Descrição:**  
O sistema deverá permitir ao participante inscrever-se em eventos e workshops.

**Fonte:**  
Stakeholders — Participantes: interesse em “inscrever-se em eventos”; entrevista com Participantes, item 5, sobre inscrição em vários workshops.

**Observações:**  
Os dados, as etapas e as condições da inscrição não foram detalhados (DL-02). O tratamento de atividades com conflito de horário também está pendente (DL-12).

## RF-03 — Acompanhar inscrições próprias

**Descrição:**  
O sistema deverá permitir ao participante acompanhar suas inscrições.

**Fonte:**  
Stakeholders — Participantes: interesse em “acompanhar inscrições”.

**Observações:**  
Os estados e dados apresentados no acompanhamento não foram definidos (DL-03).

## RF-04 — Emitir comprovante de inscrição

**Descrição:**  
O sistema deverá emitir um comprovante após a inscrição do participante.

**Fonte:**  
Entrevista com Participantes, item 2: “Seria interessante receber um comprovante logo após a inscrição.”

**Observações:**  
O conteúdo, o formato e o meio de disponibilização ou envio do comprovante não foram definidos (DL-04).

## RF-05 — Cancelar inscrição

**Descrição:**  
O sistema deverá permitir ao participante cancelar sua própria inscrição, quando o evento admitir cancelamento, sem precisar entrar em contato com a organização.

**Fonte:**  
Stakeholders — Participantes: interesse em “cancelar participação”; entrevista com Participantes, item 3; entrevista com Organizadores, item 3: “Nem todos os eventos permitem o cancelamento da inscrição.”

**Observações:**  
O prazo e as demais condições de cancelamento ainda não foram definidos (DL-05 e DL-06).

## RF-06 — Emitir certificado

**Descrição:**  
O sistema deverá permitir ao participante emitir seu certificado depois do evento.

**Fonte:**  
Stakeholders — Participantes: interesse em “emitir certificados”; entrevista com Participantes, item 4.

**Observações:**  
Os critérios de elegibilidade, inclusive a eventual confirmação de presença, não foram definidos (DL-09).

## RF-07 — Criar eventos

**Descrição:**  
O sistema deverá permitir ao organizador criar eventos.

**Fonte:**  
Stakeholders — Organizadores: interesse em “criar eventos”.

**Observações:**  
Os dados obrigatórios, o ciclo de vida e a relação entre eventos, workshops e atividades não foram definidos (DL-13 e DL-14).

## RF-08 — Controlar vagas automaticamente

**Descrição:**  
O sistema deverá controlar automaticamente o número de vagas dos eventos.

**Fonte:**  
Entrevista com Organizadores, item 1: “Precisamos controlar automaticamente o número de vagas.”

**Observações:**  
Não foi definido se a capacidade é controlada por evento, workshop ou atividade, nem em que momento uma vaga é ocupada ou liberada (DL-10 e DL-15).

## RF-09 — Manter lista de espera

**Descrição:**  
O sistema deverá permitir a manutenção de uma lista de espera quando um evento estiver lotado.

**Fonte:**  
Entrevista com Organizadores, item 2: “Quando um evento lotar, seria interessante criar uma lista de espera.”

**Observações:**  
O funcionamento da lista de espera não foi informado (DL-08). A expressão “seria interessante” também requer validação de prioridade e obrigatoriedade com os stakeholders (DL-16).

## RF-10 — Consultar quantidade de inscritos

**Descrição:**  
O sistema deverá permitir ao organizador acompanhar a quantidade atual de inscritos.

**Fonte:**  
Entrevista com Organizadores, item 4: “Gostaríamos de acompanhar a quantidade de inscritos em tempo real.”

**Observações:**  
A atualização esperada para “em tempo real” não foi quantificada e exige elicitação complementar (DL-17).

## RF-11 — Acompanhar inscrições do evento

**Descrição:**  
O sistema deverá permitir ao organizador acompanhar as inscrições dos eventos.

**Fonte:**  
Stakeholders — Organizadores: interesse em “acompanhar inscrições”.

**Observações:**  
As informações e operações incluídas nesse acompanhamento ainda precisam ser definidas (DL-18).

## RF-12 — Gerenciar participantes

**Descrição:**  
O sistema deverá permitir ao organizador gerenciar participantes.

**Fonte:**  
Stakeholders — Organizadores: interesse em “gerenciar participantes”.

**Observações:**  
As operações incluídas em “gerenciar” não foram especificadas (DL-18).

## RF-13 — Registrar confirmação de pagamento

**Descrição:**  
O sistema deverá permitir à equipe financeira confirmar pagamentos de inscrições.

**Fonte:**  
Stakeholders — Equipe Financeira: interesse em “confirmar pagamentos”; entrevista com a Equipe Financeira, item 3.

**Observações:**  
Não foi definido se a confirmação será manual ou obtida por integração, nem quais estados de pagamento existirão (DL-19). A elicitação não afirma que o sistema processará pagamentos.

## RF-14 — Controlar reembolsos

**Descrição:**  
O sistema deverá permitir à equipe financeira controlar os reembolsos.

**Fonte:**  
Stakeholders — Equipe Financeira: interesse em “controlar reembolsos”; entrevista com a Equipe Financeira, item 2.

**Observações:**  
O alcance de “controlar” e as situações que dão direito a reembolso não foram definidos (DL-07 e DL-20). A elicitação não afirma que o sistema executará a transferência financeira do reembolso.

## RF-15 — Distinguir eventos gratuitos e pagos

**Descrição:**  
O sistema deverá permitir que eventos sejam identificados como gratuitos ou como sujeitos a pagamento.

**Fonte:**  
Entrevista com a Equipe Financeira, item 1: “Alguns eventos são gratuitos e outros exigem pagamento.”

**Observações:**  
Não foram definidos preços, formas de pagamento ou regras de cobrança (DL-21).

## RF-16 — Liberar inscrição condicionada à confirmação de pagamento

**Descrição:**  
O sistema deverá liberar as inscrições para as quais essa condição se aplique somente após a confirmação do pagamento.

**Fonte:**  
Entrevista com a Equipe Financeira, item 3: “Precisamos confirmar os pagamentos antes de liberar determinadas inscrições.”

**Observações:**  
Não foi definido quais inscrições estão sujeitas a essa condição, nem o significado operacional de “liberar” uma inscrição (DL-11).

## RF-17 — Consultar programação

**Descrição:**  
O sistema deverá permitir ao palestrante consultar a programação.

**Fonte:**  
Stakeholders — Palestrantes: interesse em “consultar a programação”.

**Observações:**  
O escopo e os detalhes exibidos na programação não foram definidos (DL-22).

## RF-18 — Consultar participantes das próprias atividades

**Descrição:**  
O sistema deverá permitir ao palestrante consultar a lista de participantes inscritos em suas atividades.

**Fonte:**  
Entrevista com Palestrantes, item 1: “Gostaria de consultar a lista de participantes inscritos em minhas atividades.”

**Observações:**  
As informações de cada participante que poderão ser exibidas não foram definidas (DL-23).
