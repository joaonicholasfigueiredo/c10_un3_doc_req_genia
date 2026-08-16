# Dúvidas, ambiguidades, inconsistências e lacunas

## DL-01 — Significado de evento disponível

**Tipo:**  
Ambiguidade

**Contexto:**  
O participante deseja visualizar “todos os eventos disponíveis”, sem definição do que torna um evento disponível nem dos dados apresentados.

**Questão para o stakeholder:**  
Quais eventos devem aparecer como disponíveis e quais informações devem ser exibidas nessa consulta?

**Impacto:**  
Define o escopo e os critérios da consulta prevista em RF-01.

## DL-02 — Fluxo e dados da inscrição

**Tipo:**  
Lacuna

**Contexto:**  
A inscrição é um interesse explícito dos participantes, mas não foram descritos os dados solicitados, etapas, pré-requisitos ou forma de identificação do participante.

**Questão para o stakeholder:**  
Quais dados, etapas e pré-requisitos compõem uma inscrição em evento ou workshop?

**Impacto:**  
Impede detalhar e validar o comportamento de RF-02.

## DL-03 — Acompanhamento da inscrição

**Tipo:**  
Lacuna

**Contexto:**  
O participante deseja acompanhar inscrições, mas não foram definidos estados nem informações de acompanhamento.

**Questão para o stakeholder:**  
Quais estados e informações de uma inscrição o participante deve poder consultar?

**Impacto:**  
Define o conteúdo e as transições relevantes para RF-03 e para o controle financeiro.

## DL-04 — Comprovantes e notificações

**Tipo:**  
Lacuna

**Contexto:**  
É desejado um comprovante logo após a inscrição, mas não foram informados conteúdo, formato, canal de envio nem outras notificações necessárias.

**Questão para o stakeholder:**  
Quais comprovantes e notificações devem existir, com qual conteúdo, em que momento e por quais canais devem ser disponibilizados ou enviados?

**Impacto:**  
Afeta RF-04 e pode originar outras funcionalidades somente após a definição das notificações requeridas.

## DL-05 — Prazo para cancelamento

**Tipo:**  
Lacuna

**Contexto:**  
Não foi definido até quando o participante poderá cancelar a inscrição.

**Questão para o stakeholder:**  
Qual é o prazo limite para cancelamento e ele varia por evento ou por tipo de inscrição?

**Impacto:**  
Determina quando RF-05 pode ser executado e pode afetar vagas, lista de espera e reembolso.

## DL-06 — Configuração e demais condições de cancelamento

**Tipo:**  
Lacuna

**Contexto:**  
Nem todos os eventos permitem cancelamento, mas não foi informado quem define essa permissão nem se existem outras condições.

**Questão para o stakeholder:**  
Quem define se um evento permite cancelamento e quais condições, além do prazo, devem ser avaliadas?

**Impacto:**  
Afeta RF-05, RF-07 e a aplicação de RN-02.

## DL-07 — Critérios para reembolso

**Tipo:**  
Lacuna

**Contexto:**  
A elicitação afirma que há casos com e sem direito a reembolso, mas não especifica os critérios.

**Questão para o stakeholder:**  
Em quais situações o participante tem direito a reembolso e como o valor a reembolsar deve ser determinado?

**Impacto:**  
Afeta RF-05, RF-14 e a aplicação de RN-05.

## DL-08 — Funcionamento da lista de espera

**Tipo:**  
Lacuna

**Contexto:**  
Não foi informado como funcionará a lista de espera quando o evento lotar.

**Questão para o stakeholder:**  
Como participantes entram, são ordenados, promovidos, notificados e removidos da lista de espera, e qual prazo têm para aceitar uma vaga?

**Impacto:**  
Afeta RF-08, RF-09 e RN-04.

## DL-09 — Elegibilidade e geração de certificados

**Tipo:**  
Lacuna

**Contexto:**  
Não foi definido se o certificado será disponibilizado automaticamente depois do evento ou se dependerá da confirmação de presença; tampouco foram definidos outros critérios.

**Questão para o stakeholder:**  
Quais critérios tornam um participante elegível ao certificado, como a presença será confirmada e como o certificado será gerado e disponibilizado?

**Impacto:**  
Afeta RF-06 e a aplicação de RN-07, podendo exigir uma funcionalidade de registro de presença que ainda não tem respaldo suficiente para ser especificada.

## DL-10 — Momento da reserva da vaga em inscrição paga

**Tipo:**  
Lacuna

**Contexto:**  
Não foi definido se a vaga é reservada quando o participante inicia o pagamento ou somente após a confirmação.

**Questão para o stakeholder:**  
Em que momento uma inscrição paga ocupa uma vaga e o que ocorre com a vaga se o pagamento não for confirmado?

**Impacto:**  
Afeta RF-08, RF-13, RF-16, RN-03 e RN-06, especialmente em eventos próximos da lotação.

## DL-11 — Inscrições condicionadas a pagamento

**Tipo:**  
Ambiguidade

