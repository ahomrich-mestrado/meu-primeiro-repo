# C_grill_transcript — Sessão /grill-me: Mapa de Atores URA Seguro-Desemprego

**Contexto:** Sessão de entrevista estruturada (/grill-me) para especificação de um mapa de atores da jornada "Atendimento ao Seguro-Desemprego via URA Caixa", com base no artefato `B_relatorio_assistente_v3.md`.

---

## Pergunta 1 — Produto final

**Claude:** O documento já elenca 17+ atores organizados em camadas (Macroambiente → Backstage → Frontstage → Overflow). Antes de entrar nas decisões de estrutura, preciso entender o destino do mapa.

Qual é o produto final esperado?

| Opção | Descrição |
|---|---|
| A | **Diagrama visual** (ex: stakeholder map, bolhas concêntricas, grafo de dependências) |
| B | **Tabela/matriz estruturada** (atores × atributos: papel, poder, dependência) |
| C | **Service Blueprint** estendido (swimlanes com atores em linha do tempo da jornada) |
| D | **Texto narrativo enriquecido** com elementos visuais embutidos |

*Recomendação: A — diagrama visual em camadas concêntricas, pois o documento já organiza os atores nessa lógica e comunica assimetrias de poder de forma imediata.*

**Usuário:** A

---

## Pergunta 2 — Audiência

**Claude:** Para qual audiência é o diagrama? Isso define o nível de detalhe, o vocabulário e o quanto de teoria (Goffman, Shostack) precisa aparecer explicitamente.

| Opção | Perfil |
|---|---|
| A | **Acadêmica** — banca, orientador, artigo científico |
| B | **Gestores públicos / policy makers** — MTE, Caixa |
| C | **Equipe de UX/design de serviço** |
| D | **Uso interno de pesquisa** |

*Recomendação: A (acadêmica), dado o aparato teórico explícito do documento. Porém a escolha do usuário redirecionou para UX.*

**Usuário:** C

---

## Pergunta 3 — Ferramenta de produção

**Claude:** Para audiência de UX/design de serviço, o diagrama precisa ser visualmente polido e editável. Qual ferramenta usar?

| Opção | Ferramenta | Trade-off |
|---|---|---|
| A | **Figma / FigJam** | Máxima liberdade visual; exige conta e familiaridade |
| B | **Miro** | Ótimo para colaboração; templates prontos |
| C | **draw.io / diagrams.net** | Gratuito, exporta SVG/PNG, bom para diagramas técnicos |
| D | **Código** — Mermaid, Graphviz, D3.js | Versionável; curva de aprendizado maior |
| E | **PowerPoint / Google Slides** | Acessível; limitado para layouts não-lineares |

*Recomendação: C (draw.io) — gratuito, roda no browser, exporta em alta resolução, suporte nativo a layouts concêntricos.*

**Usuário:** C

---

## Pergunta 4 — Layout visual

**Claude:** Com draw.io e audiência de UX, qual layout para o diagrama?

| Opção | Layout | Como ficaria |
|---|---|---|
| A | **Camadas concêntricas** (onion diagram) | Cidadão no centro → Frontstage → Backstage → Macroambiente na borda |
| B | **Swimlanes horizontais** | Cada camada é uma faixa; atores da esquerda (macro) para direita (cidadão) |
| C | **Grafo de dependências** | Nós ligados por setas; sem hierarquia de camadas explícita |

*Recomendação: A — comunica imediatamente a distância estrutural entre quem decide e quem sofre as consequências, que é a tese central do documento.*

**Usuário:** A

---

## Pergunta 5 — Atores ou também relações?

**Claude:** O diagrama mostra só os atores ou também as relações entre eles?

| Opção | Descrição | Risco |
|---|---|---|
| A | **Só atores** — sem setas | Limpo, mas não mostra dependências críticas |
| B | **Atores + setas selecionadas** — só as relações mais críticas para o cidadão | Equilíbrio entre clareza e profundidade |
| C | **Atores + todas as relações mapeáveis** | Rico, mas provavelmente ilegível com 17+ atores |

*Recomendação: B — mostrar apenas as relações com impacto direto na jornada do cidadão.*

**Usuário:** B

---

## Pergunta 6 — Quais relações priorizar?

**Claude:** Para não sobrecarregar o diagrama, quais setas entram?

| # | Relação | Por que é crítica |
|---|---|---|
| 1 | Empregador → Dataprev → MTE → URA → Cidadão | Cadeia principal de falha: erro na origem vira "benefício não localizado" |
| 2 | Seg. Informação (KBA) → Cidadão | Barreira de autenticação como mecanismo de exclusão |
| 3 | CODEFAT → Caixa → URA | Regras complexas que a URA não consegue traduzir em teclado numérico |
| 4 | ACD/CTI → Atendente Humano → Cidadão | Roteamento que pode reter casos complexos indefinidamente (H5) |

