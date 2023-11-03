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
git remote add upstream https du fork (si pas déjà fait)  
git pull upstream main => Local (mettre à jour du fork au local)  
git push origin main => origin (mettre à jour le local à github)  
  
## Les branches  
  
git branch = voir sur qu'elle branche on est  
git branch (mot) = créer une branche  
git checkout (mot) = basculer de branche  




