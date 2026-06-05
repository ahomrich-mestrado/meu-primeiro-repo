# Resolução da Auditoria e Dossiê de Pesquisa (V2)

## PARTE 1: MATRIZ DE RESOLUÇÃO DA AUDITORIA

**1. Erros Factuais**
* **EF-1 (Direção do FAT):** *(a) Corrigir com texto novo.* A relação financeira foi corrigida. O texto agora reflete o FAT como fonte custeadora originária (art. 239 da CF) e a Caixa como agente pagador.
* **EF-2 (Empregador Web vs. eSocial):** *(a) Corrigir com texto novo.* Referências ao Empregador Web foram atualizadas para o eSocial como o sistema vigente de integração e gatilho inicial.
* **EF-3 (MTE e elegibilidade):** *(a) Corrigir com texto novo.* O CODEFAT foi incluído como o órgão máximo deliberativo tripartite que define as normas.
* **EF-4 ("Dinheiro do MTE"):** *(a) Corrigir com texto novo.* Corrigido para refletir a gestão do fundo constitucional e a separação de papéis entre MTE (secretaria executiva) e FAT.

**2. Lacunas de Evidência Críticas**
* **LE-1 (Maior causa de abandono):** *(c) Marcar explicitamente como pendente / em-aberto.* A afirmação superlativa foi removida do corpo do texto e transformada em uma lacuna de métrica que exige aferição empírica.
* **LE-2 (Derrubar ligação de propósito):** *(c) Marcar explicitamente como pendente / em-aberto.* O "comportamento doloso" foi remanejado para a seção de hipóteses comportamentais a serem validadas por pesquisa etnográfica.
* **LE-3 (Sincronização noturna):** *(c) Marcar explicitamente como pendente / em-aberto.* Transformada em premissa arquitetural pendente de validação junto à TI da Caixa.
* **LE-4 (Viés de sotaque no NLP):** *(c) Marcar explicitamente como pendente / em-aberto.* Movida para as hipóteses analíticas, referenciando o viés da literatura de ASR (Automatic Speech Recognition) a ser testado no contexto específico da Caixa.
* **LE-5 ("Medo" do TCU):** *(c) Marcar explicitamente como pendente / em-aberto.* A afirmação de "processo defensivo" foi reestruturada como hipótese teórica organizacional que demanda investigação em processos de auditoria passados.
* **LE-6 (Vulnerabilidade emocional):** *(b) Defender com argumento contrário / (c) Pendente.* **Defesa:** A vulnerabilidade econômica do requerente do benefício é inerente à própria natureza da política pública (proteção ao desemprego involuntário e caráter de verba alimentar), amparada em premissas socioeconômicas basilares. Contudo, **(c)** a mensuração do impacto *emocional* na jornada da URA foi devidamente remarcada como pendente de dados de *Customer Effort Score* (CES).
* **LE-7 (Ausência de métricas):** *(c) Marcar explicitamente como pendente / em-aberto.* Foi criada uma subseção explícita de "Métricas Ausentes" que precisam ser levantadas.

**3. Inferências Mal-Suportadas**
* **IMS-1 (ACD penaliza chamadas complexas):** *(c) Marcar explicitamente como pendente / em-aberto.* A suposta disfunção do algoritmo foi confinada às hipóteses de validação técnica.
* **IMS-2 (URA para reduzir custo vs. normas):** *(a) Corrigir com texto novo.* Inseridos os condicionantes federais (e-PING, TCU) como elementos de design sistêmico.
* **IMS-3 (Premissa da falsa contenção):** *(a) Corrigir com texto novo.* O viés redacional foi expurgado das seções descritivas.
* **IMS-4 ("Teto de vidro" incorreto):** *(a) Corrigir com texto novo.* Substituído pelo termo conceitualmente correto: "Barreiras Sistêmicas de Acesso".
* **IMS-5 (Ausência de Owner):** *(c) Marcar explicitamente como pendente / em-aberto.* A estrutura de governança foi marcada como lacuna de investigação (verificação do organograma).

**4. Atribuições Incorretas**
* **AI-1 (SLI vs SLA):** *(a) Corrigir com texto novo.* Correção para SLAs focados em disponibilidade (uptime) vs. SLAs/SLOs focados em resolutividade no primeiro contato.
* **AI-2 (Frontstage/Backstage sem citação):** *(a) Corrigir com texto novo.* Citação nominal a G. Lynn Shostack e o framework de *Service Blueprinting*.

**5. Atores Omitidos Relevantes**
* **AO-1 a AO-6 (CODEFAT, Empregadores, SRTE/SINE, Gov.br, Judiciário e Modalidades do Cidadão):** *(a) Corrigir com texto novo.* Todos os 6 atores/categorias foram integrados ao ecossistema sociotécnico v2, alterando radicalmente a cadeia de dependências mapeada.

---

## PARTE 2: DOSSIÊ DE PESQUISA (V2 REVISADA)

