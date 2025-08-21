# 📌 Comandos Essenciais do Git (Guia Rápido para Júnior)

### Iniciar repositório

```bash
git init
```

Inicia um novo repositório Git local na pasta atual. Cria a pasta oculta `.git/`.

---

### Ver diferenças

```bash
git diff <arquivo.extensão>
```

Mostra as modificações realizadas em **um arquivo específico** que ainda não foram adicionadas ao *stage*.

```bash
git diff
```

Mostra todas as modificações realizadas em todos os arquivos **ainda não adicionados ao stage**.

```bash
git diff --staged
```

Mostra as modificações que já foram adicionadas ao *stage* e ainda não foram commitadas.

```bash
git diff origin/<branch>
```

Compara seu código local com a branch remota informada.

---

### Adicionar arquivos ao Stage

```bash
git add <arquivo.extensão>
```

Adiciona o arquivo ao *stage*. Arquivos no stage estão prontos para serem commitados.

```bash
git add .
```

Adiciona **todos os arquivos modificados** ao *stage*.

---

### Descartar mudanças

```bash
git restore <arquivo.extensão>
```

Descarta todas as modificações feitas em um arquivo que **ainda não foi adicionado ao stage**.

```bash
git restore .
```

Descarta modificações em **todos os arquivos não stageados**.

```bash
git restore --staged <arquivo.extensão>
```

Remove o arquivo do *stage*, voltando ao estado de **modificado**.

---

### Commitar mudanças

```bash
git commit -m "Mensagem do commit"
```

Registra as alterações adicionadas ao *stage* com uma mensagem descritiva.

```bash
git commit -am "Mensagem"
```

Adiciona **e** commita arquivos que já estavam sendo rastreados (não pega arquivos novos).

---

### Atualizar repositório local

```bash
git pull
```

Baixa e mescla automaticamente alterações do repositório remoto para o local.

```bash
git fetch
```

Baixa as alterações do repositório remoto, mas não mescla.
Útil para inspecionar antes de aplicar, junto com `git diff`.

---

### Trabalhando com Branches

```bash
git branch <nome-da-branch>
```

Cria uma nova branch.

```bash
git checkout <nome-da-branch>
```

Troca para a branch desejada.

```bash
git checkout -b <nome-da-branch>
```

Cria e já troca para a nova branch.

```bash
git branch --list
```

Lista todas as branches locais.

```bash
git branch -d <nome-da-branch>
```

Deleta uma branch local já mesclada.

```bash
git push origin --delete <nome-da-branch>
```

Deleta uma branch remota.

---

### Histórico de commits

```bash
git log
```

Lista todos os commits.

```bash
git log --oneline
```

Lista commits de forma resumida em uma linha.

```bash
git log --graph --oneline --decorate
```

Mostra histórico com visualização gráfica de branches.

---

### Reverter alterações

```bash
git revert <hash>
```

Cria um novo commit que desfaz as alterações de um commit específico.

```bash
git reset --soft <hash>
```

Volta o histórico até um commit, **mantendo alterações no stage**.

```bash
git reset --mixed <hash>
```

Volta o histórico até um commit, **mantendo alterações no diretório de trabalho** (estado "modificado").

```bash
git reset --hard <hash>
```

Volta ao commit escolhido **apagando todas as alterações posteriores** (cuidado!).

---

### Quem mudou o quê?

```bash
git blame <arquivo.extensão>
```

Mostra linha a linha quem fez cada alteração em um arquivo.

---

### Enviar alterações para o remoto

```bash
git push origin <branch>
```

Envia commits da branch local para a branch remota.

```bash
git push -u origin <branch>
```

Envia commits e **configura a branch remota como padrão** para futuros push/pull.

---

### Clonar repositório

```bash
git clone <url>
```

Copia um repositório remoto para sua máquina.

---

### Status do repositório

```bash
git status
```

Mostra a situação atual dos arquivos (modificados, stageados, não rastreados).

---

# ⚡ Resumo de sobrevivência

1. `git status` → sempre olhe antes de agir.
2. `git add .` + `git commit -m "msg"` → salvar mudanças.
3. `git pull` → atualizar.
4. `git push` → enviar.
5. Trabalhe em branches → nunca faça tudo na `main`.

---
