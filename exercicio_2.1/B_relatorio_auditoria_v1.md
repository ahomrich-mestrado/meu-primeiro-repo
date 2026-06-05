# B_relatorio_auditoria_v1 — Relatório de Auditoria

**Documento auditado:** Mapeamento Analítico de Atores — Atendimento ao Seguro-Desemprego via URA (Caixa Econômica Federal)
**Total de achados:** 26
**Data da auditoria:** Junho de 2025

---

## Critérios de Escopo

A auditoria avaliou exclusivamente falhas de conteúdo:

- Erros factuais
- Lacunas de evidência
- Inferências mal-suportadas
- Atribuições incorretas
- Atores omitidos relevantes

Questões cosméticas (formatação, estilo, ordem) foram desconsideradas.

---

## 1. Erros Factuais

### EF-1 — Direção invertida do fluxo de recursos do FAT

**Trecho:** *"repassar os recursos ao Fundo de Amparo ao Trabalhador (FAT)"* (Item 10, MTE)

**Problema:** O FAT (Fundo de Amparo ao Trabalhador) já detém os recursos — alimentado por contribuições compulsórias do PIS/PASEP (Art. 239 da CF/1988). O MTE não "repassa recursos ao FAT"; o fluxo correto é o inverso: o FAT é a fonte que custeia os benefícios pagos pela Caixa. A formulação do documento inverte a relação de custódia e induz a erro sobre quem controla o caixa.

---

### EF-2 — "Empregador Web" apresentado como sistema atual de integração

**Trecho:** *"falhas de integração entre a base do MTE (Empregador Web) e a Caixa geram descompassos"* (Item 10)

**Problema:** O Empregador Web foi progressivamente substituído pelo eSocial a partir de 2018–2019. Desde então, os eventos de rescisão de contrato (que originam o requerimento do Seguro-Desemprego) transitam pelo eSocial. Apresentar o Empregador Web como o sistema vigente de integração é uma imprecisão factual temporal com impacto direto na análise de causas-raiz das falhas de integração.

---

### EF-3 — Atribuição das regras de elegibilidade diretamente ao MTE

**Trecho:** *"ditar as regras de elegibilidade"* (Item 10, atribuído integralmente ao MTE)

**Problema:** As regras de elegibilidade do Seguro-Desemprego derivam da Lei 7.998/1990 (fonte primária) e de resoluções do CODEFAT — órgão colegiado tripartite composto por representantes de trabalhadores, empregadores e governo, com poder deliberativo próprio, não subordinado a ato unilateral do MTE. Atribuir essa competência exclusivamente ao MTE ignora a natureza deliberativa colegiada da governança do FAT.

---

### EF-4 — "O dinheiro é do MTE"

**Trecho:** *"A Caixa opera o serviço, mas não é dona do dinheiro nem da política (isso é do MTE)"* (Item 9)

**Problema:** O recurso pertence ao FAT, fundo constitucional com gestão tripartite via CODEFAT. O MTE ocupa a secretaria executiva do CODEFAT e propõe políticas, mas não é proprietário do recurso. Além disso, parte dos recursos do FAT é mandatoriamente alocada ao BNDES (Art. 239 §1º CF), o que torna a simplificação "o dinheiro é do MTE" factualmente incorreta.

---

## 2. Lacunas de Evidência Críticas

> **Nota geral:** O documento não contém nenhuma citação, nota de rodapé, fonte primária ou referência a dados empíricos. As lacunas abaixo são as mais problemáticas dado o grau de assertividade das afirmações.

---

### LE-1 — "Maior causa de abandono e ódio ao serviço público automatizado"

**Trecho:** *"A falha da URA cria o efeito 'labirinto', sendo a maior causa de abandono e ódio ao serviço público automatizado."* (Item 2)

**Problema:** "Maior causa" é superlativo que exige evidência empírica — taxa de abandono, estudo de NPS, relatório de CX ou auditoria de qualidade. Nenhuma fonte é citada para este ou qualquer outro dado quantitativo do documento.

