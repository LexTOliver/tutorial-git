# Tutorial de Git - Comandos Avançados

Este é um tutorial de Git que abrange alguns comandos avançados para ajudá-lo a aproveitar ao máximo o Git em seus projetos.

---
## Criando e Gerenciando Branches

As branches são essenciais no desenvolvimento de projetos colaborativos. Veja como criar e gerenciar branches:

### Criando uma nova branch

```bash
git branch nome_da_branch
```

Esse comando cria uma nova branch com o nome especificado, mas não muda para essa branch.

### Mudando para uma branch

```bash
git checkout nome_da_branch
```

Esse comando altera o branch atual para a branch especificada.

### Criando e mudando para uma nova branch

```bash
git checkout -b nome_da_branch
```

Esse comando cria uma nova branch com o nome especificado e imediatamente muda para essa branch.

### Listando todas as branches

```bash
git branch
```

Esse comando lista todas as branches existentes no repositório. A branch atual é destacada com um asterisco.


### Excluindo uma branch

```bash
git branch -d nome_da_branch
```

Esse comando exclui a branch especificada. Certifique-se de estar em outro branch antes de excluí-la.

---
## Trabalhando com Repositórios Remotos

O Git permite interagir com repositórios remotos para facilitar o trabalho em equipe e a colaboração.

### Clonando um repositório remoto

```bash
git clone url_do_repositorio
```

Esse comando cria uma cópia local de um repositório remoto em seu computador.

### Adicionando um repositório remoto

```bash
git remote add nome_remoto url_do_repositorio
```

Esse comando associa um nome (geralmente "origin") a um repositório remoto.

### Enviando commits para um repositório remoto

```bash
git push nome_remoto nome_branch
```

Esse comando envia seus commits locais para um repositório remoto específico.

### Obtendo alterações de um repositório remoto

```bash
git pull nome_remoto nome_branch
```

Esse comando obtém as alterações mais recentes de um repositório remoto e as mescla em sua branch local.

---
## Gerenciando Conflitos de Merge

Ao mesclar branches ou obter alterações de um repositório remoto, podem ocorrer conflitos. Veja como lidar com eles:

### Resolvendo conflitos de merge

Abra os arquivos com conflitos e edite-os manualmente para resolver as diferenças.

Após resolver os conflitos, adicione os arquivos modificados usando git add nome_do_arquivo.

Faça um novo commit para finalizar o processo de merge.

---
## Recursos Avançados
O Git oferece recursos avançados para lidar com casos específicos e fluxos de trabalho complexos. Aqui estão alguns deles:

### Rebase interativo

```bash
git rebase -i commit_referencia
```

Esse comando permite reorganizar, editar ou combinar commits antes deles serem adicionados ao histórico principal.

### Cherry-pick

```bash
git cherry-pick commit_referencia
```

Esse comando permite aplicar um commit específico a um branch diferente.

---
## Submódulos

Os submódulos permitem incluir outros repositórios Git como pastas em um repositório principal.

```
git submodule add url_do_repositorio
```

---
## Tags

As tags são referências estáticas para versões específicas do código em um repositório. Elas são úteis para marcar lançamentos estáveis.

```
git tag nome_da_tag
```

## Referências adicionais

Referências de tópicos na Documentaçã Git:

* Gerenciando Branches: <a href="https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell"> Git Branching</a>
* Trabalhando com repositórios remotos: <a href="https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes"> Working with remotes</a>
* Gerenciando conflitos de Merge: <a href="https://git-scm.com/book/en/v2/Git-Tools-Advanced-Merging"> Git tools - Advanced Merging</a>
* Rebase: <a href="https://git-scm.com/book/en/v2/Git-Branching-Rebasing">Git Branching - Rebase</a>
* Git cherry-pick: <a href="https://git-scm.com/docs/git-cherry-pick">git-cherry-pick</a>
* Submódulos: <a href="https://git-scm.com/book/en/v2/Git-Tools-Submodules">Git tools - Submodules</a>
* Tags: <a href="https://git-scm.com/book/en/v2/Git-Basics-Tagging">Git Basics - Tagging</a>