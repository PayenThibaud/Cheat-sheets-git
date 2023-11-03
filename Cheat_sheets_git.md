# Commande pour git-github

## Commande  
  
git init = créer le .git du dossier  
git add (nom.txt) = Indexé un fichier  
git commit -m (mot) = Validation + Description des modif  
git status = voir où on en est  
  
## Créer une clé SSH  
  
ssh-keygen -t ed25519 -C "votre_email@example.com"  
Get-Content "C:\Users\Thibaud Payen\.ssh\id_ed25519.pub" | clip (Sur powershell)  
$ eval "$(ssh-agent -s)" = pour créer un agent SSH  
ssh-add ~/.ssh/id_ed25519 = mettre la clé privée SSH à l'agent  
  
## Synchronisation git-github  
  
Upstream (Github de quelqu'un) => fork (faire une copie prîvé) => origin (mon Github)  
Origin => git clone SSH => Local (ma machine)  
  
## Pour mettre à jour  
  
cd (dossier)  
git remote add upstream https (lecture) ou SSH (écriture) du fork (si pas déjà fait)  
git pull upstream main => Local (mettre à jour du fork au local)  
git push origin main => origin (mettre à jour le local à github)  
git remote -v (voir)  
git remote rm (surpprimer)  
  
## Les branches  
  
git branch = voir sur qu'elle branche on est  
git branch (nom nouvelle branche) = créer une branche  (locale)
git checkout (mot) = basculer de branche  
git switch (mot) = nouvelle façon de basculer de branche
Après avoir changer un fichier (git add + git commit)  
git push --set-upstream origin (nom de la nouvelle branche)  
git branch -d (nom) = supprimer une branche  
git branch -D (nom) = Supprimer une branche qui a déjà des changements  
  
### Fusion des branches  
  
Retourner sur la branches principale (git checkout)   
git merge (nom de la nouvelle branche)  
puis git push  
  
### Pull request  
  
Un remote  
Une nouvelle branche  
et le code dans la branche.  
Pull request sur Github.  
  
##
