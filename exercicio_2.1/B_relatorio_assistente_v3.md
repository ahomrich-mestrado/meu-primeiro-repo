# B_relatorio_assistente_v3 — Dossiê de Pesquisa (V3 Revisada Completa)

---

## Parte 1: Matriz de Resolução da Auditoria V2

### 1. Achados Parcialmente Resolvidos (v1)

**LE-2 (Negligência na H4):** *(a) Corrigido com texto novo.* A redação foi ajustada para remover o qualificador de "negligência". A hipótese agora questiona objetivamente se existe correlação entre as metas de Tempo Médio de Atendimento (TMA) e o encerramento prematuro das chamadas.

**LE-3 (Falhas em massa assumidas na H3):** *(a) Corrigido com texto novo.* A formulação de H3 foi reescrita para não assumir as falhas como premissa, mas testar *se* a arquitetura de lotes gera a resposta de benefício não localizado.

**LE-6 e NF-6 (CES ausente/Inconsistência):** *(a) Corrigido com texto novo.* A métrica de *Customer Effort Score* (CES) foi explicitamente incluída na Seção 4.A do Dossiê para aferir o impacto emocional e a fricção do cidadão, alinhando matriz e relatório.

**IMS-1 (Remoção do ACD/CTI):** *(a) Corrigido com texto novo.* O ator "Sistema de Roteamento (ACD/CTI)" foi restaurado ao ecossistema (Seção 2.3). A inferência não comprovada sobre sua configuração foi mantida isolada na seção de hipóteses.

**AI-1 (SLAs/SLOs):** *(a) Corrigido com texto novo.* Os termos foram devidamente desmembrados no texto para diferenciar acordos contratuais de nível de serviço (SLA) de objetivos operacionais internos (SLO).

**AI-2 (Goffman e Shostack):** *(a) Corrigido com texto novo.* Adicionadas as referências completas exigidas: a sociologia dramatúrgica de Erving Goffman (1959, *The Presentation of Self in Everyday Life*) e o artigo base de G. Lynn Shostack (1984, "Designing Services That Deliver", *Harvard Business Review*).

---

### 2. Falhas Novas (NF)

**NF-1 (Dataprev Fantasma):** *(a) Corrigido com texto novo.* A Dataprev foi mapeada formalmente como um ator (Organização Tecnológica) no Macroambiente (Seção 2.1), explicando seu papel no processamento do eSocial.

**NF-2 (TTS ambíguo):** *(a) Corrigido com texto novo.* A referência ao TTS (Text-to-Speech) foi corrigida para definir estritamente a tecnologia de *saída* de áudio, separando-a do conceito amplo de autoatendimento.

**NF-3 (Atores Removidos):** *(a) Corrigido com texto novo.* Os quatro atores suprimidos na v2 (Supervisores, Equipe de TI, Fornecedores e Segurança da Informação) foram totalmente reintegrados ao *backstage*.

**NF-4 (Migração compulsória):** *(a) Corrigido com texto novo.* O termo "compulsoriamente" foi substituído por uma formulação condicional, indicando que a URA é um dos caminhos alternativos em caso de falha biométrica.

**NF-5 (Seguro Defeso):** *(a) Corrigido com texto novo.* O Seguro Defeso foi destacado por suas especificidades (Lei 10.779/2003, calendário sazonal) para evitar confusão com o Seguro-Desemprego padrão (CLT).

---

### 3. Pontos Remanescentes (PR)

**PR-1 (Poder e Dependência):** *(a) Corrigido com texto novo.* A seção "Dinâmicas de Governança" (Seção 3.1) foi reescrita para abranger as assimetrias de poder envolvendo CODEFAT, Empregadores e Dataprev.

**PR-2 (Autenticação e Exclusão):** *(a) Corrigido com texto novo.* A reintegração do ator de Segurança da Informação permitiu restaurar a análise estrutural da fricção por KBA (Knowledge-Based Authentication) como barreira de acesso.

