# Cheat sheets commit  
  
## Forme du commit  
  
Type: description  
  
description + d'info  
  
Pied de page (Reviewed-by: ... , refs: ... etc...)  
  
## Les types  
  
fix: corrige un bug dans le code.
feat: Nouvelle fonction dans le code.
BREAKING CHANGE: Rupture de compatibilité dans l'API.
build:
chore:
docs:
style:
refactor:
perf:
test:
  
## Exemple  
  
feat!: send an email to the customer when a product is shipped  
  
  

fix: prevent racing of requests

Introduce a request id and a reference to latest request. Dismiss
incoming responses other than from latest request.

Remove timeouts which were used to mitigate the racing issue but are
obsolete now.

Reviewed-by: Z
Refs: #123