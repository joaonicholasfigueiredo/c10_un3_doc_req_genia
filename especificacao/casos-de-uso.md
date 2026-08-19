# Casos de Uso

## Critério de seleção dos Casos de Uso

Foram selecionados seis Casos de Uso. A seleção prioriza objetivos com interação clara entre ator e sistema e que envolvem fluxo, regras de negócio, alternativas conhecidas ou relações com outros requisitos: inscrição, cancelamento, emissão de certificado, criação de evento, confirmação de pagamento com liberação condicionada e controle de reembolsos.

Nem todo requisito funcional ou História de Usuário recebeu um Caso de Uso próprio. Consultas com interação simples, necessidades candidatas sem fluxo definido, comportamentos automáticos incorporados a outros objetivos e capacidades descritas de forma ampla permanecem representados nos demais artefatos. Isso evita criar Casos de Uso superficiais ou atribuir responsabilidades não elicitadas.

Todos os Casos de Uso selecionados estão parcialmente especificados. As lacunas existentes impedem completar precondições, sequências, alternativas ou pós-condições sem suposição; esses limites são indicados pelos respectivos IDs de DL.

## CU-01 — Realizar inscrição

**Objetivo:**  
Permitir que o participante se inscreva em eventos e workshops, considerando as regras conhecidas sobre vagas e as condições ainda pendentes.

**Ator principal:**  
Participante

**Atores secundários:**  
Nenhum ator secundário explicitamente identificado.

**Requisitos relacionados:**  
RF-02, RF-08, RF-09

**Histórias relacionadas:**  
HU-02, HU-08, HU-09

**Regras de negócio relacionadas:**  
RN-01, RN-03, RN-04, RN-06, RN-07

**Lacunas relacionadas:**  
DL-02, DL-08, DL-10, DL-11, DL-12, DL-13, DL-15, DL-16, DL-19, DL-21, DL-30

**Status:**  
Parcialmente especificado

### Precondições

Não completamente definidas — ver DL-02 e DL-13.

### Gatilho

O participante solicita realizar uma inscrição em um evento ou workshop.

### Fluxo principal

1. O participante solicita a inscrição no evento ou workshop de seu interesse.
2. O sistema recebe a solicitação de inscrição.
3. Os dados, as etapas e os pré-requisitos necessários para prosseguir dependem da definição registrada em DL-02 e da relação entre evento, workshop e atividade registrada em DL-13.
4. O sistema deve considerar o número de vagas, conforme RF-08 e RN-03; o nível da capacidade, o momento de ocupação da vaga e a concorrência pelas últimas vagas dependem de DL-10 e DL-15.
5. Para as inscrições às quais a confirmação de pagamento se aplicar, a liberação depende dessa confirmação, conforme RN-06; a abrangência e o significado de “liberação” dependem de DL-11, DL-19 e DL-21.
6. A conclusão e o resultado detalhado da inscrição permanecem parcialmente definidos devido às pendências indicadas.

### Fluxos alternativos e exceções

1. **Evento lotado:** as inscrições estão sujeitas às vagas disponíveis, conforme RN-03. A existência de lista de espera é um comportamento candidato de RF-09 e RN-04; sua obrigatoriedade e seu tratamento estão pendentes — ver DL-08 e DL-16.
2. **Atividades com conflito de horário:** workshops no mesmo horário podem ocorrer simultaneamente, conforme RN-07. O tratamento da tentativa de inscrição com sobreposição está pendente — ver DL-12.
3. **Evento gratuito ou pago:** existem ambas as modalidades, conforme RN-01. As regras de cobrança e seus efeitos no fluxo de inscrição estão pendentes — ver DL-11 e DL-21.
4. **Falha ou divergência entre inscrição, vaga e pagamento:** tratamento pendente — ver DL-30.

### Pós-condições

Pós-condição parcialmente definida — ver DL-02, DL-10, DL-11 e DL-15.

### Pontos pendentes

