# B_relatorio_auditoria_v2 — Relatório de Auditoria (Segunda Rodada)

**Documento auditado:** Dossiê v2 — Ecossistema e Jornada do Usuário no Atendimento ao Seguro-Desemprego via URA Caixa
**Referência:** audit_v1 (26 achados originais)
**Data da auditoria:** Junho de 2025

---

## Critérios de Verificação

Esta auditoria avaliou três dimensões:

- (a) Se cada achado de audit_v1 foi de fato endereçado na v2
- (b) Se a v2 introduziu falhas novas
- (c) Se restam pontos abertos

---

## Parte A — Rastreamento dos 26 Achados de audit_v1

### Achados corrigidos de forma satisfatória (18 de 26)

Os achados abaixo foram resolvidos sem ressalva relevante: **EF-1, EF-2, EF-3, EF-4, LE-1, LE-4, LE-5, LE-7, IMS-2, IMS-3, IMS-4, IMS-5, AO-1, AO-2, AO-3, AO-4, AO-5, AO-6**.

Destaques positivos:

- O FAT é agora corretamente descrito como custódia financeira originária (Art. 239 CF), e a Caixa como agente pagador — invertendo o erro factual de EF-1.
- O eSocial substituiu o Empregador Web como sistema de integração vigente (EF-2).
- O CODEFAT foi integrado como órgão deliberativo tripartite com competência própria sobre as regras de elegibilidade (EF-3, AO-1).
- Todos os seis atores omitidos (AO-1 a AO-6) foram incorporados ao mapa: CODEFAT, Empregadores, SRTEs/SINE, Gov.br/CTPS Digital, DPU/JEF e modalidades especiais de beneficiários.
- As hipóteses comportamentais (IMS-3, IMS-4, IMS-5) foram corretamente demarcadas como pendentes de validação empírica.

---

### Achados parcialmente corrigidos (6 de 26)

---

#### LE-2 — Parcialmente resolvido ⚠

**Trecho:** *"induzindo atendentes terceirizados à prática negligente de encerrar prematuramente ligações complexas"* (H4)

**Situação:** A matriz de resolução afirma ter remanejado o comportamento doloso para hipótese a ser validada por pesquisa etnográfica. O texto melhorou: saiu de "derrubar a ligação propositalmente" (intencional/doloso) para "prática negligente" (estrutural/induzida). Contudo, a hipótese H4 ainda caracteriza um comportamento específico — desta vez como negligência — sem qualquer fonte. A mudança de dolo para culpa não elimina a necessidade de evidência empírica; apenas muda o qualificador da afirmação não-fundamentada.

---

#### LE-3 — Parcialmente resolvido ⚠

**Trecho:** *"Falhas de comunicação em massa reportadas pela URA exigem análise da engenharia e dos tempos de processamento/lotes entre esses sistemas."* (H3)

**Situação:** H3 foi bem estruturada como hipótese arquitetural. O problema: a expressão "falhas de comunicação em massa reportadas pela URA" trata o fenômeno como premissa estabelecida — exatamente o ponto que audit_v1 sinalizou em LE-3. A hipótese deveria questionar *se* tais falhas em massa ocorrem, não partir delas como dadas. A premissa que deveria ser testada voltou embutida no enunciado da hipótese que a testaria.

---

#### LE-6 — Parcialmente resolvido ⚠

**Trecho (Parte 1):** *"a mensuração do impacto emocional na jornada da URA foi devidamente remarcada como pendente de dados de Customer Effort Score (CES)"*

**Trecho (Parte 2, Seção 4.A):** lista FCR; CES ausente.

**Situação:** Há uma discrepância interna entre o que a Parte 1 (Matriz de Resolução) afirma ter feito e o que a Parte 2 (Dossiê) entrega. O CES — que a própria matriz prometeu incluir como métrica pendente — está ausente da Seção 4.A. A defesa da vulnerabilidade econômica (verba alimentar, desemprego involuntário) é válida e defensável como premissa da política pública. O problema é que a promessa de remarcação via CES não foi executada no texto do dossiê.

---

#### IMS-1 — Parcialmente resolvido ⚠

**Situação:** A inferência sobre o ACD/CTI priorizar chamadas fáceis foi movida para as hipóteses. Porém, a solução adotada foi remover o ator inteiro: o Sistema de Roteamento de Chamadas (ACD/CTI), que era o Item 4 legítimo da v1, desapareceu do mapa da v2. O correto seria separar o ator (que existe e opera na arquitetura do serviço) da inferência infundada sobre sua configuração específica (que deve permanecer como hipótese). Ao remover o ator, a v2 perdeu um componente operacional real da arquitetura do serviço.