**Contexto:**  
A equipe financeira precisa confirmar pagamentos antes de liberar “determinadas inscrições”, mas a abrangência e o significado de “liberar” não foram explicados.

**Questão para o stakeholder:**  
Quais inscrições dependem de confirmação de pagamento e o que significa liberá-las: confirmar a inscrição, permitir acesso ao evento ou outra ação?

**Impacto:**  
Afeta RF-03, RF-13, RF-16 e RN-06.

## DL-12 — Inscrições em atividades com conflito de horário

**Tipo:**  
Lacuna

**Contexto:**  
O participante deseja inscrever-se em vários workshops no mesmo dia, e workshops no mesmo horário podem ocorrer simultaneamente. Isso não é necessariamente contraditório, mas não foi definida a política para conflitos.

**Questão para o stakeholder:**  
O participante pode inscrever-se em atividades com sobreposição de horário; em caso negativo, o sistema deve impedir ou apenas alertar?

**Impacto:**  
Afeta RF-02, a programação e a aplicação de RN-08.

## DL-13 — Relação entre evento, workshop e atividade

**Tipo:**  
Ambiguidade

**Contexto:**  
O documento alterna os termos “evento”, “workshop” e “atividade”, sem explicar sua estrutura ou relação.

**Questão para o stakeholder:**  
Como eventos, workshops e atividades se relacionam, e em qual desses níveis ocorrem inscrição, pagamento, capacidade, cancelamento e certificado?

**Impacto:**  
Afeta a interpretação da maior parte dos requisitos funcionais e regras de negócio.

## DL-14 — Dados e ciclo de vida do evento

**Tipo:**  
Lacuna

**Contexto:**  
Organizadores desejam criar eventos, mas seus campos, estados e operações posteriores não foram descritos.

**Questão para o stakeholder:**  
Quais informações são obrigatórias para criar um evento e quais estados e alterações posteriores precisam ser suportados?

**Impacto:**  
Afeta RF-07 e a configuração de vagas, pagamento, cancelamento, programação e certificados.

## DL-15 — Escopo e concorrência do controle de vagas

**Tipo:**  
Lacuna

**Contexto:**  
Foi solicitado controle automático de vagas, mas não foi definido o nível da capacidade, como vagas são liberadas nem como tratar inscrições simultâneas para a última vaga.

**Questão para o stakeholder:**  
A capacidade é definida por evento ou atividade, quais ações ocupam e liberam vagas e qual resultado é esperado quando inscrições simultâneas disputam as últimas vagas?

**Impacto:**  
Afeta RF-08, RF-09, RN-03 e a integridade do número de vagas.

## DL-16 — Obrigatoriedade da lista de espera

**Tipo:**  
Dúvida

**Contexto:**  
O organizador descreveu a lista de espera como algo que “seria interessante”, sem indicar se é obrigatória ou apenas uma possibilidade.

**Questão para o stakeholder:**  
A lista de espera faz parte do escopo obrigatório e deve existir para todos os eventos lotados ou ser configurável por evento?

**Impacto:**  
Determina a obrigatoriedade e abrangência de RF-09 e RN-04.

## DL-17 — Significado de acompanhamento em tempo real

**Tipo:**  
Ambiguidade

**Contexto:**  
Os organizadores desejam acompanhar inscritos “em tempo real”, sem uma frequência de atualização ou latência definida.

**Questão para o stakeholder:**  
Qual atraso máximo entre uma alteração de inscrição e sua exibição ao organizador é aceitável, e a atualização deve ser automática?

**Impacto:**  
Afeta a verificabilidade de RF-10 e a eventual definição de um requisito não funcional de desempenho.

## DL-18 — Escopo do gerenciamento de participantes

**Tipo:**  
Ambiguidade

**Contexto:**  
“Gerenciar participantes” aparece como interesse do organizador, mas nenhuma operação foi detalhada.

**Questão para o stakeholder:**  
Quais operações o organizador deve poder realizar sobre participantes e inscrições?

**Impacto:**  
Afeta o detalhamento de RF-11 e impede decompor e verificar RF-12 sem inventar capacidades.

## DL-19 — Processo de confirmação de pagamento

**Tipo:**  
Lacuna

**Contexto:**  
A equipe financeira precisa confirmar pagamentos, mas não foi definido de onde vem a informação nem quais estados e exceções existem.

**Questão para o stakeholder:**  
A confirmação será registrada manualmente ou recebida de outro serviço, e quais estados, falhas e correções de pagamento devem ser tratados?

**Impacto:**  
Afeta RF-13, RF-16, o acompanhamento da inscrição e o controle de vagas.

## DL-20 — Alcance do controle de reembolsos

**Tipo:**  
Ambiguidade

**Contexto:**  
“Controlar reembolsos” pode significar registrar, aprovar, acompanhar ou efetuar a devolução financeira, mas o documento não esclarece o alcance.

**Questão para o stakeholder:**  
Quais operações de reembolso o sistema deverá oferecer e a devolução financeira será executada pelo sistema ou apenas registrada e acompanhada nele?