---

### LE-2 — Comportamento doloso dos atendentes

**Trecho:** *"derrubar a ligação propositalmente para bater metas de Tempo Médio de Atendimento (TMA)"* (Item 5)

**Problema:** Afirmação de comportamento intencional, não negligente. Para ser sustentada, demandaria pesquisa etnográfica, denúncias documentadas em processos trabalhistas, ou apontamento de auditoria (TCU/CGU). Apresentada como fato estabelecido sem qualquer fonte.

---

### LE-3 — Arquitetura de integração MTE-Caixa como "sincronização noturna"

**Trecho:** *"Se a sincronização noturna entre o MTE e a Caixa falha, milhares de ligações caem na URA no dia seguinte"* (seção Consolidação)

**Problema:** A arquitetura interna de integração de dados entre MTE e Caixa (tipo de processamento, janelas, protocolos) não é informação documentada publicamente. O documento descreve como fato específico algo que é especulação sobre infraestrutura não auditada.

---

### LE-4 — Viés do NLP contra sotaques regionais neste sistema específico

**Trecho:** *"O sistema pode falhar em reconhecer sotaques regionais, gírias ou fala de idosos"* (Item 3)

**Problema:** Embora o viés em ASR (Automatic Speech Recognition) seja documentado na literatura acadêmica em geral (ex.: pesquisas com Alexa, Google ASR), o documento não cita nenhum dado sobre o desempenho do motor de voz específico da URA da Caixa. A transposição acrítica de um achado geral de pesquisa para um sistema específico sem evidência é uma lacuna.

---

### LE-5 — "O medo do TCU frequentemente leva a Caixa a..."

**Trecho:** *"O medo de apontamentos do TCU frequentemente leva a Caixa a desenhar processos excessivamente rígidos ('defensivos')"* (Item 12)

**Problema:** "Frequentemente" pressupõe padrão documentado. Nenhuma auditoria do TCU, análise de processos licitatórios ou estudo de administração pública é citado. É uma afirmação plausível no campo da teoria organizacional pública, mas totalmente não-fundamentada.

---

### LE-6 — "Alta vulnerabilidade emocional" como dado da jornada

**Trecho:** *"Alta vulnerabilidade emocional colidindo com a rigidez de um sistema parametrizado"* (Item 1)

**Problema:** A vulnerabilidade do requerente pode ser real, mas é apresentada como achado analítico sem referência a pesquisas de campo, estudos de UX, pesquisas de satisfação (CSAT, CES) ou dados do Ouvidor da Caixa.

---

### LE-7 — Ausência total de dados quantitativos de contexto

**Trecho:** Documento inteiro.

**Problema:** O documento não cita: volume de ligações anuais ao 0800 726 0207, taxa de abandono, taxa de contenção da URA, tempo médio de espera, índice de resolução no primeiro contato, nem qualquer métrica de desempenho do serviço. Esses dados são essenciais para dimensionar os problemas descritos e existem em relatórios públicos do TCU e do DIEESE.

---

## 3. Inferências Mal-Suportadas

### IMS-1 — ACD configurado para penalizar casos complexos

**Trecho:** *"O sistema pode estar configurado para priorizar perfis de chamadas que dão menos trabalho, prejudicando os casos complexos"* (Item 4)

**Problema:** O "pode estar" convive com "Priorização invisível" como título da seção, que afirma o fenômeno como real. O documento pega uma funcionalidade genérica e teórica de sistemas ACD (skill-based routing para gestão de filas) e a projeta como disfunção intencional deste serviço específico sem nenhuma evidência de que o ACD da Caixa/terceirizada está assim configurado.

---

### IMS-2 — A URA é desenhada para "reduzir custos", não para "resolver o problema"

**Trecho:** *"A URA é frequentemente desenhada com o objetivo de 'reduzir custos de call center' (contenção) em vez de 'resolver o problema do cidadão' (resolutividade)"* (Item 2)

