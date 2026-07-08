# Reunião — Superlógica Plugins

_Data: 2026-07-08_

## Anotações

### 1. Posicionamento / relacionamento
- Não vão mais **forçar boleto PJ Bank** para conta pool.
- Reforçaram que estão aqui para **nos atender**.
- Admitiram que no passado **pode ter havido um erro de estratégia**.
- O dizer de mercado **"SL é um banco"** é algo que eles **não querem mais** ser associados.

### 2. Plugins "Nexus"
- Os plugins **"Nexus"** serão **altamente customizáveis**.
- Ciclo de vida de construção de um plugin:
  1. **Solicitação**
  2. **Orçamento**
  3. **Aprovação**
  4. **Desenvolvimento sob medida** ("alfaiataria")
  5. **Uso inicial**
  6. **Melhoramento para outros** (generalização)
  7. **Avaliação e aglomeração** de plugins semelhantes
  8. **Nomeação como plugin oficial** (com suporte, ex.: `plugin-produto`)

### 3. Situação atual do Nexus Plug-ins (IA na prática)

> Legenda: **número grande = SL** | **(número entre parênteses) = sistema Ahreas**

| Etapa | SL | Ahreas |
|---|---|---|
| Entregues | 60 | (2) |
| Em documentação | 5 | (1) |
| Em desenvolvimento / validação | 21 | (8) |
| Em análise | 29 | (9) |

### 4. Primeiros plugins originados da reunião com os clientes RJ (reunião anterior)

> ⚠️ Transcrição de foto borrada — baixa confiança. Partes incertas marcadas com `[?]`; **conferir depois**.

| # | Nome do Plugin (Funcionalidade) | Status de Entrega |
|---|---|---|
| 1 | Dashboard [?] – Gerenciamento de despesas em débito automático | Concluído |
| 2 | Dashboard de Gestão de Carteira (lucro, projeção, crescimento de unidades [?]) | Concluído |
| 3 | Dashboard Métricas – Controla a criação e atualização de despesas | Concluído |
| 4 | [?] de Gestão Condôminos com log de auditoria por grupos [?] | Concluído |
| 5 | [?] Bancária – Gestão completa de Remessa e Retorno #Gestão[?] | Concluído |
| 6 | Lançamento Despesas – Nova interface de lançamento rápido Payline[?] | Concluído |
| 7 | [?] Opcionais – Gestão de campanhas de seguros online [?] | Concluído |
| 8 | [?] seguros[?] – Relatório de conferência de Guia Única | Concluído |
| 9 | [?] Carteira – Controle de saldo do condômino [Conta Pool] | Concluído |
| 10 | [?] Prestação – Personalização completa [data prevista, valor [?]] | Concluído |
| 11 | [?] Automática – Guia Única no Portal | Status diferente — talvez "Aguardando / Em desenvolvimento" [?] |

### 5. Arquitetura / abordagem técnica
- Plugins são feitos **por fora do ERP**, porque mexer **dentro do ERP** é muito trabalhoso.
- Trabalham **via API SL**, mas respeitando **todos os guardrails da SL** para garantir segurança.

### 6. Plugin #1 — Monitorar contas de pagamento em débito automático
- Objetivo: **monitorar contas de pagamento em débito automático (DA)**.
- Permite **selecionar as contas contábeis** a serem monitoradas.
- ❓ **Pergunta em aberto:** como o plugin **descobre que uma conta é débito automático (DA)**?

### 7. Plugin #2 — Impostos PIS/COFINS/CSLL por condomínio
- Lista os impostos de **PIS / COFINS / CSLL** de cada condomínio.
- Objetivo: **bater/conferir com a guia do DARF**.

### 8. Plugin #3 — Relatório de saldos dos condomínios
- **Relatório de saldos** dos condomínios.
- Com **análise de variação no tempo**.

### 9. Infraestrutura / observação minha
- Alguns plugins usam um **banco de dados próprio**.
- 💭 **Hipótese (minha):** então o **Nexus é um app por si só** (?) — *confirmar*.

### 10. Autenticação / auditoria
- As pessoas **logam nos plugins com o próprio usuário SL**.
- Assim, **toda ação feita via plugins fica registrada no SL** como **auditoria**.

### 11. Paybox 2.0 (Fernanda)
- A **Fernanda** melhorou muito a ferramenta **Paybox**.
- Fez uma versão **"Paybox 2.0"** com **mais de 40 melhorias**.
- ⚠️ Ainda **não está liberada**.

### 12. Plugin #4 — Contas a pagar (visão analítica)
- **Reorganiza a tela de contas a pagar** com uma **visão mais analítica** de cada pagamento.
- Tem uma **facilidade de lançamento rápido**, como a do **Paybox**.

### 13. Plugin #5 — Dashboard de despesas
- **Dashboard de despesas** — plugin de **métricas de lançamento de contas a pagar**.
- Similar ao **nosso KPI Contas a Pagar**.

