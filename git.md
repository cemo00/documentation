# Documentation GIT

`git init`
A faire à la racine du projet pour initiatliser le projet

`git status`
Donne les infos sur les modifications

`git diff`
Liste les différents fichiers modifiés

`git add <fichier>`
Indexe les modifications du fichier donné

`git add .`
Indexe toutes les modifications

`Git commit -m"message"`
Commit les modifications indexées avec le message donné
Possibilité d’ajouter #x au début du message pour faire référence à l’issue x

`git log`
Affiche la liste des commit précédent le tag HEAD (HEAD est le commit courant)

`git log -n X`
Affiche les X derniers commit

`git log <branche>`
Affiche les commit de la branche donnée

`Git show <sha-1>`
Affiche le diff du commit donné

`git checkout <sha-1>`
Se positionne sur le commit donné

`Git checkout <branche>`
Se positionne sur la branche donnée

`Git checkout <tag>`
Se positionne sur le commit attaché au tag donné

`git tag <nom>`
Place un tag sur le commit courant

`git tag —delete <nom>`
Supprime le tag

`Git tag`
Liste l’ensemble des tags

`git clone <htttps://url> <dossier> `
Clone le dépôt distant dans le dossier indiqué

`git remote -v`
Affiche la liste des remotes

`Git push -u <remote> <branche>`
Pousse la branche donnée sur le remote donné

`git push <remote> <tag>`
pousse le tag donné sur le remote donné

`git push —tags`
pousse tous les tags sur le remote courant

`git fetch`
Récupère les informations sur le dépôt

`git pull`
Applique les modifications récupérées par le git fetch

`git blame <fichier>`
Donne des informations sur le contenu d’un fichier

`git stash save "<message>"`
met de côté les modifications

`git stash list`
Affiche la liste des stash

`git stash show X`
Affiche le stash d’index X

`git pull —rebase`

`git branch <nom>`
Créé une branche sur le local à partir du dernier commit avec le nom donné

`git branch`
Affiche la liste des branches

`git push —set-upstream <remote> <branche>`
pousse la branche donnée sur le dépôt donné

`git branch -a`
affiche la liste des branches locales et distantes

`git cherry-pick <sha-1>`
`git cherry-pick <tag>`
Duplique le commit donné sur la branche courante

`git merge <branche>`
Merge la branché donnée dans la branche courante

`Git rebase <branche>`
Rebase la branche courante sur la branche donnée

`git branch -d <branche>`
Supprime la branche en local

`git push <remote> —delete <branche>`
Supprime la branche sur le remote