# Pesquisa Aprofundada: Ecossistema e Jornada do Usuário no Atendimento ao Seguro-Desemprego via URA Caixa (V2)

## 1. Introdução e Abordagem Metodológica
Este documento apresenta o mapeamento do serviço público de atendimento ao Seguro-Desemprego via Unidade de Resposta Audível (URA) da Caixa Econômica Federal. Utilizando como base teórica o *Service Blueprinting* (Shostack, 1984), o mapa transcende o fluxo telefônico em si, dividindo a jornada entre atores visíveis ao cidadão (*frontstage*), infraestruturas operacionais (*backstage*) e instâncias de governança do macroambiente.

Dado o caráter de verba alimentar do benefício, o serviço opera sobre uma base de usuários inerentemente exposta a riscos de vulnerabilidade econômica. Para garantir o rigor analítico, esta pesquisa delimita estritamente o que é fluxo operacional estabelecido e o que são hipóteses empíricas pendentes de verificação no campo.

---

## 2. Mapeamento Analítico dos Atores

Para efeitos de acurácia ecossistêmica, a cadeia se inicia muito antes da chamada telefônica e envolve ramificações de poder e custódia variadas.

### 2.1. O Macroambiente (Governança e Origem)

**A. Empregadores (Empresas)**
* **Categoria:** Organização (Privada/Pública).
* **Papel:** Iniciadores formais da cadeia.
* **Responsabilidades:** Comunicar formalmente a rescisão do contrato de trabalho sem justa causa por meio do eSocial.
* **Riscos e Impactos na UX:** Erros de digitação no eSocial, atrasos na comunicação ou divergências de dados cadastrais geram bloqueios automáticos no sistema. Quando o cidadão liga na URA e ouve "benefício não localizado", a causa-raiz comumente reside neste ator.

**B. CODEFAT (Conselho Deliberativo do Fundo de Amparo ao Trabalhador)**
* **Categoria:** Órgão Colegiado Deliberativo (Tripartite).
* **Papel:** Gestor supremo das regras e dos recursos.
* **Responsabilidades:** Aprovar resoluções que definem os critérios operacionais, alocação de verbas e prazos do benefício. É composto por representantes do Governo, Trabalhadores e Empregadores.
* **Riscos e Impactos:** O distanciamento físico do Conselho em relação às trincheiras de atendimento. Resoluções complexas muitas vezes dificultam a tradução sistêmica em árvores de URA.

**C. Ministério do Trabalho e Emprego (MTE)**
* **Categoria:** Órgão Público Federal.
* **Papel:** Secretaria executiva do CODEFAT e processador de dados trabalhistas.
* **Responsabilidades:** Consolidar os dados do eSocial, aplicar as regras de elegibilidade estabelecidas na Lei 7.998/1990 e resoluções do CODEFAT, e autorizar a Caixa a efetuar os pagamentos com recursos do FAT.
* **Dependências:** Depende da higienização dos dados vindos do eSocial.

**D. O FAT (Fundo de Amparo ao Trabalhador)**
* **Categoria:** Fundo Constitucional.
* **Papel:** Custódia financeira originária (alimentado por recursos do PIS/PASEP), que repassa os recursos para o agente pagador atuar.

### 2.2. A Instância Operacional Estratégica

**E. Caixa Econômica Federal (Gestora do Canal)**
* **Categoria:** Empresa Pública Federal (Agente Pagador).
* **Papel:** Operadora da rede de pagamento e do canal de atendimento.
* **Responsabilidades:** Traduzir as regras do MTE/CODEFAT em scripts de atendimento, licitar as plataformas de telefonia e empresas de contact center.
* **Riscos e Impactos:** Falha na adequação das árvores da URA a normativos federais (como o padrão e-PING) ou a burocratização excessiva da jornada por receio de sanções de auditoria.

**F. Canais Digitais Paralelos (Portal Gov.br e CTPS Digital)**
* **Categoria:** Sistema/Plataforma.
* **Papel:** Ecossistema digital que absorve (ou deveria absorver) a carga principal de requerimentos.
* **Interações e Dependências:** A URA atua frequentemente em complemento ou falha deste canal. Usuários que não conseguem validação biométrica no Gov.br migram compulsoriamente para a URA ou canais físicos.

**G. Órgãos de Controle (TCU, CGU, MPF)**
* **Categoria:** Órgão de Estado.
* **Papel:** Fiscalização e Auditoria.
* **Responsabilidades:** Auditar o uso do dinheiro do FAT e os contratos bilionários de terceirização do atendimento da Caixa.

### 2.3. O Frontstage (Linha de Frente e Usuário)

**H. Cidadãos Requerentes (Segmentados)**
* **Categoria:** Pessoa / Usuário Final.
* **Papel:** Beneficiário que interage com o canal.
* **Segmentação Necessária:** A jornada não é monolítica. As opções de URA e bases legais diferem substancialmente para trabalhadores formais (CLT padrão), empregados domésticos, pescadores artesanais (Seguro Defeso) e trabalhadores resgatados, criando árvores de navegação e atritos muito distintos.