**Impacto:**  
Define o comportamento verificável de RF-14 e possíveis integrações ainda não especificadas.

## DL-21 — Cobrança dos eventos pagos

**Tipo:**  
Lacuna

**Contexto:**  
Há eventos pagos, mas não foram definidos preços, formas de pagamento, prazos, processamento ou integrações.

**Questão para o stakeholder:**  
Como são definidos e cobrados os valores dos eventos pagos, quais formas e prazos de pagamento são aceitos e o sistema deverá processar o pagamento ou apenas registrar sua situação?

**Impacto:**  
Afeta RF-13, RF-15, RF-16 e o alcance do sistema financeiro.

## DL-22 — Conteúdo e escopo da programação para palestrantes

**Tipo:**  
Lacuna

**Contexto:**  
Palestrantes desejam consultar a programação, mas não foi definido se verão toda a programação ou apenas suas atividades, nem quais detalhes serão exibidos.

**Questão para o stakeholder:**  
Qual parte da programação o palestrante poderá consultar e quais informações deverão ser apresentadas?

**Impacto:**  
Afeta o escopo e o controle de acesso de RF-17.

## DL-23 — Dados de participantes visíveis aos palestrantes

**Tipo:**  
Lacuna

**Contexto:**  
Não foi definido quais informações dos participantes poderão ser visualizadas pelos palestrantes.

**Questão para o stakeholder:**  
Quais campos de cada participante o palestrante poderá visualizar e para qual finalidade?

**Impacto:**  
Afeta RF-18, RN-09, privacidade e autorização de acesso.

## DL-24 — Segurança e controle de acesso

**Tipo:**  
Lacuna

**Contexto:**  
Não foram levantados requisitos de segurança, embora existam diferentes perfis com capacidades e dados distintos.

**Questão para o stakeholder:**  
Quais requisitos de autenticação, autorização por perfil, auditoria e proteção contra incidentes devem ser atendidos?

**Impacto:**  
Impossibilita estabelecer requisitos verificáveis de segurança e delimitar com precisão o acesso de cada stakeholder.

## DL-25 — Desempenho e volume de uso

**Tipo:**  
Lacuna

**Contexto:**  
Não foram levantados requisitos de desempenho nem estimativas de volume de eventos, participantes ou acessos simultâneos.

**Questão para o stakeholder:**  
Quais volumes e picos de uso são esperados e quais tempos de resposta são aceitáveis para as operações principais?

**Impacto:**  
Impede definir e verificar requisitos de desempenho e capacidade.

## DL-26 — Disponibilidade e recuperação

**Tipo:**  
Lacuna

**Contexto:**  
Não foram levantados requisitos de disponibilidade.

**Questão para o stakeholder:**  
Em quais períodos o sistema deve estar disponível, qual indisponibilidade é aceitável e quais objetivos de recuperação são necessários?

**Impacto:**  
Impede definir requisitos verificáveis de disponibilidade e continuidade.

## DL-27 — Acessibilidade

**Tipo:**  
Lacuna

**Contexto:**  
Não foram levantados requisitos de acessibilidade.

**Questão para o stakeholder:**  
Quais necessidades do público e quais padrões ou níveis de conformidade de acessibilidade devem ser atendidos?

**Impacto:**  
Impede definir critérios verificáveis de acessibilidade e pode excluir participantes se permanecer sem decisão.

## DL-28 — Privacidade e tratamento de dados pessoais

**Tipo:**  
Lacuna

**Contexto:**  
Não foram levantados requisitos de privacidade, embora dados de participantes sejam tratados e parcialmente acessados por organizadores, equipe financeira e palestrantes.

**Questão para o stakeholder:**  
Quais dados pessoais serão tratados, para quais finalidades, por quanto tempo, com quais compartilhamentos e restrições, e quais obrigações de privacidade devem ser atendidas?

**Impacto:**  
Impede definir requisitos verificáveis de privacidade, retenção e acesso a dados.

## DL-29 — Objetivo de melhor experiência

**Tipo:**  
Ambiguidade

**Contexto:**  
O contexto do projeto menciona “uma melhor experiência aos participantes”, sem indicar aspectos ou critérios observáveis.

**Questão para o stakeholder:**  
Quais aspectos da experiência devem melhorar e como o sucesso dessa melhoria será avaliado?

**Impacto:**  
A afirmação não pode ser transformada em requisito não funcional verificável enquanto permanecer vaga.

## DL-30 — Tratamento de falhas e integridade

**Tipo:**  
Lacuna

**Contexto:**  
O controle centralizado envolve vagas, pagamentos, cancelamentos e reembolsos, mas não foram descritos comportamentos diante de falhas ou divergências entre essas operações.

**Questão para o stakeholder:**  
Como o sistema deve preservar e reconciliar as informações de inscrição, vaga e pagamento quando uma operação falhar ou houver dados divergentes?

**Impacto:**  
Impede definir requisitos verificáveis de confiabilidade e integridade operacional.
