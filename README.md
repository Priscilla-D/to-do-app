# Todo app

## Objectif

Le but est de créer une application gestionnaire de tâches (to-do app). L'utilisateur pourra ajouter, supprimer une tâche ou encore la marquer en tant que "faite".

La solution retenue pour le style est libre (css, scss, styled-components, tailwind, ...).

--------

### **Faire l'exercice dans un repository git et commit à la fin de chaque étape des consignes**

--------

## Consignes

1. Créer une application React vierge avec la commande suivante : `yarn create react-app my-app --template typescript`. Copier ce fichier (*README.md*) à la racine du projet. *Commiter.*
2. Créer un composant pour afficher une tâche. Celui-ci devra comporter un titre et une checkbox pour savoir si la tâche est faite ou pas. *Commiter.*
3. Créer un composant de liste pour afficher la liste des tâches. Utiliser des fausses données temporaires pour générer la liste. *Commiter.*
4. Créer un composant qui servira à créer une tâche avec un input de type "text" et un bouton pour créer la tâche. *Commiter.*
5. Sur la page principale, afficher le formulaire puis la liste des tâches en dessous. Lorsque j'ajoute une tâche via le formulaire, ma liste de tâches est mise à jour. *Commiter.*
6. Faire en sorte que l'utilisateur ne puisse pas ajouter une tâche qui a un titre de moins de 4 caractères. *Commiter.*
7. Lorsqu'une tâche est notée "Terminée", le titre de celle-ci doit être barré. *Commiter.*
8. Pour chaque tâche, ajouter un bouton qui permet de supprimer la tâche (supprimer != "marquer en terminé"). *Commiter.*
9. Consommer l'API JSONPlaceholder pour récupérer une liste de tâches : **fetcher** la liste des todos depuis cette route `https://jsonplaceholder.typicode.com/todos` puis les afficher. *Commiter.*
10. Entre le formulaire d'ajout et la liste, ajouter un filtre sous forme de checkbox qui permettra de n'afficher que les tâches non-terminées. *Commiter et pusher.*

### 🎉 Félicitations, c'est terminé ! 🎉

## Ressources

- Les tâches auront la structure suivante :
```ts
  interface Task {
    userId: number; // id de l'utilisateur
    id: number; // id incrémental de la tâche
    title: string;
    completed: boolean;
  }
```
- [Documentation pour créer une app React](https://create-react-app.dev/docs/adding-typescript/)
- [Documentation de l'API](https://jsonplaceholder.typicode.com/)