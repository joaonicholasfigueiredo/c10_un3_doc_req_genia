# Critérios de Aceitação

## Critério de seleção

Os Critérios de Aceitação desta versão são seletivos. Somente comportamentos para os quais contexto, ação e resultado observável podem ser derivados da documentação consolidada receberam critérios.

A cobertura numérica de 100% não foi utilizada como objetivo. Necessidades candidatas e comportamentos dependentes de decisões ainda abertas permanecem sem Critério de Aceitação completo quando sua formulação exigiria suposições. A ausência de CA não exclui o requisito, a História de Usuário ou o Caso de Uso do projeto.

# Participante

## CA-01 — Consultar eventos disponíveis em um único local

**História relacionada:**  
HU-01

**Caso de Uso relacionado:**  
Nenhum Caso de Uso relacionado nesta versão.

**Requisitos relacionados:**  
RF-01

**Regras de negócio relacionadas:**  
Nenhuma regra de negócio diretamente relacionada.

**Lacunas relevantes:**  
DL-01

**Critério:**

Dado que existam eventos considerados disponíveis  
Quando o participante solicitar a consulta dos eventos disponíveis  
Então o sistema apresentará esses eventos em um único local.

**Limites da validação:**  
O critério não define o que torna um evento disponível nem quais informações são apresentadas, pontos ainda pendentes em DL-01.

## CA-02 — Acompanhar inscrições próprias

**História relacionada:**  
HU-03

**Caso de Uso relacionado:**  
Nenhum Caso de Uso relacionado nesta versão.

**Requisitos relacionados:**  
RF-03

**Regras de negócio relacionadas:**  
Nenhuma regra de negócio diretamente relacionada.

**Lacunas relevantes:**  
DL-03, DL-11

**Critério:**

Dado que o participante possua inscrições  
Quando solicitar o acompanhamento de suas inscrições  
Então o sistema apresentará as inscrições associadas a esse participante.

**Limites da validação:**  
O critério valida somente a possibilidade de consultar as próprias inscrições. Não define os dados, os estados apresentados nem o significado de inscrição liberada, ainda pendentes em DL-03 e DL-11.

## CA-03 — Impedir cancelamento em evento que não o admite

**História relacionada:**  
HU-05

**Caso de Uso relacionado:**  
CU-02

**Requisitos relacionados:**  
RF-05

**Regras de negócio relacionadas:**  
RN-02

**Lacunas relevantes:**  
DL-05, DL-06, DL-07, DL-08, DL-15, DL-20

**Critério:**

Dado que o participante possua uma inscrição em um evento que não admite cancelamento  
Quando solicitar o cancelamento dessa inscrição  
Então o sistema não realizará o cancelamento.

**Limites da validação:**  
O critério valida somente a condição negativa estabelecida por RN-02. Não define prazo, outras condições, efeitos sobre vagas ou lista de espera nem tratamento de reembolso, ainda pendentes nas DLs relacionadas.

# Organizador

## CA-04 — Consultar quantidade de inscritos

**História relacionada:**  
HU-10

**Caso de Uso relacionado:**  
Nenhum Caso de Uso relacionado nesta versão.

**Requisitos relacionados:**  
RF-10

**Regras de negócio relacionadas:**  
Nenhuma regra de negócio diretamente relacionada.

**Lacunas relevantes:**  
DL-17, DL-18

**Critério:**

Dado que existam participantes inscritos em um evento

Quando o organizador solicitar a quantidade de inscritos desse evento

Então o sistema apresentará a quantidade de inscritos do evento.

**Limites da validação:**  
O critério valida a consulta da quantidade, mas não estabelece latência, frequência ou atualização automática para a expressão “tempo real”, pendente em DL-17. Também não valida outras informações ou operações de acompanhamento, pendentes em DL-18.

# Equipe Financeira

## CA-05 — Registrar confirmação de pagamento

**História relacionada:**  
HU-12

**Caso de Uso relacionado:**  
CU-05

**Requisitos relacionados:**  
RF-13

**Regras de negócio relacionadas:**  
Nenhuma regra de negócio diretamente validada por este critério.

**Lacunas relevantes:**  
DL-10, DL-11, DL-19, DL-21, DL-30

**Critério:**

Dado que a equipe financeira disponha da confirmação do pagamento de uma inscrição  
Quando confirmar esse pagamento no sistema  
Então o sistema registrará a confirmação associada à inscrição.

**Limites da validação:**  
O critério valida somente o registro da confirmação pela equipe financeira. Não define a origem da confirmação, estados financeiros, processamento de pagamento, inscrições condicionadas, significado de liberação nem efeitos sobre vagas.

# Palestrante

## CA-06 — Consultar programação

**História relacionada:**  
HU-14

**Caso de Uso relacionado:**  
Nenhum Caso de Uso relacionado nesta versão.

**Requisitos relacionados:**  
RF-17

**Regras de negócio relacionadas:**  
Nenhuma regra de negócio diretamente validada por este critério.

**Lacunas relevantes:**  
DL-22

**Critério:**

Dado que exista uma programação de evento  
Quando o palestrante solicitar sua consulta  
Então o sistema apresentará a programação ao palestrante.

**Limites da validação:**  
O critério não define se a consulta abrange toda a programação ou somente atividades do palestrante, nem quais detalhes são apresentados, pontos pendentes em DL-22.

## CA-07 — Consultar participantes de atividade vinculada ao palestrante

**História relacionada:**  
HU-15

