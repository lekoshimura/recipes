# Anotações de How to Use Git and GitHub

- [Udacity: How to Use Git and GitHub](https://www.udacity.com/course/how-to-use-git-and-github--ud775)

```bash

# git está instaldo?
$ git --version
git version 1.9.1

# Compare two commits, printing each line that is present in one but not the other:
$ git diff [id 1] [id 2] # sem os colchetes

# Make a copy of a entire Git repository, including the history, onto yout computer:
$ git clone [url]

# Temporarily reset all files in a repository to their state at the time of a specific commit:
$ git chekcout [id do commit]

# para ver o diff com cores:
$ git config --global color.ui auto

# Show the commits made in a repository, starting with the first:
$ git log

# Listar commits com gráfico de barras das alterações feitas (diffstat) :
$ git log --stat

# 
$ git checkout [id do commit antigo]
You are in 'detached HEAD' state.
# - O quê acontece se você fizer alterações neste estado?
# - Como voltar ao commit mais recente?
```