- Dados, etapas e pré-requisitos da inscrição: DL-02.
- Relação entre evento, workshop e atividade: DL-13.
- Ocupação, liberação e concorrência de vagas: DL-10 e DL-15.
- Abrangência e significado da liberação condicionada a pagamento: DL-11, DL-19 e DL-21.
- Conflitos de horário: DL-12.
- Obrigatoriedade e funcionamento da lista de espera candidata: DL-08 e DL-16.
- Tratamento de falhas e divergências: DL-30.

## CU-02 — Cancelar inscrição

**Objetivo:**  
Permitir que o participante cancele sua própria inscrição quando o evento admitir cancelamento.

**Ator principal:**  
Participante

**Atores secundários:**  
Nenhum ator secundário explicitamente identificado.

**Requisitos relacionados:**  
RF-05, RF-08

**Histórias relacionadas:**  
HU-05, HU-08

**Regras de negócio relacionadas:**  
RN-02, RN-03, RN-05

**Lacunas relacionadas:**  
DL-05, DL-06, DL-07, DL-08, DL-15, DL-20

**Status:**  
Parcialmente especificado

### Precondições

O participante possui a inscrição que deseja cancelar. As condições adicionais e o prazo aplicável não estão completamente definidos — ver DL-05 e DL-06.

### Gatilho

O participante solicita o cancelamento de sua inscrição.

### Fluxo principal

1. O participante solicita cancelar sua própria inscrição.
2. O sistema considera se o evento admite cancelamento, conforme RN-02.
3. A verificação do prazo e das demais condições para prosseguir depende de DL-05 e DL-06.
4. Quando o cancelamento for admitido e as condições aplicáveis forem atendidas, o sistema cancela a inscrição sem exigir contato do participante com a organização.
5. Os efeitos do cancelamento sobre vaga, lista de espera e eventual reembolso permanecem pendentes — ver DL-07, DL-08, DL-15 e DL-20.

### Fluxos alternativos e exceções

1. **Evento que não admite cancelamento:** o cancelamento não é realizado, conforme RN-02.
2. **Situação com ou sem direito a reembolso:** a existência dessas duas possibilidades é estabelecida por RN-05, mas os critérios e o tratamento estão pendentes — ver DL-07 e DL-20.
3. **Efeito sobre vaga e lista de espera:** tratamento pendente — ver DL-08 e DL-15.

### Pós-condições

A inscrição é cancelada quando o evento admite cancelamento e as condições aplicáveis são atendidas. Os efeitos sobre vaga, lista de espera e reembolso permanecem parcialmente definidos — ver DL-07, DL-08, DL-15 e DL-20.

### Pontos pendentes

- Prazo para cancelamento: DL-05.
- Configuração e demais condições de cancelamento: DL-06.
- Critérios e alcance do reembolso: DL-07 e DL-20.
- Efeitos sobre vaga e lista de espera: DL-08 e DL-15.

## CU-03 — Emitir certificado

**Objetivo:**  
Permitir que o participante emita seu certificado depois do evento.

**Ator principal:**  
Participante

**Atores secundários:**  
Nenhum ator secundário explicitamente identificado.

**Requisitos relacionados:**  
RF-06

**Histórias relacionadas:**  
HU-06

**Regras de negócio relacionadas:**  
Nenhuma regra de negócio diretamente relacionada.

**Lacunas relacionadas:**  
DL-09

**Status:**  
Parcialmente especificado

### Precondições

Não completamente definidas — ver DL-09.

### Gatilho

O participante solicita emitir seu certificado depois do evento.

### Fluxo principal

1. O participante solicita a emissão de seu certificado.
2. A continuidade do fluxo depende da definição dos critérios de elegibilidade e da eventual confirmação de presença registradas em DL-09.
3. Quando os critérios que vierem a ser definidos forem atendidos, o sistema permite ao participante emitir o certificado.

### Fluxos alternativos e exceções

Não há fluxos alternativos ou exceções suficientemente definidos. A eventual ausência de elegibilidade depende da definição registrada em DL-09.

### Pós-condições

Pós-condição parcialmente definida — ver DL-09.

### Pontos pendentes

- Critérios de elegibilidade, eventual confirmação de presença, geração e disponibilização do certificado: DL-09.

## CU-04 — Criar evento

