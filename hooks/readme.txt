Hook Git : pre-commit

Ce hook permet de demander à l'utilisateur s'il veut enregistrer une trace du commit.

Fonctionnement :
- Le hook demande si l'on souhaite enregistrer un message de vérification.
- Si la réponse est 'y', il crée un fichier 'suivi/commitInfo.txt' avec la date et l'heure.
- Ce fichier est automatiquement ajouté au commit.

Installation :
Copier le fichier 'pre-commit' dans le dossier '.git/hooks/' de votre dépôt local :
   cp hooks/pre-commit .git/hooks/