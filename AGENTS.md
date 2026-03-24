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

---

## Git Rules

- Usar somente remoto Git via SSH.
- Não usar remoto HTTPS para este projeto.
- Antes de enviar alterações, verificar se o `ssh-agent` está ativo e se a chave correta está carregada.
- Não usar email pessoal em commits deste repositório.
- Usar o email GitHub noreply configurado para o projeto: `3450955+haulisson@users.noreply.github.com`.
- Preservar o fluxo simples do repositório: `git add .`, `git commit -m "mensagem"`, `git push`.
- Não alterar a configuração atual de autenticação Git sem necessidade explícita.
