# Profil développeur

Ce projet affiche une description professionelle, en listant les compétences de la personne et diverses informations pertinentes.  

## Notions

- Composables : décorateur `@Composable`, permet à une fonction d'être réutilisée
- Paramètres : arguments des fonctions composables, pour personnaliser un composable
- Modifiers : paramètre de type `Modifier` sur les composables, pour personnaliser l'affichage
- Padding : méthode `.padding()` de `Modifier`, pour ajouter des marges autour du contenu des composables (padding externe = padding autour du composable principal, padding interne = padding dans un composable)
- Callbacks : fonction passée en argument d'un composable pour qu'il l'appelle (par exemple `onClick` pour passer une fonction à bouton, appelée à chaque clic sur le bouton)
- Previews : configurations de test
- Accessibilité : role `modifier.clickable(role = Role.Button)` et `modifier.semantics { contentDescription = ... }`

## Explication

1. `Header`, `SkillItem`, `Skills`, `GitHubButton`, `PhoneNumber`, `Profile`
2. `Profile`
3. `MePreview`, `JohnDoePreview`
4. `PhoneNumber`
5. `GitHubButton`
6. `GitHubButton`: `role = Role.button` et `modifier.semantics { contentDescription = ... }`
7. Ils sont isolés et configurables

![./screen.png](./screen.png)
