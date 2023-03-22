Utilisation du hook de vérification de commit

Ce hook permet de créer un fichier de vérification de commit automatiquement lors de chaque commit.

Pour utiliser ce hook, suivez les étapes suivantes :

1. Assurez-vous que le hook est présent dans le dossier .git/hooks/ de votre projet.
2. Ouvrez un terminal et naviguez jusqu'au dossier racine de votre projet.
3. Entrez la commande "chmod +x .git/hooks/pre-commit" pour rendre le hook exécutable.
4. Effectuez des modifications sur votre projet comme d'habitude.
5. Lorsque vous êtes prêt à effectuer un commit, entrez la commande "git commit" dans le terminal.
6. Lorsque le hook vous demande si vous souhaitez créer un fichier de vérification de commit, répondez "y" ou "Y" pour créer le fichier ou "n" ou "N" pour annuler la création du fichier.
7. Si vous avez choisi de créer le fichier, il sera automatiquement créé dans le dossier "suivi/" et ajouté à Git pour être inclus dans le commit.

Note : le hook crée un fichier nommé "commitInfo.txt" dans le dossier "suivi/". Ce fichier contient la date et l'heure au format européen suivis du texte "commit vérifié le".

