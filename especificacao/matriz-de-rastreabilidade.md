# Matriz de Rastreabilidade

A matriz utiliza o Requisito Funcional como unidade principal e registra somente relações declaradas ou sustentadas pelos artefatos consolidados. O símbolo “—” indica ausência deliberada de artefato relacionado nesta versão, e não exclusão do requisito.

## Matriz principal

| RF | Resumo | Fonte/Stakeholder | RN relacionadas | DL relacionadas | HU | CU | CA | Situação |
|---|---|---|---|---|---|---|---|---|
| RF-01 | Consultar eventos disponíveis | Participantes — entrevista, item 1 | RN-01 | DL-01 | HU-01 | — | CA-01 | Especificação parcial — cobertura seletiva |
| RF-02 | Realizar inscrição | Participantes — interesses; entrevista, item 5 | RN-01, RN-03, RN-06, RN-07 | DL-02, DL-10, DL-11, DL-12, DL-13, DL-15, DL-21 | HU-02 | CU-01 | — | Especificação parcial — sem CA completo |
| RF-03 | Acompanhar inscrições próprias | Participantes — interesses | RN-06 | DL-03, DL-11 | HU-03 | — | CA-02 | Especificação parcial — cobertura seletiva |
| RF-04 | Obter comprovante de inscrição | Participantes — entrevista, item 2 | — | DL-04 | HU-04 | — | — | Candidato — sem CU/CA próprios |
| RF-05 | Cancelar inscrição | Participantes — interesses e entrevista, item 3; Organizadores — entrevista, item 3 | RN-02, RN-03, RN-05 | DL-05, DL-06, DL-07, DL-08, DL-15, DL-20 | HU-05 | CU-02 | CA-03 | Especificação parcial — cobertura seletiva |
| RF-06 | Emitir certificado | Participantes — interesses; entrevista, item 4 | — | DL-09 | HU-06 | CU-03 | — | Especificação parcial — sem CA completo |
| RF-07 | Criar eventos | Organizadores — interesses | RN-01, RN-02 | DL-06, DL-13, DL-14 | HU-07 | CU-04 | — | Especificação parcial — sem CA completo |
| RF-08 | Controlar vagas automaticamente | Organizadores — entrevista, item 1 | RN-03 | DL-08, DL-10, DL-13, DL-15, DL-30 | HU-08 | CU-01, CU-02 | — | Especificação parcial — sem CA completo |
| RF-09 | Manter lista de espera | Organizadores — entrevista, item 2 | RN-03, RN-04 | DL-08, DL-15, DL-16 | HU-09 | CU-01 (comportamento candidato) | — | Candidato — sem CA completo |
| RF-10 | Consultar quantidade de inscritos | Organizadores — entrevista, item 4 | — | DL-17 | HU-10 | — | CA-04 | Especificação parcial — cobertura seletiva |
| RF-11 | Acompanhar inscrições do evento | Organizadores — interesses | — | DL-18 | HU-10 | — | — | Especificação parcial — sem CA completo |
| RF-12 | Gerenciar participantes | Organizadores — interesses | — | DL-18 | HU-11 | — | — | Especificação parcial — sem CA completo |
| RF-13 | Registrar confirmação de pagamento | Equipe Financeira — interesses; entrevista, item 3 | RN-01, RN-03, RN-06 | DL-10, DL-11, DL-19, DL-21, DL-30 | HU-12 | CU-05 | CA-05 | Especificação parcial — cobertura seletiva |
| RF-14 | Controlar reembolsos | Equipe Financeira — interesses; entrevista, item 2 | RN-05 | DL-07, DL-20, DL-30 | HU-13 | CU-06 | — | Especificação parcial — sem CA completo |
| RF-15 | Distinguir eventos gratuitos e pagos | Equipe Financeira — entrevista, item 1 | RN-01 | DL-13, DL-21 | — | CU-05 (condição de domínio) | — | Sem HU própria — sem CA completo |
| RF-16 | Condicionar liberação à confirmação de pagamento | Equipe Financeira — entrevista, item 3 | RN-01, RN-03, RN-06 | DL-10, DL-11, DL-19, DL-21, DL-30 | HU-12 | CU-05 | — | Especificação parcial — sem CA completo |
| RF-17 | Consultar programação | Palestrantes — interesses | RN-07 | DL-22 | HU-14 | — | CA-06 | Especificação parcial — cobertura seletiva |
| RF-18 | Consultar participantes das próprias atividades | Palestrantes — entrevista, item 1 | RN-08 | DL-23 | HU-15 | — | CA-07 | Especificação parcial — cobertura seletiva |

