# Git Workflow

## Objetivo

Documentar o fluxo Git oficial deste repositório para evitar regressões de autenticação e manter consistência entre contribuições.

## Configuração Atual

### Remote

O remoto `origin` deve usar **SSH**:

```bash
git@github.com:haulisson/SPICE-MNA.git
```

Não usar remoto HTTPS neste projeto.

### Autenticação

Este repositório usa autenticação por chave SSH:

- chave carregada no `ssh-agent`;
- comunicação com GitHub sem senha;
- sem uso de autenticação por usuário/senha em HTTPS.

Antes de operações de `push`, verificar se o agente SSH está ativo e se a chave correta está carregada.

Exemplos:

```bash
ssh-add -l
ssh -T git@github.com
```

## Política de Email de Commit

Para evitar bloqueios de privacidade do GitHub, os commits deste repositório devem usar o email noreply:

```bash
3450955+haulisson@users.noreply.github.com
```

Não usar email pessoal nos commits deste projeto.

Para conferir a configuração:

```bash
git config user.name
git config user.email
```

## Fluxo Padrão

Fluxo recomendado para alterações normais:

```bash
git add .
git commit -m "message"
git push
```

Como `main` já está configurada com upstream para `origin/main`, o `push` simples é suficiente após novos commits.

## Regras Operacionais

- manter `origin` em SSH;
- não trocar o remoto para HTTPS;
- verificar SSH antes de publicar;
- manter nome e email consistentes nos commits;
- evitar reinventar o fluxo quando o setup atual já funciona.

## Verificações Úteis

Ver o remoto atual:

```bash
git remote -v
```

Confirmar branch e tracking:

```bash
git branch -vv
```

Confirmar autenticação SSH:

```bash
ssh -T git@github.com
```

## Observação para Contribuidores

Se um estudante ou colaborador clonar este projeto em outra máquina, deve repetir apenas o essencial:

1. configurar uma chave SSH;
2. adicionar a chave ao GitHub;
3. carregar a chave no `ssh-agent`;
4. confirmar que o remoto está em SSH;
5. confirmar que o email de commit está correto antes de publicar.
