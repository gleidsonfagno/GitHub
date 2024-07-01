# Projeto git

## iniciando um repositorio

- git init

### configurar o git

- nome e email

- git config --global user.name "gledsonfagno"

- git config --global user.email "<usuarionome@gmail.com>"

#### vai listar as configuraçoes

- git config --list

### fazer um commits

- git add . vai adicionar os aquivos recentes

- git commit -m "created redme.md" messagem que vai ficar na alterção

### ver os commits e as alteracoes

- git log

#### uma forma mais resumida

- git log --oneline

#### vai trazer a quantidades de commits que quiser nesse caso 3

- git log -n 3

### Git Status

#### vai ferificar as alteraçoes

- git status

#### estagios dos aquivios

- working directory
- unstage
- log

### HEAD

- ele mostra  em que ponto da historio o projeto se encontra

### Git diff

- vai mostrar o que mudou
- git diff

### Desfazendo modificações

- git restore nome do aquivo /se for aquivo unico

- git restore . para todas as alteracoes

### Restaurando da Staged

- depois que execitar o git add .
- git restore --staged .
vai pegar os aquivos que estao no stage e voltar para aquivos modificados
- working directory

### Corrigi o ultimo commit

se ja fez o commit so executar

- git commit --amend -m "corrigindo commit"

### Desfazer o último commit