**Problema:** Em serviços públicos federais, os condicionantes de design de URA incluem especificações técnicas de licitação, frameworks de governança de TI (e-PING, e-MAG), TCU e CGU — uma cadeia de incentivos estruturalmente diferente da URA corporativa privada. Generalizar a lógica de "contenção de custo corporativo" para este contexto sem análise dos contratos e editais é uma inferência não-suportada.

---

### IMS-3 — A "Hipótese da Falsa Contenção" contamina a análise antes de ser validada

**Trecho:** *"Suspeito que o alto índice de 'resolução' na URA (contenção) não seja resolução real"* (seção Lacunas)

**Problema:** Embora honestamente rotulada como hipótese, o raciocínio desta hipótese já estava pressuposto em diversas partes anteriores do documento (ex.: "vai engrossar as filas das agências físicas", "frustração processual de ponta a ponta"). A hipótese não testada está funcionando como premissa de análise.

---

### IMS-4 — Metáfora "Teto de Vidro da UX" semanticamente incorreta

**Trecho:** *"Hipótese do Teto de Vidro da UX: O viés algorítmico do reconhecimento de voz pune regiões específicas do Brasil?"* (seção Lacunas)

**Problema:** "Teto de vidro" (glass ceiling) refere-se a barreiras invisíveis de progressão/ascensão, não de acesso inicial. O fenômeno descrito — impossibilidade de entrar no sistema — é uma barreira de acesso, adequadamente descrita por termos como "barreira sistêmica" ou "muro de exclusão digital". O erro conceitual compromete a precisão analítica do texto.

---

### IMS-5 — "Não há Owner único" afirmado sem verificação estrutural

**Trecho:** *"Não há um Owner único de ponta a ponta olhando para o First Contact Resolution (Resolução no Primeiro Contato) do cidadão."* (seção Consolidação)

**Problema:** Esta é uma afirmação sobre estrutura de governança que poderia ser verificada por organograma, contrato de terceirização, portaria ministerial ou matriz de responsabilidade. O documento a apresenta como conclusão evidente sem demonstrar que investigou se tal papel existe ou não formalmente.

---

## 4. Atribuições Incorretas

### AI-1 — Terminologia SLI/SLA

**Trecho:** *"SLAs contratuais (que medem tempo no ar) vs. SLIs de negócio (que medem resolutividade real)"* (Item 8)

**Problema:** SLI (Service Level Indicator) é uma métrica de medição (ex.: latência em ms), enquanto SLA (Service Level Agreement) é o compromisso contratual e SLO (Service Level Objective) é a meta interna. O contraste correto seria entre SLAs focados em disponibilidade vs. SLAs/SLOs focados em resolutividade. O uso de "SLI" em oposição a "SLA" confunde os termos da disciplina de SRE/gestão de serviços.

---

### AI-2 — Frontstage/Backstage sem atribuição teórica

**Trecho:** *"Podemos agrupar os atores acima em quatro camadas concêntricas de serviço: Frontstage (O Visível)... Backstage Operacional..."* (seção Consolidação)

**Problema:** A terminologia "frontstage/backstage" em serviços é diretamente derivada do Service Blueprinting (G. Lynn Shostack, 1984, Harvard Business Review) e da sociologia dramatúrgica de Goffman. O documento usa o framework como se fosse estrutura analítica original, sem qualquer atribuição. Em texto analítico, essa omissão é intelectualmente relevante.

---

## 5. Atores Omitidos Relevantes

### AO-1 — CODEFAT (Conselho Deliberativo do Fundo de Amparo ao Trabalhador)

**Impacto:** Completamente ausente. O CODEFAT é o órgão de governança máxima do FAT — 18 membros tripartites (trabalhadores, empregadores, governo) —, responsável por resoluções que definem critérios de elegibilidade, valores e operação do Seguro-Desemprego. É mais relevante para "as regras do jogo" do que o MTE isoladamente, e sua omissão distorce toda a análise de poder no macroambiente.

---

### AO-2 — Empregadores / Empresas (iniciadores formais do processo)

