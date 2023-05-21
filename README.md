# Curso digital: GIT/Versionamentos

## Salvando alterações no repositório
* comando git push
    - `git push origin <branch>` 
        -> envia as alterações para o repositório remoto

* comando git add
    - `git add <file>` 
        -> adiciona o arquivo para ser commitado

    - `git add .` 
        -> adiciona todos os arquivos para serem commitados

* comando git pull
    - `git pull origin <branch>`
        -> puxa as alterações do repositório remoto

* comando git fetch 
        -> puxa as alterações do repositório remoto


## Branches
* comando git branch
    - `git branch -D <branch>` 
        -> deleta a branch mesmo que ela não tenha sido mergeada
    - `git branch -d <branch>`
        -> só deleta se ela já foi mergeada

* comando git checkout
    - `git checkout <branch>` 
        -> muda para a branch especificada
    - `git checkout -b <branch>`
        -> cria uma nova branch e muda para ela
    - `git checkout -B <branch>`
        -> força a criação de uma nova branch

* comando git merge
    - `git merge <branch> --no-ff`
        --no-ff -> não faz o fast-forward
        --ff -> faz o fast-forward
        --squash -> junta todos os commits em um só
        --abort -> cancela o merge

* comando git rebase
    - `git rebase <branch>`
        --continue -> continua o rebase
        --abort -> cancela o rebase
        --skip -> pula o commit atual

* comando git log
    - `git log --graph --oneline --decorate --all`
        -> mostra o log de forma gráfica


## Stash
* comando git stash
    - `git stash`
        -> salva as alterações em um stash
    - `git stash list`
        -> mostra a lista de stashes
    - `git stash apply`
        -> aplica o último stash
    - `git stash apply stash@{<numero do stash>}`
        -> aplica o stash especificado
    - `git stash drop`
        -> deleta o último stash
    - `git stash drop stash@{<numero do stash>}`
        -> deleta o stash especificado
    - `git stash pop`
        -> aplica o último stash e o deleta
    - `git stash pop stash@{<numero do stash>}`
        -> aplica o stash especificado e o deleta
    - `git stash clear`
        -> deleta todos os stashes