---

#### AI-1 — Parcialmente resolvido ⚠

**Trecho:** *"SLAs/SLOs de resolutividade"* (Seção 4.A)

**Situação:** A introdução de SLO é um avanço sobre a confusão original com SLI. Mas a formulação "SLAs/SLOs" usada como par solidário ainda obscurece a distinção: SLA (Service Level Agreement) é o compromisso contratual; SLO (Service Level Objective) é a meta operacional interna. Eles não são intercambiáveis e não deveriam ser listados como sinônimos. Melhoria real, porém incompleta.

---

#### AI-2 — Parcialmente resolvido ⚠

**Trecho:** *"Service Blueprinting (Shostack, 1984)"* (Seção 1)

**Situação:** A atribuição a Shostack foi inserida, cumprindo o essencial. Duas deficiências permanecem:

1. A citação está em formato informal (apenas autor e ano), sem título do artigo — "Designing Services That Deliver", HBR, jan.–fev. 1984 — nem periódico, tornando-a irrastreável para fins acadêmicos.
2. O audit_v1 apontou a origem dual na sociologia dramatúrgica de Goffman (1959, *The Presentation of Self in Everyday Life*), que permanece sem reconhecimento.

---

## Parte B — Falhas Novas Introduzidas na v2

### NF-1 — Dataprev introduzido como "ator fantasma"

**Trecho:** *"do processamento desse evento pelo Dataprev/MTE"* (Seção 3, parágrafo final)

**Problema:** A Dataprev (Empresa de Tecnologia e Informações da Previdência Social) aparece na conclusão do dossiê como processador crítico dos eventos do eSocial que alimentam o MTE — sem nunca ter sido mapeada como ator formal. Se a Dataprev é relevante o suficiente para constar na análise de dependências críticas, ela pertence ao mapa de atores com Papel, Riscos e Dependências. A menção isolada em parágrafo conclusivo é estruturalmente inconsistente.

---

### NF-2 — "TTS" usado como abreviatura indevida para autoatendimento

**Trecho:** *"Triagem e contenção via autoatendimento (TTS)"* (Seção 2.3.I)

**Problema:** No ecossistema de telefonia e URA, TTS designa especificamente Text-to-Speech — a tecnologia de síntese de voz que converte texto em áudio para o usuário ouvir. É uma tecnologia de *saída*, não um sinônimo de autoatendimento. Usar "(TTS)" como parentético explicativo de "autoatendimento" é tecnicamente incorreto e cria ambiguidade com o item J, que descreve ASR/NLP como tecnologia de *entrada*. A separação lógica entre tecnologia de entrada (ASR) e de saída (TTS) — que era um ponto correto da v1 — fica comprometida.

---

### NF-3 — Regressão estrutural: quatro atores legítimos da v1 removidos sem justificativa

**Problema:** A v2 suprimiu quatro atores que estavam corretamente mapeados na v1 e que não foram sinalizados como problemáticos pelo audit_v1:

| Ator removido | Item na v1 | Contribuição perdida |
|---|---|---|
| Supervisores e Gestores da Central | Item 6 | Análise da tensão entre métricas e qualidade |
| Equipe de Suporte Tecnológico (TI) | Item 7 | Responsabilidade por incidentes de lentidão/queda |
| Fornecedores de Infraestrutura e Software | Item 8 | Risco de indisponibilidade nacional (telecom/cloud) |
| Segurança da Informação e LGPD | Item 11 | Fricção de autenticação como mecanismo de exclusão |

O ator de Segurança da Informação era especialmente crítico: era o único lugar do documento que explicava por que usuários legítimos são bloqueados pelo funil de autenticação da URA — análise que desapareceu sem substituto na v2. Adicionalmente, o ACD/CTI (v1 Item 4) foi removido como consequência de IMS-1 (ver Parte A). A v2 ganhou seis atores novos mas perdeu cinco legítimos do backstage operacional. O balanço é regressivo nessa camada.

---

### NF-4 — "Migram compulsoriamente" para a URA sem fonte

**Trecho:** *"Usuários que não conseguem validação biométrica no Gov.br migram compulsoriamente para a URA ou canais físicos."* (Seção 2.2.F)

**Problema:** "Compulsoriamente" é uma afirmação causal forte que pressupõe: (a) a falha biométrica no Gov.br ocorre com frequência significativa; (b) o único caminho de overflow é a URA ou a rede física; (c) não existem outros mecanismos de recuperação de acesso no ecossistema digital. Nenhum desses três pressupostos é documentado. Reproduz o padrão sistematicamente apontado no audit_v1: afirmação operacional específica apresentada como fato estabelecido sem fonte.

