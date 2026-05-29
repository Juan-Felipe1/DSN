# 🧰 SQUADS Toolbox — Referência Completa de Times Disponíveis

## Status Atual

| Squad | Status | Instalado | Versão |
|-------|--------|-----------|--------|
| **dispatch** | ✅ ATIVO | Sim | 1.0.0 |
| **design-testing** | ✅ ATIVO | Sim | 1.0.0 |
| apex | 📋 Disponível | Não | 1.0.0 |
| brand | 📋 Disponível | Não | 1.0.0 |
| curator | 📋 Disponível | Não | 1.0.0 |
| deep-research | 📋 Disponível | Não | 1.0.0 |
| education | 📋 Disponível | Não | 1.0.0 |
| kaizen | 📋 Disponível | Não | 1.0.0 |
| kaizen-v2 | 📋 Disponível | Não | 1.0.0+ |
| legal-analyst | 📋 Disponível | Não | 1.0.0 |
| seo | 📋 Disponível | Não | 1.0.0 |
| squad-creator | 📋 Disponível | Não | Built-in AIOX |
| squad-creator-pro | 📋 Disponível | Não | Pro upgrade |

---

## 📌 DISPATCH (Instalado ✅)

**Propósito:** Motor de execução paralela que economiza tokens em 43-58x

**Quando usar:**
- Decompor stories em tasks atômicas
- Executar múltiplas tarefas em paralelo (waves)
- Otimizar custos automaticamente
- Rotear para modelos certos (Haiku, Sonnet, Opus)

**Oferece:**
- 4 agentes orchestradores (chief, quality-gate, wave-planner, task-router)
- 31 scripts Python para otimização
- Quality gates automáticos
- Cost tracking e health scoring

**Entrada:** `@dispatch-chief` ou `/dispatch:agents:dispatch-chief`

---

## 🧪 DESIGN-TESTING (Instalado ✅)

**Propósito:** Comprehensive UI/UX testing — design, events, fluxos, clicks, forms, backend

**Quando usar:**
- Testes intensivos de design e interações
- Cobertura de eventos (click, hover, keydown, etc.)
- Fluxos de usuário (navegação, wizard, modais)
- Validação de formulários e campos
- Estados de controles (enabled/disabled, visible/hidden, loading)
- Integração com backend (API responses na UI)
- Regressão antes de release

**Oferece:**
- 10 agentes especializados (design-chief, 3 tier agents, 6 specialists)
- 60+ cenários de teste por tela
- Cobertura de 7 áreas: Design, Events, Flows, Forms, State, Backend, Combinations
- Saída em formato PASS/FAIL/N/A com severity badges
- Sign-off table para governança
- Event registry (30+ tipos de eventos)

**Entrada:** `@design-chief` ou `/design-testing:agents:design-chief`

**Exemplo de uso:**
```
@design-chief

Por favor teste a tela FrmTarefaDepositoLayoutSepara.
Ela tem: combo boxes, buttons, grid, mode switching.
Cubra: design, eventos, fluxos, estados, backend.
```

---

## 🎨 APEX (Frontend Intelligence)

**Propósito:** Autonomous frontend squad — design system, componentes, acessibilidade

**Quando usar:**
- Arquitetura de frontend
- Design system components
- Acessibilidade (a11y) reviews
- React/CSS/motion optimization
- Mobile cross-platform

**Oferece:**
- 20+ agentes especializados (frontend-arch, react-eng, mobile-eng, css-eng, a11y-eng, design-system-eng, etc.)
- Checklists de qualidade
- Exemplos e patterns

**Instalação:** `*download-squad apex` (quando pronto)

---

## 🎯 BRAND (Branding & Identity)

**Propósito:** Elite brand building — frameworks de 6 maiores branding experts

**Quando usar:**
- Brand strategy e positioning
- Brand guidelines criação
- Brand voice consistency
- Visual identity
- Messaging framework

**Oferece:**
- Agentes clonados de experts reais (Dan Mall, Pedro Valério, etc.)
- Battle-tested frameworks
- Brand methodology

**Instalação:** `*download-squad brand` (quando pronto)

---

## 📚 CURATOR (Content Curation)

**Propósito:** Curação de conteúdo automática e inteligente

**Quando usar:**
- Agregar conteúdo de múltiplas fontes
- Organizar por tópico/categoria
- Síntese de trending topics
- Newsletter automation
- Social media content selection

**Oferece:**
- Agentes de discovery
- Filtering e ranking
- Synthesis e formatting

**Instalação:** `*download-squad curator` (quando pronto)

---

## 🔬 DEEP-RESEARCH (Evidence-Based Research)

**Propósito:** Pipeline de 11 agentes para pesquisa rigorosa com auditoria de viés

**Quando usar:**
- Pesquisa acadêmica
- Competitive analysis
- Market research
- Due diligence
- Evidence synthesis com confidence levels

**Oferece:**
- 11 agentes especializados
- Bias auditing
- Confidence scoring
- Bibliography management

**Instalação:** `*download-squad deep-research` (quando pronto)

---

## 🎓 EDUCATION (Online Course Design)

**Propósito:** Transformar expertise em cursos online pedagogicamente sólidos

**Quando usar:**
- Criar cursos online
- Instructional design
- Learning path creation
- Assessment design
- Compliance (GDPR, accessibility)

**Oferece:**
- Agentes de course design
- Curriculum templates
- Legal compliance checks

