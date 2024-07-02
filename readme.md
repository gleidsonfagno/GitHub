# Projeto git

## iniciando um repositorio

- git init

### configurar o git

- nome e email

- git config --global user.name "gledsonfagno"

- git config --global user.email "<usuarionome@gmail.com>"

### vai listar as configuraçoes

- git config --list

### fazer um commits

- git add . vai adicionar os aquivos recentes

- git commit -m "created redme.md" messagem que vai ficar na alterção

### ver os commits e as alteracoes

- git log

### uma forma mais resumida

- git log --oneline

### vai trazer a quantidades de commits que quiser nesse caso 3

- git log -n 3

### Git Status

### vai ferificar as alteraçoes

- git status

### estagios dos aquivios

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

- depois que executar o git add .
- git restore --staged .
vai pegar os aquivos que estao no stage e voltar para aquivos modificados
- working directory

### Corrigi o ultimo commit

se ja fez o commit so executar

- git commit --amend -m "corrigindo commit"

### Desfazer o último commit

depois de fazer o commit

- git reset --soft HEAD~1

### Git Push

```bash
git remote add origin https://github.com/gleidsonfagno/GitHub.git
git branch -M main
git push -u origin main
```

### Arquivo gitignore

ele e lido pelo github e tudo que estiver escrioto dentro dele e nao vai ser enviado para o reposditorio github.

### Gerar uma nova chave SSH

[GitHubDocs](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#about-ssh-key-passphrases
)

```bash

ssh-keygen -t ed25519 -C "your_email@example.com"
# assim que fica no terminal adiciona o eval no Enter file
Generating public/private ed25519 key pair.
Enter file in which to save the key (C:\Users\gleid/.ssh/id_ed25519): eval $(ssh-agent -s)

# remove 
Remove-Item -Force -Path C:\Users\gleid\.ssh\id_ed25519

adiciona a chave publica no repositorio a do arquivo .epub
```

### Gerenciando mudanças com git branches e git tags

Para mais informações, veja a [Documentação Detalhada](./docs/README.md).
