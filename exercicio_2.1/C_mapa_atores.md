# C_mapa_atores — Matriz RACI: Atendimento ao Seguro-Desemprego via URA Caixa

---

## Decisões de design que fundamentam este mapa

Este mapa é derivado de uma sessão de especificação estruturada (ver `C_grill_transcript.md`). As escolhas abaixo rastreiam cada decisão relevante:

| Decisão | Escolha | Referência no transcript |
|---|---|---|
| Produto final | Diagrama + tabela RACI | Pergunta 1 (P1) |
| Audiência | Equipe de UX / design de serviço | P2 |
| Atividades-coluna | 7 atividades da jornada | Passo 1 da construção da RACI |
| Atores-linha | 17 atores mapeados (A–S) | P4 — camadas concêntricas confirmadas |
| Relações críticas priorizadas | Cadeia de dados, KBA, norma, roteamento | P6 — todas as 4 relações confirmadas |
| Hipóteses | Sinalizadas explicitamente (H5) | P8 |

---

## Legenda RACI

| Símbolo | Significado |
|---|---|
| **AR** | Accountable + Responsible — mesmo ator responde e executa |
| **A** | Accountable — responde pelo resultado final |
| **R** | Responsible — executa a atividade |
| **C** | Consulted — consultado antes da execução |
| **I** | Informed — notificado após a execução |
| — | Sem papel nesta atividade |

> **Nota sobre H5:** A atribuição de J. ACD/CTI na Atividade 6 é classificada como **R**, porém corresponde à Hipótese H5 do documento (roteamento como mecanismo de retenção de casos complexos). Pendente de validação empírica.

---

## Matriz RACI

| Ator | Camada | 1. Registro da Rescisão (eSocial) | 2. Processamento e Autorização do Benefício | 3. Configuração das Regras na URA | 4. Autenticação do Cidadão (KBA) | 5. Atendimento Automatizado (URA/ASR) | 6. Atendimento Humano e Roteamento | 7. Transbordo Presencial / Judicial |
|---|---|---|---|---|---|---|---|---|
| A. Empregadores | Macroambiente | **AR** | — | — | — | — | — | — |
| B. CODEFAT | Macroambiente | — | C | **A** | — | — | — | — |
| C. MTE | Macroambiente | I | **AR** | C | — | — | — | C |
| D. Dataprev | Macroambiente | C | **R** | — | — | — | — | — |
| E. FAT | Macroambiente | — | I | — | — | — | — | — |
| F. Caixa Econômica Federal | Backstage Estratégico | — | I | **AR** | C | **A** | **A** | I |
| G. Seg. Informação / LGPD | Backstage Estratégico | — | — | C | **A** | — | — | — |
| H. Gov.br / CTPS Digital | Backstage Estratégico | — | — | — | C | I | — | — |
| I. TCU / CGU | Backstage Estratégico | — | I | I | — | I | I | I |
| J. ACD/CTI *(H5)* | Backstage Tecnológico | — | — | — | — | C | **R** *(H5)* | — |
| K. Fornecedores Telecom | Backstage Tecnológico | — | — | — | — | C | C | — |
| L. Equipe de TI | Backstage Tecnológico | — | — | C | C | **R** | C | — |
| M. Supervisores da Central | Backstage Tecnológico | — | — | — | — | I | **A** | — |
| N. Cidadão Requerente | Frontstage | I | I | — | **R** | **R** | I | R |
| O. URA | Frontstage | — | — | — | **R** | **R** | — | — |
| P. ASR / NLP | Frontstage | — | — | — | — | C | — | — |
| Q. Atendente Humano | Frontstage | — | — | — | — | — | **R** | I |
| R. SRTEs / SINE | Transbordo | — | — | — | — | — | — | **R** |
| S. DPU / JEF | Transbordo | — | — | — | — | — | — | **R** |

---

## Análise de lacunas e achados RACI

### Atividades sem Accountable único (risco de fragmentação)
- **Atividade 7 — Transbordo:** múltiplos responsáveis (R. SRTEs, S. DPU/JEF), nenhum Accountable formal atribuído. Isso reflete a Hipótese H1 do documento — ausência de titularidade ponta-a-ponta no serviço.

### Cidadão como Responsible (N)
- O Cidadão aparece como **R** nas Atividades 4 e 5 — é ele quem fornece os dados de KBA e navega a URA. Isso evidencia a assimetria estrutural: o elo mais frágil da cadeia carrega responsabilidade de execução sem ter poder de influência sobre o sistema.

### Ator oculto de alto impacto (Dataprev)
- D. Dataprev aparece apenas nas Atividades 1 e 2, mas suas falhas reverberam em todas as demais. Isso valida a descrição do documento: "ator oculto essencial; se a infraestrutura da Dataprev atrasa um lote, a Caixa fica cega e o cidadão recebe erro na URA" (Seção 2.1).

---

## Referências

- **Documento-base:** `B_relatorio_assistente_v3.md`
- **Transcript da sessão de especificação:** `C_grill_transcript.md`
- **Artefato visual complementar:** `mapa_atores_ura_seguro_desemprego.drawio`
- Goffman, E. (1959). *The Presentation of Self in Everyday Life*. Doubleday.
- Shostack, G. L. (1984). Designing Services That Deliver. *Harvard Business Review*.