**Instalação:** `*download-squad education` (quando pronto)

---

## 🔄 KAIZEN (Continuous Improvement)

**Propósito:** Squad que vigia e melhora continuamente todos os outros squads

**Quando usar:**
- Otimização de processos
- Quality improvement
- Performance monitoring
- Pattern learning

**Oferece:**
- Observadores automáticos
- Recomendações de melhoria

**Versões:**
- **kaizen** (v1) — base de observação
- **kaizen-v2** — com sensing diário + learning via forgetting curve

**Instalação:** `*download-squad kaizen` ou `*download-squad kaizen-v2`

---

## ⚖️ LEGAL-ANALYST (Legal Review)

**Propósito:** Análise legal automatizada

**Quando usar:**
- Document review
- Compliance checking
- Contract analysis
- Risk assessment
- Privacy/GDPR audit

**Oferece:**
- Agentes legais
- Compliance checklists

**Instalação:** `*download-squad legal-analyst` (quando pronto)

---

## 🔍 SEO (Search Engine Optimization)

**Propósito:** Post-design SEO optimization — avalia sites (0-100), otimiza todos os fatores

**Quando usar:**
- SEO audit
- On-page optimization
- Technical SEO
- Content optimization
- Competitive SEO analysis

**Oferece:**
- Agentes de SEO
- Score 0-100 com breakdown
- Before/after improvement tracking
- Like Yoast/RankMath but AI-powered

**Instalação:** `*download-squad seo` (quando pronto)

---

## 🏗️ SQUAD-CREATOR (Squad Factory)

**Propósito:** Cria novos squads customizados

**Quando usar:**
- Criar novo squad especializado
- Clonar squad existente
- Extend squad base com customizações
- Template squad design

**Oferece:**
- Squad generator
- Agent scaffolding
- Architecture guidance

**Status:** Incluído no AIOX base (não precisa instalar separadamente)

---

## 🚀 SQUAD-CREATOR-PRO (Squad Factory Pro)

**Propósito:** Upgrade pack que transforma Squad Creator em fábrica elite de squads

**Quando usar:**
- Criar squads de produção (não just experimento)
- Squads com múltiplas teams
- Squads com external integrations
- Publishing e sharing

**Oferece:**
- Advanced squad patterns
- Multi-team orchestration
- Publishing tools

**Status:** Upgrade pack (opcional sobre base squad-creator)

---

## 📋 Recomendação de Instalação Sequencial

### Fase 1 (Hoje ✅)
- ✅ dispatch — Motor de execução paralela

### Fase 2 (Conforme necessário)
**Escolha baseado em próxima prioridade:**
- **Se foco em frontend:** apex
- **Se foco em branding:** brand
- **Se foco em pesquisa:** deep-research
- **Se foco em criação de conteúdo:** curator
- **Se foco em cursos:** education
- **Se foco em legal/compliance:** legal-analyst
- **Se foco em SEO:** seo

### Fase 3 (Opcional)
- kaizen ou kaizen-v2 — observadores contínuos
- squad-creator-pro — se criar muitos squads

---

## 🔧 Como Instalar um Squad Novo

Quando pronto, execute:

```bash
cd C:\Users\DSV-07\Desktop\DSN

# Opção 1: via AIOX (recomendado)
*download-squad {squad-name}

# Opção 2: Manual (se acima não funcionar)
cp -r /tmp/aiox-squads/squads/{squad-name} squads/{squad-name}
python squads/dispatch/scripts/build-command-registry.py
python squads/dispatch/scripts/build-domain-registry.py
git add squads/{squad-name} .claude/settings.local.json
git commit -m "Add {squad-name} squad"
git push origin main
```

---

## 💡 Lógica de Lazy Loading

**Como funciona:**
- Todos os squads vivem em `squads/` (L4 mutable layer)
- `.aiox-core/core-config.yaml` tem `lazyLoading.heavySections: [squads]`
- Squads carregam **sob demanda** via `@squad-name-chief`
- Não pré-carregam — não contamina contexto

**Benefício:** Caixa de ferramentas completa, mas zero overhead!

---

## 📊 Comparativo Rápido

| Squad | Especialização | Agentes | Complexidade | Tokens | Tempo Setup |
|-------|---|---|---|---|---|
| dispatch | Execução paralela | 4 | Alta | - | 5 min ✅ |
| apex | Frontend | 20+ | Alta | ~2M | 15 min |
| brand | Branding | 8+ | Média | ~1.5M | 10 min |
| curator | Content | 6+ | Média | ~800K | 8 min |
| deep-research | Pesquisa | 11 | Muito Alta | ~2.5M | 20 min |
| education | Cursos | 7+ | Média | ~1.2M | 12 min |
| legal-analyst | Legal | 5+ | Média | ~1M | 8 min |
| seo | SEO | 6+ | Média | ~900K | 10 min |
| kaizen | Monitoramento | 4+ | Baixa | ~400K | 5 min |

---

## ✅ Checklist: Sua Caixa de Ferramentas

- ✅ Dispatch instalado e funcionando
- ✅ Lazy loading ativo (zero overhead)
- ✅ Documentação de 11 squads adicionais (este arquivo)
- ✅ Instruções de instalação para cada squad
- ⏳ Próximos: Instalar conforme necessário

**Próximo passo:** Testar dispatch com uma story simples!

---

*Documento criado em 2026-05-29 como referência de disponibilidade de squads.*