**Objetivo:**  
Permitir que o organizador crie eventos.

**Ator principal:**  
Organizador

**Atores secundários:**  
Nenhum ator secundário explicitamente identificado.

**Requisitos relacionados:**  
RF-07

**Histórias relacionadas:**  
HU-07

**Regras de negócio relacionadas:**  
RN-01, RN-02

**Lacunas relacionadas:**  
DL-06, DL-13, DL-14

**Status:**  
Parcialmente especificado

### Precondições

Não completamente definidas — ver DL-14.

### Gatilho

O organizador solicita criar um evento.

### Fluxo principal

1. O organizador solicita a criação de um evento.
2. O sistema permite ao organizador criar o evento.
3. Os dados necessários, as etapas de criação, o ciclo de vida e a relação entre evento, workshop e atividade dependem de DL-13 e DL-14.
4. RN-01 e RN-02 estabelecem condições do domínio que afetam eventos, mas a documentação não define quem determina ou mantém a modalidade financeira nem quem configura a permissão de cancelamento — ver DL-06.

### Fluxos alternativos e exceções

Não há fluxos alternativos ou exceções suficientemente definidos.

### Pós-condições

Um evento é criado. Seus dados, sua estrutura e seu estado resultante não estão completamente definidos — ver DL-13 e DL-14.

### Pontos pendentes

- Relação entre evento, workshop e atividade: DL-13.
- Dados, etapas e ciclo de vida do evento: DL-14.
- Responsabilidade e condições para configurar a permissão de cancelamento: DL-06.
- A documentação não atribui a um stakeholder a definição ou manutenção da modalidade financeira do evento.

## CU-05 — Confirmar pagamento e tratar liberação condicionada

**Objetivo:**  
Permitir que a equipe financeira confirme pagamentos e representar a condição conhecida para liberação de determinadas inscrições.

**Ator principal:**  
Equipe Financeira

**Atores secundários:**  
Nenhum ator secundário explicitamente identificado.

**Requisitos relacionados:**  
RF-13, RF-15, RF-16

**Histórias relacionadas:**  
HU-12

**Regras de negócio relacionadas:**  
RN-01, RN-03, RN-06

**Lacunas relacionadas:**  
DL-10, DL-11, DL-19, DL-21, DL-30

**Status:**  
Parcialmente especificado

### Precondições

Não completamente definidas — ver DL-11, DL-19 e DL-21.

### Gatilho

A equipe financeira solicita confirmar o pagamento de uma inscrição.

### Fluxo principal

1. A equipe financeira solicita registrar a confirmação do pagamento de uma inscrição.
2. O sistema permite à equipe financeira confirmar o pagamento, conforme RF-13.
3. A origem da confirmação, os estados de pagamento e o tratamento de falhas ou correções dependem de DL-19 e DL-30.
4. Para determinadas inscrições, a confirmação deve ocorrer antes da liberação, conforme RF-16 e RN-06.
5. As inscrições sujeitas a essa condição e o significado operacional de “liberação” dependem de DL-11.
6. O efeito da confirmação sobre a ocupação da vaga depende de DL-10.

### Fluxos alternativos e exceções

1. **Modalidade financeira do evento:** RF-15 e RN-01 estabelecem que há eventos gratuitos e eventos sujeitos a pagamento. Este Caso de Uso não atribui à equipe financeira a responsabilidade por definir ou manter essa modalidade.
2. **Pagamento não confirmado, divergente ou corrigido:** tratamento pendente — ver DL-19 e DL-30.
3. **Inscrição que não depende de confirmação para liberação:** a existência de “determinadas inscrições” sujeitas à condição é conhecida, mas a abrangência e o tratamento da alternativa estão pendentes — ver DL-11.

### Pós-condições

A confirmação do pagamento é registrada. A eventual liberação da inscrição e seus efeitos sobre a vaga permanecem parcialmente definidos — ver DL-10 e DL-11.

### Pontos pendentes

