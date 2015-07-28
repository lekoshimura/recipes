# Anotações de How to Use Git and GitHub

- [Udacity: How to Use Git and GitHub](https://www.udacity.com/course/how-to-use-git-and-github--ud775)

```bash

# git está instaldo?
$ git --version
git version 1.9.1

#  Initializing a Repository
$ git init
# - Após a criação do repositório (=> do arquivo .git no diretório raíz do projeto), ainda não há commits.
# - O prompt só vai exibir o branch atual após o primeiro commit.

# Compare two commits, printing each line that is present in one but not the other:
$ git diff [id 1] [id 2] # sem os colchetes

# Compare working directory and stagin area
$ git diff

# Compare staging area and (the last commit on) the repository
$ git diff --staged

# Make a copy of a entire Git repository, including the history, onto yout computer:
$ git clone [url]

# Temporarily reset all files in a repository to their state at the time of a specific commit:
$ git chekcout [id do commit]

# para ver o diff com cores:
$ git config --global color.ui auto

# Show the commits made in a repository, starting with the most recent in the current branch:
$ git log

# Listar commits com gráfico de barras das alterações feitas (diffstat) :
$ git log --stat

# Viewing the commit history with visual representation:
$ git log --graph --oneline master coins

# Restore a commit to the working directory
$ git checkout [id do commit antigo]
You are in 'detached HEAD' state.
# - O quê acontece se você fizer alterações neste estado?
# - Como voltar ao commit mais recente?
#   $ git checkout master

# Recupera arquivos do repository. As diferenças no staging area e working directory são sobrescritas. CUIDADO: não há como recuperar as diferenças que foram sobrescritas!
$ git reset --hard

# Merge branch1 into the the currently checked-out
$ git merge branch1

# Restore your files to their state before you started the merge
$ git merge --abort

# Compare a commit to its parent. Useful when "git log" return commit sfrom several branches and you don´t know what is the parent commit of commit_id.
$ git show commit_id
```
