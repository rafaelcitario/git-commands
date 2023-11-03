# Comandos importantes do Git

```
git init
```
* Este comando inicia um repositório em sua maquina.

```
git diff <Arquivo.extensão>
```
* Este comando mostra todas as modificações realizadas no arquivo.
```
git diff *
```
* Este comando mostra todas as modificações realizadas em todos os arquivos.

```
git add <Arquivo.extensão>
```
* Este comando adiciona o arquivo modificado ao "Stage".
* Arquivos no Stage, estão prontos para serem comitados.

```
git restore <Arquivo.extensão>
```
* Este comando deleta todas as modifações que você fez no arquivo.

```
git restore *
```
* Deleta todas as modificações que você realizou em todos os arquivos modificados.

```
git restore --staged <Arquivo.extensão>
```
* Este comando retorna um arquivo que estava em "Staged" para "Modificado".
Sendo necessario realizar ```git add <Arquivo.extensão>``` novamente para depois comitar.