**Impacto:** O empregador é o ator que inicia a cadeia: a rescisão comunicada via eSocial gera o registro que a URA da Caixa vai consultar. Falhas do lado do empregador (comunicação de rescisão incorreta, atraso, divergência de dados) são causa-raiz de uma classe inteira de erros que a URA reporta como "benefício não localizado". O documento os menciona apenas de passagem ("processamento prévio de seus dados pelo empregador") sem incluí-los como ator formal.

---

### AO-3 — SRTEs (Superintendências Regionais do Trabalho e Emprego) e Postos SINE

**Impacto:** O documento menciona "agências físicas" como destino genérico do overflow da URA, mas não identifica as SRTEs (ex-Delegacias Regionais do Trabalho) e os Postos do SINE como atores formais. O SINE é obrigatório em algumas modalidades e é o destino físico real da frustração gerada pela URA. A omissão é estrutural para o mapeamento.

---

### AO-4 — Canal Digital Gov.br / CTPS Digital

**Impacto:** O ecossistema de requerimento do Seguro-Desemprego foi parcialmente migrado para o portal gov.br e para a Carteira de Trabalho Digital (CTPS Digital), que já permite o requerimento online. Mapear apenas a URA como ponto de contato é analisar um ecossistema multicanal como se fosse monocanal, ignorando um canal que desloca demanda da própria URA.

---

### AO-5 — Poder Judiciário / Defensoria Pública da União (DPU)

**Impacto:** Em casos de negativa de benefício, o Juizado Especial Federal (JEF) e a DPU são acionados. Esses atores são relevantes no mapa de ponta a ponta — especialmente na análise de "falhas sistêmicas na concessão" — e sua ausência torna o mapeamento incompleto para ciclos de falha escalados.

---

### AO-6 — Modalidades especiais de beneficiários (pescadores artesanais, domésticas, resgatados)

**Impacto:** A partir da Lei 13.134/2015, o Seguro-Desemprego cobre pescadores artesanais, empregadas domésticas e trabalhadores resgatados de condição análoga à escravidão. Cada modalidade tem fluxos distintos na URA. Tratar o "Cidadão Requerente" como categoria monolítica apaga diferenças sistêmicas de atendimento que são centrais para uma análise de exclusão e vulnerabilidade como a proposta.

---

## 6. Síntese e Veredito

| Categoria | Achados | Severidade |
|---|:---:|---|
| Erros factuais | 4 | Crítico — invalida análise |
| Lacunas de evidência | 7 | Alto — enfraquece conclusões |
| Inferências mal-suportadas | 5 | Alto — enfraquece conclusões |
| Atribuições incorretas | 2 | Médio — imprecisão corrigível |
| Atores omitidos relevantes | 6 | Crítico — invalida mapa de atores |
| Fontes citadas (doc. inteiro) | 0 | Crítico — zero fontes |
| **Total de achados** | **26** | |

### Três problemas sistêmicos

**Problema 1 — Zero fontes em 100% das afirmações.**
Nenhuma afirmação quantitativa, institucional ou comportamental tem fonte citada. O documento transita entre hipótese, análise e conclusão sem sinalizar as fronteiras, tornando impossível separar o que é dado do que é opinião.

**Problema 2 — Dois erros factuais de base (EF-1 e EF-3).**
Os erros sobre o FAT e o CODEFAT invalidam diretamente a análise do macroambiente de governança — a camada que o próprio texto considera mais determinante para a qualidade do serviço.

**Problema 3 — Seis atores omitidos distorcem o mapa de poder.**
Especialmente o CODEFAT (governança real do FAT), os empregadores (iniciadores formais da cadeia) e o canal gov.br/CTPS Digital (canal que desloca demanda da URA). O fluxo real começa na rescisão comunicada pelo empregador, não na ligação do cidadão — essa omissão é estrutural.

---

*Auditoria conduzida por IA generativa. Recomenda-se validação por especialista em política pública de trabalho e emprego para os achados EF-1 a EF-4.*