**I. Sistemas Automatizados (URA)**
* **Categoria:** Sistema.
* **Responsabilidades:** Triagem e contenção via autoatendimento (TTS).
* **Dependências:** Integração em tempo real com bancos de dados. A URA está submetida a uma dupla pressão: resolver a demanda do cidadão e seguir estritas normativas federais de tecnologia.

**J. Mecanismos de Reconhecimento de Voz (ASR/NLP)**
* **Categoria:** Sistema Tecnológico.
* **Papel:** Identificação de intenção do usuário sem uso de teclado (DTMF).

**K. Atendentes Humanos**
* **Categoria:** Pessoa (Terceirizados).
* **Responsabilidades:** Escalar chamadas complexas e orientar correções no eSocial ou comparecimento ao SINE.

### 2.4. O Destino Físico e Judiciário (Overflow)

**L. SRTEs (Superintendências Regionais do Trabalho) e SINE**
* **Categoria:** Órgão/Rede Física de Atendimento.
* **Papel:** Instância de absorção de falhas sistêmicas.
* **Impacto na UX:** Quando a URA falha de forma definitiva na resolução de divergências de dados da rescisão, o cidadão é deslocado a essa rede.

**M. Defensoria Pública da União (DPU) e Juizado Especial Federal (JEF)**
* **Categoria:** Órgão do Sistema de Justiça.
* **Papel:** Ator de última instância, acionado na ponta final da jornada de não resolução (negativa indevida de benefício).

---

## 3. Consolidação e Dinâmicas de Governança

Ao aplicar a separação *frontstage/backstage* (Shostack), fica evidente que grande parte das falhas percebidas no *frontstage* da Caixa (a URA ou o Atendente) não nasce no canal, mas reflete desvios nas etapas de alimentação de dados (eSocial) e regras do ecossistema tripartite (CODEFAT).

**Dependências Críticas Remapeadas:**
O cidadão não depende apenas do "sistema da Caixa". Ele depende fundamentalmente do contador da empresa onde trabalhava ter imputado corretamente a data de rescisão no eSocial e do processamento desse evento pelo Dataprev/MTE, para que só então a URA da Caixa possua informações válidas para informar o status das parcelas.

---

## 4. Auditoria de Dados: Lacunas e Hipóteses de Campo (Pendente)

Uma limitação estrita deste mapeamento inicial é a ausência de volumetria e validação de inferências comportamentais, que demandam acesso a logs restritos e pesquisa primária. Ficam registradas explícita e textualmente como **pendentes / em-aberto**:

### A. Lacunas de Dados Quantitativos (Métricas Ausentes)
Nenhum diagnóstico definitivo sobre o desempenho do serviço pode ser feito sem a obtenção de:
* Volume anual de ligações para a opção do Seguro-Desemprego.
* Taxa de abandono dentro da árvore de opções.
* Taxas de resolução medidas por FCR (*First Contact Resolution*) visando contrapor métricas de SLA de disponibilidade (infraestrutura) a SLAs/SLOs de resolutividade.

### B. Hipóteses para Investigação Organizacional e Operacional
* **H1 - A Hipótese da Falsa Contenção:** A alta taxa de encerramento de chamadas pela URA pode não representar resolução, mas sim repasse de demanda para a rede física (SINE/SRTE). Demanda validação por meio do cruzamento de logs telefônicos e atendimentos no SINE num delta de 48 horas.
* **H2 - Barreiras Sistêmicas e Viés de NLP:** Com base na literatura consolidada sobre reconhecimento automatizado de voz, formula-se a hipótese de que o sistema NLP específico em uso pela Caixa pode penalizar dialetos regionais, configurando uma barreira sistêmica ("muro de exclusão"). Demanda teste empírico em campo segmentado por DDD.
* **H3 - Arquitetura de Integração Oculta:** Qual é o desenho de infraestrutura exata entre a base do eSocial (MTE) e a Caixa? Falhas de comunicação em massa reportadas pela URA exigem análise da engenharia e dos tempos de processamento/lotes entre esses sistemas.
* **H4 - Desvios Comportamentais (O Fator TMA):** É necessário investigar por meio de pesquisa etnográfica o potencial de que a cobrança por metas estritas de Tempo Médio de Atendimento (TMA) esteja induzindo atendentes terceirizados à prática negligente de encerrar prematuramente ligações complexas.
* **H5 - Dinâmicas de Governança Defensiva e Ownership:** Avaliar se a pressão fiscalizatória (TCU) gera processos de URA excessivamente rígidos e confirmar formalmente nos contratos qual área da Caixa (ou fora dela) detém o *ownership* (titularidade) do sucesso da jornada de ponta a ponta.
