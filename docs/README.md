# Git Branches e Tags

Branches
Os branches permitem que você trabalhe em diferentes versões de um projeto simultaneamente. Eles são úteis para desenvolver novas funcionalidades, corrigir bugs e experimentar sem afetar o branch principal (geralmente chamado de “main” ou “master”).

Criar um Novo Branch
Para criar um novo branch:

```bash
git checkout -b nome-do-branch
```

Listar Branches
Para listar todos os branches:

```bash
git branch
```

Alternar entre Branches
Para mudar para outro branch:

```bash
git checkout nome-do-branch
```

Unir Branches
Para unir um branch ao branch atual:

```bash
git merge nome-do-branch
```

Excluir um Branch
Para excluir um branch que não é mais necessário:

```bash
git branch -d nome-do-branch
```

## Git Tags

### As tags são utilizadas para marcar pontos específicos na história do repositório, como versões de lançamentos (releases). Tags são imutáveis e diferem dos branches, que podem ser modificados

Criar uma Tag Anotada
Tags anotadas são recomendadas porque armazenam mais informações, como a data, o autor e uma mensagem:

```bash
git tag -a v1.0.0 -m "Versão 1.0.0"
```

Criar uma Tag Leve
Tags leves são apenas marcadores simples:

```bash
git tag v1.0.0
```

Listar Tags
Para listar todas as tags no repositório:

```bash
git tag
```

Exibir Informações de uma Tag
Para ver detalhes de uma tag anotada:

```bash
git show v1.0.0
```

Compartilhar Tags com o Remoto

Por padrão, o git push não envia tags para o repositório remoto. Você precisa enviá-las explicitamente:

```bash
git push origin v1.0.0
```

Para enviar todas as tags de uma vez:

```bash
git push --tags
```

Excluir uma Tag
Para excluir uma tag localmente:

```bash
git tag -d v1.0.0
```

Para excluir uma tag no repositório remoto:

```bash
git push origin --delete tag v1.0.0
```

Fluxo de Trabalho com Branches e Tags
Criação de uma Nova Funcionalidade:
Crie um branch a partir do branch principal:

```bash
git checkout -b nova-funcionalidade
```

Desenvolva a funcionalidade, faça commits frequentemente e teste-a.
Quando estiver pronta, faça merge no branch principal:

```bash
git checkout main
```

```bash
git merge nova-funcionalidade
```

Correção de Bug:
Crie um branch de correção a partir do branch principal:

```bash
git checkout -b correcao-bug
```

Corrija o bug, faça commits frequentemente e teste a correção.
Quando estiver pronta, faça merge no branch principal:

```bash
git checkout main
```

```bash
git merge correcao-bug
```

Lançamento de uma Versão:
Crie uma tag anotada no branch principal:

```bash
git checkout main
```

```bash
git tag -a v1.0.0 -m "Versão 1.0.0"
```

Envie a tag para o repositório remoto:

```bash
git push origin v1.0.0
```

Conclusão
Seguindo esse exemplo, você pode gerenciar branches e tags de forma
eficiente em seus projetos Git. Mantenha seu fluxo de trabalho organizado e aproveite ao máximo essas ferramentas! 🚀
