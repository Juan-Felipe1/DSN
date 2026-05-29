# Dispatch Squad Test Guide

## 🚀 Como Testar o Dispatch

### Step 1: Ativar o Dispatch Chief

Digite um dos seguintes comandos:

```bash
@dispatch-chief
```

ou

```bash
/dispatch:agents:dispatch-chief
```

---

### Step 2: Passar a Story

Cole a story de teste ou a leia:

**Opção A - Usar a story de teste:**
```
Leia o arquivo: docs/dispatch-test-story.md
```

**Opção B - Usar a story em texto livre:**
```
Preciso que você:
1. Crie um documento técnico com seções de summary, instalação, exemplos e troubleshooting
2. Resume deve ter 2 parágrafos
3. Instalação deve ser step-by-step
4. Exemplos: 3 exemplos de código
5. Troubleshooting: 5 problemas comuns e soluções

Você pode usar Haiku para tasks bem definidas (summary, instalação, exemplos) e Sonnet para troubleshooting que precisa de julgamento.
```

---

### Step 3: O que esperar

Dispatch vai:

1. **Sufficiency Gate (QG-SUFF)** → Validar se a story é clara
2. **Plan Execution** → Decompor em tasks atômicas
3. **Wave Optimizer** → Organizar em waves paralelas
4. **Pre-Execution Gate (QG-PRE)** → Validar cada task
5. **Execute Waves** → Rodar em paralelo
6. **Post-Execution Gate (QG-POST)** → Validar outputs
7. **Generate Report** → Mostrar resultados + custo

---

### Step 4: Observe

**Você vai ver:**

- ✅ **Execution Plan** - Como dispatch decompos a story
- 📊 **Wave Manifest** - Quais tasks rodam em paralelo
- 🔍 **Model Selection** - Por que cada task usa Haiku/Sonnet
- ⏱️ **Timeouts** - Quanto tempo cada wave vai levar
- 💰 **Cost Estimate** - Quanto vai custar

**Durante execução:**
- Cada subagent vai executar sua task
- Você verá outputs em tempo real
- Quality gates validam resultados

**Após execução:**
- 📈 **Execution Report** - Tudo que foi feito
- 💵 **Cost Report** - Custo real vs. estimado
- ⚕️ **Health Score** - Score de 0-100 da execução

---

## 🎯 Métricas para Validar

| Métrica | Esperado | O que significa |
|---------|----------|-----------------|
| **Waves** | 2+ | Execução paralela funcionando |
| **Haiku tasks** | 3+ | Modelo certo para tasks simples |
| **Sonnet tasks** | 1+ | Modelo certo para tasks com julgamento |
| **Cost** | ~$0.03-0.05 | 43-58x mais barato que contexto principal |
| **Health Score** | 80+ | Execução saudável |
| **Quality Gates** | 100% pass | Sem erros de validação |

---

## 🐛 Se algo der errado

**Erro: "Story não é suficientemente clara"**
- Dispatch vai pedir clarificação
- Adicione mais detalhes e tente novamente

**Erro: "Task não foi validada"**
- Quality gate detectou problema
- Dispatch sugere fix automático (auto-fix-veto.py)

**Erro: "Subagent falhou"**
- Log de falha criado
- Dispatch tenta retry (até 3 vezes)
- Se falhar, mostra qual task falhou

---

## 📊 Output Esperado

Após sucesso, você terá em `_temp/dispatch/runs/{run_id}/`:

```
├── execution-plan.yaml      (Plano completo)
├── wave-manifest.yaml       (Manifesto de waves)
├── execution-report.md      (Relatório de execução)
├── cost-report.md           (Breakdown de custos)
├── dispatch-state.json      (Estado final)
└── task-outputs/
    ├── summary.md
    ├── installation.md
    ├── examples.md
    └── troubleshooting.md
```

---

## ✅ Checklist de Teste

- [ ] Dispatch chief ativa corretamente
- [ ] Story é aceita (passa sufficiency gate)
- [ ] Plano é criado com 3+ tasks
- [ ] Waves são otimizadas (2+ waves)
- [ ] Modelos selecionados corretamente
- [ ] Execução completa sem erros
- [ ] Quality gates passam 100%
- [ ] Relatório gerado com custo
- [ ] Health score > 80
- [ ] Outputs estão em _temp/dispatch/

---

## 🎓 7 Immutable Laws em Ação

Você vai ver esses princípios funcionando:

1. **LAW #0: NEVER MAIN CONTEXT** → Todo trabalho via subagents (zero pollution)
2. **LAW #1: CODE > LLM** → Scripts fazem roteamento (não LLM)
3. **LAW #2: RIGHT MODEL** → Haiku para bem-definido, Sonnet para julgamento
4. **LAW #3: STORY-DRIVEN** → Tudo começa com a story
5. **LAW #4: SLASH COMMAND MAP** → Dispatch sabe todos os /commands
6. **LAW #5: WAVE OPTIMIZED** → DAG topológico = máximo paralelismo
7. **LAW #6: OPTIMIZE EVERYTHING** → Decide Worker vs Agent vs Hybrid

---

**Pronto para testar? Invoque:** `@dispatch-chief`