- Inscrições condicionadas e significado operacional de liberação: DL-11.
- Processo, estados, falhas e correções da confirmação: DL-19 e DL-30.
- Momento de ocupação da vaga: DL-10.
- Cobrança de eventos pagos: DL-21.
- Responsabilidade pela definição ou manutenção da modalidade financeira não atribuída pela elicitação.
- O Caso de Uso não pressupõe processamento de pagamentos pelo sistema.

## CU-06 — Controlar reembolsos

**Objetivo:**  
Permitir que a equipe financeira controle reembolsos, preservando a indefinição sobre as operações abrangidas por esse controle.

**Ator principal:**  
Equipe Financeira

**Atores secundários:**  
Nenhum ator secundário explicitamente identificado.

**Requisitos relacionados:**  
RF-14

**Histórias relacionadas:**  
HU-13

**Regras de negócio relacionadas:**  
RN-05

**Lacunas relacionadas:**  
DL-07, DL-20, DL-30

**Status:**  
Parcialmente especificado

### Precondições

Não completamente definidas — ver DL-07 e DL-20.

### Gatilho

A equipe financeira solicita controlar um reembolso.

### Fluxo principal

1. A equipe financeira solicita realizar uma operação de controle de reembolso.
2. O sistema permite à equipe financeira controlar reembolsos, conforme RF-14.
3. As operações compreendidas pelo verbo “controlar” dependem da definição registrada em DL-20.
4. A aplicação da regra que distingue situações com e sem direito a reembolso depende dos critérios pendentes em DL-07.
5. O tratamento de falhas ou divergências permanece pendente — ver DL-30.

### Fluxos alternativos e exceções

1. **Situação com direito a reembolso:** o tratamento depende dos critérios e das operações ainda não definidos — ver DL-07 e DL-20.
2. **Situação sem direito a reembolso:** o tratamento depende dos critérios e das operações ainda não definidos — ver DL-07 e DL-20.

### Pós-condições

Pós-condição parcialmente definida — ver DL-07, DL-20 e DL-30.

### Pontos pendentes

- Critérios que determinam o direito a reembolso: DL-07.
- Operações abrangidas pelo controle de reembolsos: DL-20.
- Tratamento de falhas e divergências: DL-30.
- O Caso de Uso não pressupõe aprovação, cálculo, solicitação, processamento, transferência ou execução financeira do reembolso.

## Cobertura e limitações

Os Casos de Uso cobrem diretamente RF-02, RF-05, RF-06, RF-07, RF-08, RF-09, RF-13, RF-14, RF-15 e RF-16, além de HU-02, HU-05, HU-06, HU-07, HU-08, HU-09, HU-12 e HU-13. RF-09 e HU-09 aparecem somente como comportamento candidato dentro de CU-01. RF-15 aparece em CU-05 apenas como condição de domínio aplicável a pagamentos; nenhum ator foi indicado como responsável por definir ou manter a modalidade financeira.

RF-01, RF-03, RF-04, RF-10, RF-11, RF-12, RF-17 e RF-18, assim como HU-01, HU-03, HU-04, HU-10, HU-11, HU-14 e HU-15, permanecem representados nos demais artefatos. Não receberam Casos de Uso próprios porque correspondem a consultas simples, necessidade candidata sem fluxo confirmado ou capacidades cujo detalhamento atual não sustenta uma sequência comportamental relevante. Sua ausência como CU próprio não os exclui do projeto.

RF-08 e HU-08 foram incorporados aos fluxos de inscrição e cancelamento, pois o controle de vagas é um comportamento automático relacionado a esses objetivos, e não uma interação independente iniciada por ator. RF-09 e HU-09 não originaram CU candidato próprio porque a obrigatoriedade e todo o funcionamento da lista de espera permanecem pendentes. RF-04 e HU-04 também continuam candidatos e não possuem fluxo suficiente para justificar um CU próprio.

As lacunas que mais limitaram os fluxos foram DL-02, DL-05, DL-07, DL-08, DL-09, DL-10, DL-11, DL-13, DL-14, DL-15, DL-19, DL-20, DL-21 e DL-30. Nenhum desses pontos foi resolvido por suposição, e nenhum estado formal, prazo, mecanismo de pagamento, política de conflito, política de lista de espera, critério de certificado ou operação financeira de reembolso foi criado.
