# AGENTS.md

## Objetivo do Projeto
Criar um repositório educacional em Quarto para estudo da teoria de MNA aplicada a simuladores SPICE.

O conteúdo deve ser:
- técnico
- incremental
- reutilizável como apostila
- aberto (CC BY-NC-SA 4.0)

---

## Regras Gerais

1. Não implementar código arbitrário.
2. Foco em documentação estruturada e didática.
3. Todo conteúdo deve ser modular, em arquivos `.qmd` independentes.
4. Sempre usar MathJax para fórmulas.
5. Diagramas devem ser feitos com Mermaid.

---

## Execução com Planos

Sempre usar `PLANS.md` para qualquer tarefa complexa.

Nenhuma implementação deve começar sem:
- milestone definida
- critério de aceitação claro

---

## Estrutura de Conteúdo

Cada tópico deve conter:

- Intuição
- Formulação matemática
- Derivação
- Aplicação em SPICE
- Exemplo resolvido
- Possível implementação

---

## Regras de Remanufatura

- `upstream/` é somente leitura
- Não copiar código de SPICE
- Extrair apenas:
  - arquitetura
  - conceitos
  - padrões

---

## Estilo

Baseado em:
<https://mickael.canouil.fr/posts/2023-03-12-quarto-mathjax-packages/>

- uso intensivo de LaTeX
- organização limpa
- foco em legibilidade

---

## Licença

Todo conteúdo deve incluir:

CC BY-NC-SA 4.0
