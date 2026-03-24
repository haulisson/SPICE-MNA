# PLANS.md

## ExecPlan: Quarto MNA Study System

Este plano organiza a execução incremental do repositório Quarto para estudo de MNA.

---

## Objetivo

Criar um sistema de documentação em Quarto que permita:

- estudar MNA do zero ao avançado
- servir como base para implementação de simulador SPICE
- funcionar como apostila pública

---

## Milestone 1 - Setup do Quarto

### Entregáveis

- `_quarto.yml`
- estrutura inicial
- página `index.qmd`
- validação da configuração Git antes de operações maiores

### Critério de Aceitação

- `quarto render` gera site navegável
- configuração Git validada antes de operações maiores de publicação ou sincronização

### Riscos

- configuração incorreta de MathJax

### Dependências

- Quarto instalado

### Checkpoint

- [ ] Validate Git configuration before major operations

---

## Milestone 2 - Fundamentos de MNA

### Entregáveis

- `intro.qmd`
- definição de MNA
- equações nodais

### Critério de Aceitação

- documento explica MNA sem código

### Riscos

- excesso de formalismo

---

## Milestone 3 - Stamping

### Entregáveis

- `stamping.qmd`
- regras para:
  - resistor
  - fonte de corrente
  - fonte de tensão

### Critério de Aceitação

- leitor consegue montar a matriz MNA manualmente

### Riscos

- inconsistência matemática

---

## Milestone 4 - Exemplos

### Entregáveis

- `examples.qmd`
- circuitos resolvidos

### Critério de Aceitação

- exemplos completos com solução

---

## Milestone 5 - Numérico

### Entregáveis

- `numerical.qmd`
- métodos:
  - LU
  - pivotamento

### Critério de Aceitação

- ligação clara com SPICE

---

## Milestone 6 - Publicação

### Entregáveis

- GitHub Pages ativo
- licença aplicada

### Critério de Aceitação

- site público funcionando