*Recomendação: todas as 4, com cores diferentes por tipo de relação.*

**Usuário:** todas as 4

---

## Pergunta 7 — Diferenciação visual dos tipos de ator

**Claude:** Como diferenciar visualmente os tipos de ator?

| Opção | Diferenciação | Exemplo |
|---|---|---|
| A | **Forma geométrica** — retângulo (org), círculo (pessoa), hexágono (sistema) | Distinção clara, maior complexidade |
| B | **Cor de preenchimento** — uma cor por tipo de ator | Intuitivo para UX; legenda simples |
| C | **Ícone interno** — ícone de pessoa, engrenagem, prédio | Visual rico; mais trabalhoso |
| D | **Só cor de borda** | Minimalista; menos impacto visual |

*Recomendação: B — 5 cores: azul (órgão público), cinza (sistema), laranja (org privada), verde (pessoa), roxo (fundo/lei).*

**Usuário:** B

---

## Pergunta 8 — Hipóteses no diagrama?

**Claude:** O diagrama inclui as hipóteses (H1–H5) ou só o estado atual mapeado?

| Opção | Descrição | Risco |
|---|---|---|
| A | **Só estado atual** | Mais limpo; não contamina com incerteza |
| B | **Hipóteses sinalizadas** — setas/atores com marcação visual (tracejado, ícone "?") | Honesto epistemicamente; útil para priorizar pesquisa de campo |
| C | **Diagrama duplo** — versão "atual" e versão "hipóteses" separadas | Completo, mas dobra o trabalho |

*Recomendação: B — setas tracejadas com cor diferente para relações hipotéticas.*

**Usuário:** B

---

## Pergunta 9 — Formato de entrega

**Claude:** O draw.io permite exportar em vários formatos. Qual entregar?

| Opção | Formato | Quando usar |
|---|---|---|
| A | **PNG** — imagem estática em alta resolução | Apresentações, documentos |
| B | **SVG** — vetor escalável | Redimensionamento sem perda |
| C | **PDF** — página única | Impressão ou entrega formal |
| D | **XML (.drawio)** — arquivo editável nativo | Quando a equipe precisar continuar editando |

*Recomendação: A + D — PNG para uso imediato, .drawio para iteração da equipe.*

**Usuário:** A+D

---

## Pergunta 10 — Uso imediato do diagrama

**Claude:** Onde este diagrama será usado primeiro? Isso define proporção e densidade de texto nos nós.

| Opção | Contexto |
|---|---|
| A | Apresentação para stakeholders (slides) |
| B | Documento de pesquisa / relatório escrito |
| C | Workshop com a equipe de design |
| D | Ainda não definido |

*Recomendação: definir para calibrar proporção (16:9 para slides vs. A4 para documento) e densidade dos rótulos.*

**Usuário:** B

---

## Especificação Final Consolidada

| Decisão | Escolha |
|---|---|
| Produto | Diagrama visual |
| Audiência | Equipe de UX / design de serviço |
| Ferramenta | draw.io / diagrams.net |
| Layout | Camadas concêntricas (onion) — cidadão no centro |
| Conteúdo | Atores + relações críticas selecionadas |
| Relações incluídas | 4 cadeias: dados, KBA, norma, roteamento |
| Código visual | Cor de preenchimento por tipo de ator (5 cores) |
| Hipóteses | Sinalizadas com setas tracejadas (roxo) |
| Formato de entrega | PNG + .drawio editável |
| Uso imediato | Documento de pesquisa / relatório escrito (proporção A4) |

---

## Artefato Gerado

**Arquivo:** `mapa_atores_ura_seguro_desemprego.drawio`

**Conteúdo do diagrama:**

- 5 anéis concêntricos: Cidadão (centro) → Frontstage → Backstage Tecnológico → Backstage Estratégico → Macroambiente → Transbordo Físico/Institucional
- 17 atores (A–S) posicionados em seus respectivos anéis e coloridos por tipo
- 3 relações sólidas: cadeia de dados (vermelho), barreira KBA (laranja), cadeia normativa (azul)
- 1 relação tracejada: H5 — roteamento ACD (roxo)
- Legenda completa no canto inferior esquerdo
- Crédito de fonte com referência ao documento-base e aos frameworks teóricos (Goffman 1959, Shostack 1984)

**Como exportar PNG:** abrir em [diagrams.net](https://app.diagrams.net) → File → Export as → PNG.
