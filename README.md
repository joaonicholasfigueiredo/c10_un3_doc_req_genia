# Engenharia de Requisitos com apoio de GenAI — Eventus

Este repositório apresenta um exercício acadêmico de análise e especificação de requisitos para uma proposta de sistema centralizado de gestão de eventos da Eventus. O trabalho foi desenvolvido com apoio de Inteligência Artificial Generativa (GenAI), cujas sugestões foram avaliadas e adaptadas durante a elaboração dos artefatos.

O conteúdo é exclusivamente documental: não há uma aplicação implementada neste repositório.

## Cenário do projeto

A Eventus organiza conferências, workshops e eventos corporativos. No cenário inicial, o gerenciamento de inscrições, vagas, pagamentos, cancelamentos e certificados utiliza formulários online e planilhas, dificultando a centralização das informações.

O exercício documenta requisitos para uma proposta de solução centralizada. Os stakeholders identificados foram Participantes, Organizadores, Equipe Financeira, Palestrantes e Equipe de TI. Esta última foi reconhecida como stakeholder, mas a elicitação não apresentou necessidades funcionais próprias suficientes para gerar funcionalidades específicas para esse perfil.

## Objetivo

O objetivo foi transformar a elicitação fornecida em documentação estruturada de Engenharia de Requisitos, relacionando necessidades, regras do domínio, incertezas e artefatos de especificação.

Adotou-se como princípio:

> Informações não fornecidas pelos stakeholders não foram completadas por suposição.

Quando uma decisão não podia ser sustentada pelas entrevistas, o ponto foi registrado como dúvida ou lacuna. RF-04, relativo ao comprovante de inscrição, e RF-09, relativo à lista de espera, permaneceram como necessidades candidatas. A elicitação também não forneceu evidências suficientes para estabelecer Requisitos Não Funcionais concretos.

## Artefatos produzidos

| Artefato | Quantidade | Documento |
| -------- | ---------: | --------- |
| Requisitos Funcionais | 18 | [Requisitos Funcionais](analise/requisitos-funcionais.md) |
| Requisitos Não Funcionais concretos | 0 | [Requisitos Não Funcionais](analise/requisitos-nao-funcionais.md) |
| Regras de Negócio | 8 | [Regras de Negócio](analise/regras-de-negocio.md) |
| Dúvidas e Lacunas | 30 | [Dúvidas e Lacunas](analise/duvidas-e-lacunas.md) |
| Histórias de Usuário | 15 | [Histórias de Usuário](especificacao/historias-de-usuario.md) |
| Casos de Uso | 6 | [Casos de Uso](especificacao/casos-de-uso.md) |
| Critérios de Aceitação | 7 | [Critérios de Aceitação](especificacao/criterios-de-aceitacao.md) |
| Matriz de Rastreabilidade | 1 | [Matriz de Rastreabilidade](especificacao/matriz-de-rastreabilidade.md) |

## Por que esses artefatos foram escolhidos

### Histórias de Usuário

Foram utilizadas para representar necessidades e objetivos sob a perspectiva dos diferentes stakeholders, mantendo vínculos com os requisitos, regras e lacunas correspondentes.

### Casos de Uso

Foram selecionados para interações em que a representação por fluxo agregava informação, como inscrição, cancelamento e confirmação de pagamento. Não houve a intenção de transformar cada requisito em um Caso de Uso. Quando o comportamento dependia de uma lacuna, o fluxo permaneceu parcialmente especificado.

### Critérios de Aceitação

Foram usados seletivamente, apenas quando contexto, ação e resultado podiam ser descritos de forma verificável. Por isso, foram produzidos 7 critérios para os 18 Requisitos Funcionais, sem criar condições ausentes na elicitação.

### Matriz de Rastreabilidade

A matriz relaciona cada Requisito Funcional à sua fonte, às Regras de Negócio, às Dúvidas e Lacunas e aos artefatos de especificação existentes. Ela também torna visíveis as ausências deliberadas de HU, CU ou CA.

Um Diagrama de Estados chegou a ser considerado, mas foi descartado porque estados e transições importantes de inscrição e pagamento ainda dependiam de informações não presentes na elicitação.

## Como a GenAI apoiou o desenvolvimento

A GenAI apoiou a organização das informações, a classificação inicial, a elaboração de propostas de requisitos, Histórias de Usuário, Casos de Uso e Critérios de Aceitação, além da construção da rastreabilidade e das revisões de consistência.

> As sugestões foram analisadas antes de serem incorporadas à documentação, principalmente quando envolviam informações não explícitas na elicitação.

Esse uso reduziu o trabalho repetitivo e facilitou comparações entre documentos, sem substituir a análise necessária para aceitar, modificar ou descartar uma proposta.

## Sugestões da GenAI aproveitadas, modificadas ou descartadas

### Aproveitadas

Entre as propostas aproveitadas estão o uso de Histórias de Usuário, Casos de Uso, Critérios de Aceitação em formato verificável e Matriz de Rastreabilidade, além da separação explícita das dúvidas e lacunas. A composição final foi definida após comparar a utilidade de cada artefato com o nível de informação disponível.

### Modificadas

**RF-04 — comprovante de inscrição.** A frase “seria interessante” não foi considerada suficiente para tornar a funcionalidade obrigatória. RF-04 permaneceu como necessidade candidata. A mesma cautela foi aplicada a RF-09, pois a lista de espera também foi apresentada como um desejo ainda sujeito a validação.

**RF-15 — eventos gratuitos e pagos.** RF-15 chegou a ser agrupado com HU-12, da Equipe Financeira. A relação foi retirada porque a elicitação não informa quem define ou mantém a modalidade financeira do evento. HU-12 permaneceu relacionada a RF-13 e RF-16, enquanto RF-15 ficou deliberadamente sem HU própria.

**Cobertura dos Critérios de Aceitação.** Em vez de criar um critério para cada requisito, foram documentados somente os comportamentos com resultado verificável. A cobertura final foi de 7 CAs para 18 RFs.

### Descartadas

**Regra sobre certificado.** Foi descartada uma interpretação que transformava a emissão posterior ao evento em proibição absoluta de emissão em qualquer outro momento. Essa restrição não estava sustentada pela elicitação.

**Diagrama de Estados.** Foi descartado nesta etapa porque estados e transições relevantes ainda dependiam de lacunas.

**Preenchimento automático das lacunas.** Não foram acrescentadas soluções como autenticação, formas específicas de pagamento, políticas de reembolso, métricas de desempenho ou regras de lista de espera quando não havia evidência suficiente.

## Estrutura do repositório

```text
.
├── analise/
│   ├── requisitos-funcionais.md
│   ├── requisitos-nao-funcionais.md
│   ├── regras-de-negocio.md
│   └── duvidas-e-lacunas.md
│
├── especificacao/
│   ├── historias-de-usuario.md
│   ├── casos-de-uso.md
│   ├── criterios-de-aceitacao.md
│   └── matriz-de-rastreabilidade.md
│
└── README.md
```

A documentação representa a especificação possível a partir da elicitação fornecida para o exercício. Os pontos que ainda dependem de informações dos stakeholders foram preservados como dúvidas e lacunas e podem orientar eventuais ciclos futuros de elicitação.
