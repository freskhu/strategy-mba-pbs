# Agente de IA para Exame de Estratégia

**Executive MBA — Porto Business School**
**Disciplina:** Estratégia (Professor Luís Filipe Reis)
**Autor:** Simão Curval Ferreira
**Ano:** 2026

## Sobre

Este repositório contém o trabalho de grupo da disciplina de Estratégia: um agente de inteligência artificial implementado como plugin para o Claude (Anthropic), capaz de auxiliar na preparação e resolução do exame final.

O exame vale 60% da nota final, dura 2 horas, e avalia a aplicação de frameworks estratégicos a 4 empresas reais.

## Estrutura

```
strategy-repo/
├── README.md                    # Este ficheiro
├── docs/
│   └── Agente-Estrategia-MBA-PBS.docx   # Documento formal do trabalho
├── exames-resolvidos/           # 7 casos pré-resolvidos
│   ├── DIGI.md
│   ├── NORS.md
│   ├── FRULACT.md
│   ├── SUPER-BOCK.md
│   ├── TEKEVER.md
│   ├── VISABEIRA.md
│   └── VISTA-ALEGRE.md
├── skills/                      # Código das 3 skills do agente
│   ├── strategy-exam-solver/
│   │   └── SKILL.md
│   ├── strategy-tutor/
│   │   └── SKILL.md
│   └── strategy-answer-validator/
│       └── SKILL.md
└── plugin/
    └── strategy-mba-pbs-v3.plugin   # Plugin instalável
```

## As 3 Skills

### 1. Strategy Exam Solver
Gera respostas completas no formato gold standard (Passo 1→2→3) para qualquer das 7 empresas. Opera em 3 modos: pré-resolver, adaptar no exame, e resolver questão individual.

### 2. Strategy Tutor
Tutor interativo com 4 modos: EXPLICA, QUIZ, LIGA (conexões entre frameworks), e CASO (aplica a empresa real).

### 3. Strategy Answer Validator
Auditor que avalia respostas contra 5 dimensões: Formato (25%), Dados (25%), Frameworks (25%), Tipo de Questão (15%), e Terminologia (10%).

## Frameworks Integrados

34 frameworks documentados incluindo: PESTEL, Porter+ (7 forças), Estratégias Genéricas (Curva U/Deep Shit Valley), VRIN/VRIO, BCG (Ciclo do Dinheiro), McKinsey 7S, Teia Cultural, CAGE, Ansoff, Modos de Entrada, M&A, Ashridge, Cadeia de Valor, SWOT, entre outros.

## Como Instalar o Plugin

1. Abrir Claude Desktop
2. Entrar em modo Cowork
3. Menu > Customize > Upload plugin
4. Selecionar `plugin/strategy-mba-pbs-v3.plugin`
5. Confirmar instalação

## Como Usar no Exame

1. Abrir sessão Cowork com o plugin instalado
2. Colar/fotografar os enunciados das 4 empresas
3. O agente lança 4 agentes em paralelo (1 por empresa)
4. Cada agente gera ficheiro completo com respostas em formato Passo 1/2/3
5. Consultar ficheiros pré-resolvidos como referência complementar
6. Ajustar e submeter

## Terminologia do Professor

O agente usa exclusivamente a terminologia do Professor Luís Filipe Reis:
- **Porter+** (nunca "5 Forças")
- **Deep Shit Valley** (nunca "stuck in the middle")
- **Key Drivers for Change**, **Headwinds/Tailwinds**
- **Ciclo do Dinheiro**, **Joia da Coroa**
- **Teste do Algodão** (Gary Hamel)
- **Arquitetura Financeira**, **Boca do Crocodilo**
