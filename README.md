# iniciando um repositório com Git (máquina local)

- pré-requisitos: ter o git instalado e abrir o terminal git bash
```bash
User@LAPTOP-DE-USER007MINGW64~
/*
User -> usuário
@LAPTOP-DE-USER007 -> nome do computador
MINGW64 -> programa usado pela git e é instalado por ele automaticamente
~ -> arquivo principal do usuário
*/
```
- para determinar o diretório atual, use o comando
```bash
$pwd
```
- caso seja sua primeira vez usando o git, primeiro configure-o com seu nome de usuário e endereço de e-mail, pois essa informação será usada nos commits que enviar
```bash
$ git config --global user.name "Nome do usuário"
$ git config --global user.email "seu@email.com"
```
- para listar os arquivos presentes no diretório
```bash
$ ls
```
- para abrir uma pasta
```bash
$ cd nome da pasta
```
- para rastrear o repositório indicado
```bash
git init
```
- O git mostrará o nome da branch principal que está em uso que, normalmente, se chama **master**.
    - **Nota**: Para garantir a compatibilidade no futuro é recomendado atualizar o nome da branch principal, de **master** para **main**, com o seguinte comando:
    
      ```c
      $ git branch -M main // comando usado para renomear uma branch
      ```
#comandos básicos mais utilizados para versionamento em git
- **git config:** primeiro comando a ser executado após a instalação. Usado para configurar seu nome e email que ficará vinculado às alterações
```jsx
$ git config --global user.name "Nome do usuário"
$ git config --global user.email "seu@email.com"
```
- **git init:** inicia ou cria um repositório
```jsx
$ git init
```
- **********************git status:********************** visualizar o estado do repositório
```jsx
$ git status
```
- ****************git add:**************** adiciona o conteúdo ao rastreio do git
```jsx
$ git add nome-do-arquivo //adiciona apenas o arquivo mencionado
$ git add . // adiciona todos os arquivos do projeto
```
- **********************git commit:********************** salva o conteúdo adicionado junto com uma mensagem de descrição das alterações
```jsx
$ git commit -m "descrição do commit"
```
- ********************git clone:******************** clona um repositório existente
```jsx
$ git clone [url] //ou
$ git clone [chave SSH]
```
- **********************git branch:********************** Uma branch nada mais é do que uma ramificação dentro do repositório. Este comando pode ser utilizado de diversas maneiras.
```jsx
$ git branch // mostra todas as branchs existentes em um repositório
$ git branch nome-da-branch // cria uma nova branch
$ git branch -M nome_da_branch // renomeia a branch atual
```
- ******************************************git checkout branch:****************************************** navegar entre as branches criadas no repositório
```jsx
$ git checkout 01-branch
Switched to branch '01-branch'
```
- ****************git log:**************** exibe um histórico de commits
```jsx
$ git log //ou
$ git log --oneline
```
- ****************git remote:**************** exibe o repositório remoto
```jsx
$ git remote
$ git remote -v
```
- ******************git pull:****************** atualiza o repositório local, com o conteúdo do repositório remoto
```jsx
$ git pull
```
- ******************git push:****************** envia o conteúdo do repositório local, atualizando o repositório remoto
```jsx
$ git push
```