**Caso de Uso relacionado:**  
Nenhum Caso de Uso relacionado nesta versão.

**Requisitos relacionados:**  
RF-18

**Regras de negócio relacionadas:**  
RN-08

**Lacunas relevantes:**  
DL-23

**Critério:**

Dado que uma atividade vinculada ao palestrante possua participantes inscritos  
Quando o palestrante solicitar a lista de participantes dessa atividade  
Então o sistema apresentará os participantes inscritos na atividade vinculada ao palestrante.

**Limites da validação:**  
O critério valida a relação entre o palestrante, sua atividade e os participantes inscritos. Não define quais informações de cada participante são apresentadas, ponto pendente em DL-23.

## Requisitos e histórias ainda sem Critério de Aceitação completo

**Elemento:**  
RF-02 / HU-02

**Motivo:**  
Informação insuficiente

**Lacunas relacionadas:**  
DL-02, DL-10, DL-11, DL-12, DL-13, DL-15, DL-21, DL-30

**O que falta definir:**  
Dados, etapas, estrutura do objeto de inscrição, ocupação da vaga, relação com pagamento, conflitos de horário e resultado final do processo.

---

**Elemento:**  
RF-04 / HU-04

**Motivo:**  
Candidata

**Lacunas relacionadas:**  
DL-04

**O que falta definir:**  
Obrigatoriedade, prioridade, conteúdo, formato e meio de entrega do comprovante.

---

**Elemento:**  
RF-06 / HU-06

**Motivo:**  
Informação insuficiente

**Lacunas relacionadas:**  
DL-09

**O que falta definir:**  
Critérios de elegibilidade, eventual confirmação de presença, geração e disponibilização do certificado.

---

**Elemento:**  
RF-07 / HU-07

**Motivo:**  
Comportamento excessivamente aberto

**Lacunas relacionadas:**  
DL-06, DL-13, DL-14

**O que falta definir:**  
Dados, etapas, ciclo de vida, estrutura entre evento e atividades e responsabilidades sobre condições configuráveis.

---

**Elemento:**  
RF-08 / HU-08

**Motivo:**  
Informação insuficiente

**Lacunas relacionadas:**  
DL-08, DL-10, DL-13, DL-15, DL-30

**O que falta definir:**  
Nível da capacidade, momentos de ocupação e liberação, concorrência pelas últimas vagas e tratamento de falhas.

---

**Elemento:**  
RF-09 / HU-09

**Motivo:**  
Candidata

**Lacunas relacionadas:**  
DL-08, DL-15, DL-16

**O que falta definir:**  
Obrigatoriedade, prioridade e funcionamento da lista de espera.

---

**Elemento:**  
RF-11 / HU-10, parcialmente

**Motivo:**  
Comportamento excessivamente aberto

**Lacunas relacionadas:**  
DL-18

**O que falta definir:**  
Informações e operações incluídas no acompanhamento das inscrições. CA-04 cobre somente RF-10, relativo à quantidade de inscritos.

---

**Elemento:**  
RF-12 / HU-11

**Motivo:**  
Comportamento excessivamente aberto

**Lacunas relacionadas:**  
DL-18

**O que falta definir:**  
Operações compreendidas pelo gerenciamento de participantes.

---

**Elemento:**  
RF-14 / HU-13

**Motivo:**  
Comportamento excessivamente aberto

**Lacunas relacionadas:**  
DL-07, DL-20, DL-30

**O que falta definir:**  
Critérios de elegibilidade e operações abrangidas pelo controle de reembolsos, sem pressupor execução financeira.

---

**Elemento:**  
RF-15 / sem História de Usuário própria

**Motivo:**  
Informação insuficiente

**Lacunas relacionadas:**  
DL-13, DL-21

**O que falta definir:**  
Responsabilidade por definir ou manter a modalidade financeira e comportamento verificável associado, sem atribuir essa responsabilidade a um stakeholder por suposição.

---

**Elemento:**  
RF-16 / HU-12, parcialmente

**Motivo:**  
Informação insuficiente

**Lacunas relacionadas:**  
DL-10, DL-11, DL-19, DL-21, DL-30

**O que falta definir:**  
Quais inscrições dependem da confirmação, o significado operacional de liberação e os efeitos sobre vagas. CA-05 cobre somente o registro da confirmação previsto em RF-13.

## Cobertura dos Critérios de Aceitação

Os critérios cobrem diretamente RF-01, RF-03, RF-05, RF-10, RF-13, RF-17 e RF-18; HU-01, HU-03, HU-05, HU-10, HU-12, HU-14 e HU-15; e relacionam-se a CU-02 e CU-05.

RF-02, RF-04, RF-06, RF-07, RF-08, RF-09, RF-11, RF-12, RF-14, RF-15 e RF-16 não receberam Critério de Aceitação completo. HU-02, HU-04, HU-06, HU-07, HU-08, HU-09, HU-11 e HU-13 permanecem sem cobertura direta completa; HU-10 e HU-12 têm cobertura parcial, limitada respectivamente a RF-10 e RF-13. CU-01, CU-03, CU-04 e CU-06 não possuem CA relacionado nesta versão porque seus fluxos dependem de decisões ainda abertas.

A cobertura seletiva preserva somente resultados atualmente verificáveis. RF-04/HU-04 e RF-09/HU-09 permanecem candidatos. Nenhuma lacuna foi resolvida por suposição e nenhum critério foi criado para requisitos não funcionais, pois não existem RNFs concretos nesta versão.
