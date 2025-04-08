# ![Formation GoLogic Example de Projet](Gologic.png)

## Pré-requis pour exemple de projet 

Nous sommes ravis d'explorer GitHub Copilot avec vous à travers des exemples pratiques. Pour assurer le bon déroulement, veuillez préparer votre poste de travail de la manière suivante :

- Installer le plugin SonarLint
  -   **Visual Studio Code** : Ouvrir VSCode, Ctrl+Shift+X, saisir "SonarQube for IDE" dans la barre de recherche, cliquer sur "Install".

## Démarrer l'application

- Ouvrir VSCode et ouvrir une nouvelle fenêtre (Ctrl+Shift+N).
- Dans l'accueil, cliquer sur "Clone Git Repository...", entrer l'URL de ce dépôt (à savoir : [https://github.com/Nordic-Structures/Exemple-FastApi-Mongo-GHCopilot.git](https://github.com/Nordic-Structures/Exemple-FastApi-Mongo-GHCopilot.git)) et confirmer en cliquant sur "Clone from the URL". Cliquer sur "Open".
- Une fois le projet ouvert, ouvrir un nouveau terminal (Shift+Ctrl+\`). Installer l'environnement :
  - `conda env create -f env.yml`
Une fois que l'environnement est créé, définir l'interpréteur python pour le projet :
  - Ouvrir le fichier `./src/__init__.py`.
  - Cliquer sur "Select Interpreter" en bas à droite de la fenêtre.
  - Choisir "Python 3.11.11 ('gologic')" dans la liste qui vient d'apparaître au milieu de la fenêtre.
- Exécuter les commandes :
  - `conda activate gologic`
  - `uv run uvicorn --app-dir ./src/ api:app --reload`
- Validez que l'application fonctionne en allant à `http://127.0.0.1:8000/docs` ou `localhost:8080/docs`

Félicitations, l'application devrait bien être partie !