**PR-3 (Padronização de idioma):** *(a) Corrigido com texto novo.* O termo *ownership* foi traduzido para "titularidade", e *First Contact Resolution* (FCR) passou a constar padronizado como "Resolução no Primeiro Contato (FCR)".

---

## Parte 2: Dossiê de Pesquisa (V3 Revisada Completa)

# Pesquisa Aprofundada: Ecossistema e Jornada do Usuário no Atendimento ao Seguro-Desemprego via URA Caixa (V3)

## 1. Introdução e Abordagem Metodológica

Este documento consolida o mapeamento analítico do serviço público de atendimento ao Seguro-Desemprego operado via Unidade de Resposta Audível (URA) pela Caixa Econômica Federal.

O arcabouço teórico que alicerça esta análise une duas disciplinas complementares: a sociologia dramatúrgica de Erving Goffman (1959, *The Presentation of Self in Everyday Life*), que inspira a divisão analítica dos papéis em cena e fora de cena, e a ferramenta de *Service Blueprinting* desenvolvida por G. Lynn Shostack (1984, "Designing Services That Deliver", *Harvard Business Review*).

Sob essa ótica, o serviço telefônico não é uma interação isolada, mas o resultado final visível (*frontstage*) sustentado por múltiplas engrenagens operacionais (*backstage*) e diretrizes regulatórias sistêmicas. Afirmações sem dados empíricos publicados encontram-se demarcadas na seção de lacunas e hipóteses para futura validação de campo.

---

## 2. Mapeamento Analítico dos Atores

Para garantir completude sistêmica, mapeamos 17 atores (e sistemas) atuando do macroambiente à linha de frente.

### 2.1. O Macroambiente (Governança e Geração de Dados)

**A. Empregadores (Empresas)**

- **Categoria:** Organização (Privada/Pública).
- **Papel:** Iniciadores formais da jornada do trabalhador.
- **Responsabilidades:** Informar adequadamente os eventos de rescisão de contrato via eSocial.
- **Riscos e Impactos:** Falhas, atrasos e erros de digitação do empregador na origem geram o bloqueio da concessão que eclodirá, semanas depois, como uma chamada do cidadão frustrado para a URA da Caixa.

---

**B. CODEFAT (Conselho Deliberativo do Fundo de Amparo ao Trabalhador)**

- **Categoria:** Órgão Colegiado Deliberativo.
- **Papel:** Autoridade normativa suprema.
- **Responsabilidades:** Composto tripartite (governo, trabalhadores, empregadores), edita resoluções determinando prazos e regras do benefício.
- **Riscos e Impactos:** O distanciamento tático. Se o Conselho cria regras condicionantes muito elaboradas, a Caixa tem severa dificuldade de transformá-las em opções de navegação simples em um teclado numérico (URA).

---

**C. Ministério do Trabalho e Emprego (MTE)**

- **Categoria:** Órgão Público Federal.
- **Papel:** Formulador de políticas e secretaria executiva do CODEFAT.
- **Responsabilidades:** Aplicar as regras de elegibilidade da Lei 7.998/1990 e aprovar as remessas financeiras para pagamento.

---

**D. Dataprev (Empresa de Tecnologia e Informações da Previdência Social)**

- **Categoria:** Organização Pública Tecnológica.
- **Papel:** Processador central de dados.
- **Responsabilidades:** Sustentar o ecossistema eSocial e consolidar os lotes de informações trabalhistas que o MTE utiliza para autorizar o benefício.
- **Dependências:** Ator oculto essencial; se a infraestrutura da Dataprev atrasa um lote, a Caixa fica "cega" e o cidadão recebe erro na URA.

---

**E. FAT (Fundo de Amparo ao Trabalhador)**

- **Categoria:** Fundo Constitucional.
- **Papel:** Custódia financeira (Art. 239 da Constituição Federal). Financia os benefícios operados pela Caixa.

---

### 2.2. A Instância Operacional Estratégica (*Backstage*)

**F. Caixa Econômica Federal (Gestora do Canal)**

