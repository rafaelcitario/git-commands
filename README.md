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
git diff origin/<branch>
```
* Este comando mostra todas as modificações realizadas na brunch selecionada.

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
* Sendo necessario realizar ```git add <Arquivo.extensão>``` novamente para depois comitar.

```
git pull
```
* Este comando atualiza AUTOMATICAMENTE seus arquivos locais, com o que foi adicionado em seu repositório na nuvem ( GitHub ).
  
```
git fetch 
```
* Este comando realiza o download de todos os arquivos modificados que estão atualmente em seu repositório na nuvem ( Github ) para sua maquina.
* Este comando não é igual a ```git pull```, após o uso deste comando, você pode utilizar ```git diff origin/<branch>``` para visualizar quais modificações estão faltando no arquivo atual localizado em sua maquina.

```
git branch <Nome da nova Branch>
```
* Este comando cria uma nova branch.
* Apos a criação da nova branch você continua na branch atual. Para mover-se a nova branch utilize ```git checkout <Nome da Branch desejada```.

```
git branch --list
```
* Este comando lista todas as branches existentes

```
git branch -d <Nome da Branch>
```
* Este comando deleta a branch desejada.

```
git checkout <Nome da Branch desejada>
```
* Este comando seleciona a branch que você deseja utilizar.

```
git log
```
* Este comando retorna todas modificações adicionadas ```git add``` e commitadas ```git commit```.
* Você pode modificar a forma de visualização do conteúdo retornado utilizando ```git log --oneline```. Esta opção retorna o conteúdo em apenas uma unica linha.