RF-04 e RF-09 permanecem necessidades candidatas. A existência de HU-04, HU-09 e da referência a RF-09 em CU-01 não confirma sua obrigatoriedade.

RF-15 permanece sem História de Usuário própria. Sua presença em CU-05 representa somente a condição de domínio de que existem eventos gratuitos e eventos sujeitos a pagamento; a documentação não atribui a nenhum stakeholder a responsabilidade por definir ou manter essa modalidade.

## Requisitos não funcionais

Nenhum requisito não funcional concreto foi incluído na matriz. Segurança, desempenho, disponibilidade, acessibilidade, privacidade, usabilidade, confiabilidade e demais atributos de qualidade ainda dependem de elicitação complementar antes que possam ser formulados de maneira verificável.

## Lacunas com maior impacto transversal

| DL | Tema | RFs afetados | Artefatos afetados |
|---|---|---|---|
| DL-07 | Critérios para reembolso | RF-05, RF-14 | HU-05, HU-13; CU-02, CU-06 |
| DL-08 | Funcionamento da lista de espera | RF-05, RF-08, RF-09 | HU-05, HU-08, HU-09; CU-01, CU-02 |
| DL-10 | Momento de ocupação da vaga em inscrição paga | RF-02, RF-08, RF-13, RF-16 | HU-02, HU-08, HU-12; CU-01, CU-05 |
| DL-11 | Inscrições condicionadas e significado de liberação | RF-02, RF-03, RF-13, RF-16 | HU-02, HU-03, HU-12; CU-01, CU-05; CA-02, CA-05 (limites) |
| DL-13 | Relação entre evento, workshop e atividade | RF-02, RF-07, RF-08, RF-15 | HU-02, HU-07, HU-08; CU-01, CU-04 |
| DL-15 | Escopo, ocupação e concorrência de vagas | RF-02, RF-05, RF-08, RF-09 | HU-02, HU-05, HU-08, HU-09; CU-01, CU-02 |
| DL-18 | Escopo do acompanhamento e gerenciamento | RF-11, RF-12 | HU-10, HU-11; CA-04 (limite) |
| DL-30 | Falhas e integridade entre inscrições, vagas e finanças | RF-08, RF-13, RF-14, RF-16 | HU-08, HU-12, HU-13; CU-01, CU-05, CU-06 |

## Análise de cobertura

- **Total de RFs:** 18.
- **RFs com História de Usuário:** 17.
- **RFs sem HU própria:** 1 — RF-15. Essa ausência é deliberada porque não há stakeholder responsável definido para sua manutenção.
- **RFs relacionados a Casos de Uso:** 10 — RF-02, RF-05, RF-06, RF-07, RF-08, RF-09, RF-13, RF-14, RF-15 e RF-16.
- **RFs sem CU:** 8 — RF-01, RF-03, RF-04, RF-10, RF-11, RF-12, RF-17 e RF-18. A cobertura de CUs foi deliberadamente seletiva.
- **RFs com Critério de Aceitação direto:** 7 — RF-01, RF-03, RF-05, RF-10, RF-13, RF-17 e RF-18.
- **RFs sem CA completo:** 11 — RF-02, RF-04, RF-06, RF-07, RF-08, RF-09, RF-11, RF-12, RF-14, RF-15 e RF-16. A ausência decorre de candidatura, informação insuficiente ou comportamento excessivamente aberto.
- **Necessidades candidatas:** 2 — RF-04 e RF-09.
- **RFs afetados por lacunas relevantes:** 18. Todos possuem pelo menos uma DL que limita algum aspecto de sua especificação, embora sete tenham comportamentos parciais suficientemente definidos para CA direto.
- **RNFs concretos:** 0.

As ausências registradas não representam esquecimento. Elas refletem a seleção deliberada dos artefatos e os limites impostos pela elicitação atual. Nenhuma lacuna foi considerada resolvida e nenhuma relação foi criada apenas por semelhança temática.