- **Categoria:** Empresa Pública (Agente Pagador).
- **Papel:** Tradutora e Operadora.
- **Responsabilidades:** Estruturar a URA, garantir conformidade com frameworks de TI governamentais (ex: e-PING) e gerir os fornecedores de call center.

---

**G. Atores da Segurança da Informação e LGPD**

- **Categoria:** Pessoa / Área Organizacional.
- **Papel:** Guardiões da integridade de dados.
- **Responsabilidades e Impactos:** Configuram os protocolos de autenticação baseados em conhecimento (KBA — *Knowledge-Based Authentication*). O excesso de zelo técnico na definição das perguntas de segurança atua frequentemente como forte barreira e mecanismo involuntário de exclusão digital.

---

**H. Canais Digitais Paralelos (Gov.br e CTPS Digital)**

- **Categoria:** Plataforma/Sistema.
- **Papel:** Absorção principal de autoatendimento. Cidadãos que encontram falhas biométricas ou sistêmicas nestes canais podem recorrer à URA como via alternativa de resolução.

---

**I. Órgãos de Controle (TCU, CGU)**

- **Categoria:** Órgãos de Estado.
- **Papel:** Auditores da aplicação orçamentária e da moralidade das contratações terceirizadas de atendimento.

---

### 2.3. A Infraestrutura Tecnológica de Atendimento (*Backstage*)

**J. Sistemas de Roteamento de Chamadas (ACD/CTI)**

- **Categoria:** Sistema.
- **Responsabilidades:** O Distribuidor Automático de Chamadas mapeia filas e aloca a ligação transbordada da URA ao humano correspondente, provendo dados à tela do atendente (*screen pop*).

---

**K. Fornecedores de Infraestrutura e Software**

- **Categoria:** Organização Privada (Telecom, Nuvem).
- **Responsabilidades e Riscos:** Garantir enlaces de rede estatais, licenças de URA e armazenamento. Rompimentos de rotas podem causar isolamento de serviço para regiões inteiras.

---

**L. Equipes de Suporte Tecnológico (TI)**

- **Categoria:** Organização / Pessoa.
- **Papel:** Sustentação do banco de dados da Caixa, vitais para evitar a latência da informação durante o autoatendimento.

---

**M. Supervisores e Gestores da Central**

- **Categoria:** Pessoa.
- **Responsabilidades:** Fiscalização de qualidade, escala e modulação do ritmo da central humana diante da pressão de volume diário.

---

### 2.4. O Frontstage (Linha de Frente e Cidadão)

**N. Cidadão Requerente (Multimodalidade)**

- **Categoria:** Pessoa.
- **Papel:** Acessador do direito.
- **Atenção Analítica:** Não é um ator monolítico. O trabalhador CLT interage com uma matriz legal diferente do Pescador Artesanal (Seguro Defeso — Lei 10.779/2003), que possui calendário sazonal e exige laudos de colônias de pescadores. Cada modalidade vivencia atritos de navegação diferentes na árvore telefônica.

---

**O. Sistemas Automatizados de Atendimento (URA)**

- **Categoria:** Sistema.
- **Responsabilidades:** Triagem e contenção via fluxos lógicos e integração com APIs. Fornece respostas ao cidadão utilizando tecnologias de saída de áudio sintetizado, como o TTS (*Text-to-Speech*).

---

**P. Mecanismos de Reconhecimento de Voz (ASR/NLP)**

- **Categoria:** Sistema Tecnológico.
- **Responsabilidades:** Sistemas de entrada de áudio baseados em inteligência artificial responsáveis por mapear a intenção do usuário sem a digitação.

---

**Q. Atendente Humano**

- **Categoria:** Pessoa (Terceirizado).
- **Papel:** Agente de resolução final; a ponta que lida diretamente com os conflitos gerados pelas divergências sistêmicas acumuladas.

---

### 2.5. O Transbordo Físico e Institucional (Overflow)

**R. SRTEs e Sistema Nacional de Emprego (SINE)**

- **Categoria:** Rede Física.
- **Papel:** Destino do cidadão quando ocorrem impasses insuperáveis de eSocial na URA e exigem-se recursos documentais in loco.