---

### NF-5 — Seguro Defeso conflacionado com modalidade de Seguro-Desemprego

**Trecho:** *"pescadores artesanais (Seguro Defeso)"* (Seção 2.3.H)

**Problema:** O Seguro Defeso é regido pela Lei 10.779/2003, possui critérios de elegibilidade próprios (vedação temporária da pesca por decreto), calendário sazonal e documentação específica (licença de pesca, declaração da colônia). Embora o MTE o administre e ele apareça em algumas comunicações oficiais sob o guarda-chuva do Programa Seguro-Desemprego, suas árvores de URA, bases legais e fluxos de atendimento são substancialmente distintos do Seguro-Desemprego CLT padrão. A v2 propõe corrigir a monoliticidade do Cidadão Requerente (AO-6 do audit_v1), mas cria uma nova imprecisão ao colocar o Seguro Defeso como mero parentético de uma modalidade, como se fosse uma variante nomenclatural.

---

### NF-6 — Inconsistência interna: Parte 1 afirma correção que Parte 2 não executa

**Trecho Parte 1:** *"a mensuração do impacto emocional na jornada da URA foi devidamente remarcada como pendente de dados de Customer Effort Score (CES)"*

**Trecho Parte 2, Seção 4.A:** CES ausente; apenas FCR listado.

**Problema:** A Matriz de Resolução (Parte 1) e o Dossiê (Parte 2) se contradizem. A matriz atesta uma correção que o dossiê não executa. Em auditoria formal, esse tipo de divergência entre sumário executivo e corpo do documento invalida a afirmação da correção — é o mesmo padrão de "compliance defensivo" que o próprio texto critica nos processos da Caixa e do TCU.

---

## Parte C — Pontos Remanescentes

### PR-1 — Análise de Poder e Dependência não reconstruída para o novo mapa

A v1 continha uma seção de "Análise de Poder, Influência e Dependência" que era analiticamente densa: mapeava quem detém mandato (MTE/CODEFAT), quem detém execução (Caixa) e quem absorve toda a frustração (Atendente e Cidadão). Com seis novos atores integrados na v2, essa análise precisaria ser reconstruída para o mapa ampliado. A v2 entrega mais atores, mas não entrega análise sistêmica sobre as relações de poder entre eles.

### PR-2 — Autenticação/exclusão digital sem cobertura analítica

Com a remoção do ator Segurança da Informação/LGPD (NF-3), a análise da fricção de autenticação como mecanismo de exclusão de usuários legítimos desapareceu do documento sem substituto. É uma lacuna explicativa real: a v2 discute acessibilidade para modalidades especiais (pescadores, domésticas), mas não discute a barreira da autenticação que afeta todas as modalidades.

### PR-3 — Padronização de idioma pendente

A hipótese H5 usa "ownership" em inglês sem tradução. A Seção 4.A usa "FCR" sem explicitá-lo. O audit_v1 havia sinalizado o mesmo padrão nos termos "Owner" e "First Contact Resolution" da v1. A padronização de idioma no texto analítico permanece pendente de revisão sistemática.

---

## Síntese e Veredito

| Dimensão | Resultado |
|---|---|
| Achados v1 corrigidos | 18 de 26 (69%) |
| Achados v1 parcialmente corrigidos | 6 de 26 (23%) |
| Achados v1 não corrigidos | 0 de 26 (0%) |
| Falhas novas introduzidas | 6 (NF-1 a NF-6) |
| Pontos remanescentes | 3 (PR-1 a PR-3) |

A v2 resolve dois terços dos problemas sinalizados no audit_v1 e melhora estruturalmente o documento em aspectos críticos: a governança do FAT/CODEFAT, os empregadores como iniciadores da cadeia e os canais digitais foram corretamente integrados. As hipóteses comportamentais foram devidamente demarcadas.

Dois problemas exigem atenção prioritária na v3:

**Regressão de atores (NF-3):** A v2 ganhou seis atores novos mas perdeu cinco legítimos do backstage operacional. O saldo de cobertura é negativo nessa camada, e a perda do ator de Segurança da Informação/LGPD cria uma lacuna analítica real sobre os mecanismos de exclusão por autenticação.

**Inconsistência interna Parte 1 × Parte 2 (NF-6 + LE-6):** Quando uma matriz de resolução atesta correções que o dossiê não executa, o documento se autoavalia melhor do que efetivamente é — reproduzindo o padrão de compliance defensivo que o próprio texto critica nos órgãos de controle.

---

*Auditoria conduzida por IA generativa. Recomenda-se validação por especialista em política pública de trabalho e emprego para os achados factuais (NF-5, LE-3 residual).*