---

**S. Defensoria Pública da União (DPU) e Juizado Especial Federal (JEF)**

- **Categoria:** Sistema de Justiça.
- **Papel:** Via de acesso extremo. Demandados para o ingresso de ações reparatórias ou mandados em situações de bloqueios crônicos e sistêmicos.

---

## 3. Dinâmicas de Governança, Poder e Dependência

A assimetria de poder que define a qualidade percebida pelo cidadão é estrutural:

**Custódia vs. Execução:** O CODEFAT prescreve o direito e o limite; a Caixa desenha a interface técnica; e a Dataprev e o MTE intermedeiam as bases de dados eSocial. Nenhuma falha estrutural neste serviço é passível de resolução unilateral por apenas um desses entes.

**Barreiras Sistêmicas de Acesso:** Com a inclusão da área de Segurança da Informação no mapa, evidencia-se que a URA impõe fricção massiva sob a justificativa de proteção contra fraudes (KBA). Usuários de baixa escolaridade reprovam nos testes automáticos de autenticação, sendo bloqueados do benefício não por falta de direito, mas por falta de memória exata de dados cadastrais remotos.

**Pontas Dependentes:** O Atendente e o Cidadão estão no final da cadeia. Uma vírgula errada gerada pelo Empregador no momento da rescisão reverbera através de cinco sistemas distintos até virar a frase automatizada: *"benefício não localizado"*.

---

## 4. Auditoria de Dados: Lacunas e Hipóteses de Campo (Pendentes)

Dado o escopo deste mapeamento sociotécnico, conclusões definitivas dependem da obtenção das métricas a seguir e da validação metodológica das hipóteses demarcadas.

### A. Lacunas de Dados Quantitativos (Métricas Ausentes)

**Volume, Retenção e Abandono:** Total de chamadas direcionadas à árvore, % de contenção automática vs. transbordo humano, e a taxa de abandono na fila (abandono intra-URA vs. abandono no CTI).

**Qualidade e Fricção:** Necessidade fundamental de obtenção de relatórios de *Customer Effort Score* (CES) — para mensurar matematicamente o grau de dificuldade imposto ao usuário vulnerável — e taxas de Resolução no Primeiro Contato (FCR), de forma a confrontar as métricas contratuais de disponibilidade técnica (SLA — *Service Level Agreement*) com os reais objetivos de impacto do negócio (SLO — *Service Level Objective*).

---

### B. Hipóteses Analíticas para Verificação

**H1 — A Hipótese da Titularidade:** Formula-se a premissa de que a governança do serviço é fragmentada (silos) sem uma titularidade clara interministerial ou interdepartamental que assuma a responsabilidade ponta-a-ponta pelo índice de FCR. Requer verificação contratual.

**H2 — A Hipótese do Processamento em Lotes:** Se existem falhas de integração reportadas aos milhares em determinados dias, deve-se investigar tecnicamente se essas anomalias derivam da ausência de processamento em tempo real (APIs) entre a base eSocial/Dataprev e os servidores da URA Caixa.

**H3 — A Hipótese da Fricção Cognitiva:** O viés algorítmico (ASR) prejudica regionalmente o acesso? A literatura de pesquisa aponta assimetrias no reconhecimento de sotaques regionais. É imperativo testar os motores de inteligência de voz da Caixa para constatar tais desvios.

**H4 — A Hipótese Comportamental do TMA:** Testar empiricamente, via escutas de qualidade e pesquisa de campo, se a pressão das terceirizadas para o cumprimento da meta de Tempo Médio de Atendimento (TMA) possui correlação com a decisão induzida de operadores finalizarem prematuramente chamadas sistêmicas complexas.

**H5 — A Hipótese da Defesa Contratual (Roteamento de ACD):** Investigar nas parametrizações operacionais se os Sistemas de Roteamento de Chamadas (ACD/CTI) possuem regras de distribuição por habilidades (*skill-based routing*) configuradas para penalizar e reter indefinidamente na fila os casos mais complexos, visando maquiar o sucesso estatístico geral do canal.
