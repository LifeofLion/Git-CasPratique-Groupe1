# CasPratique : *Versioning avec Git et GitHub*

### Modalités

Durée : 1h30

Ce TP est à faire par groupes de 3. Dans les rares cas où vous ne seriez que 2, l'intégralité du TP est à réaliser, mais vous pouvez vous répartir les tâches de l'élève n°3. 

### Livrables

Le seul livrable attendu est **l'URL du repo GitHub de travail** uniquement. Cette URL est à déposer sur MyGES dans les délais de rendu du TP. Le repo GitHub doit être public.

### Ressources autorisées

Vous avez accès à toutes les ressources fournies en cours (supports PDF, cheat sheet, etc.). Vous n'avez **pas** l'autorisation d'utiliser des LLMS et IAs génératives (ChatGPT, Copilot, etc.) pour trouver les commandes à utiliser. Vous n'avez également pas le droit de communiquer avec les étudiants des autres groupes.

# Instructions

## Règles de nomenclature

Afin d'identifier votre travail, vos **branches** doivent respecter la nomenclature suivante : `branch/<nom-de-l'élève>`. Par exemple, `branch/Jane-Doe`.

Afin de structurer vos commits, vous devez respecter la nomenclature de commits suivante :
- `feat/<nom-de-l'élève>: <description de la modification>` pour les modifications principales avec nom-de-l'élève étant l'élève qui a fait la modification
- `merge/<nom-de-l'élève>: merge de <source> vers <destination>` pour les merge, avec `<source>` étant le nom de la branche source, et `<destination>` celui de la branche vers laquelle le merge est effectué

Si vous ne souhaitez pas mettre vos noms complets dans les commits et les noms de branches, vous pouvez utiliser seulement votre prénom (s'il n'y a pas de doppelganger dans votre groupe) ou votre pseudo GitHub. Vous devrez rajouter dans le livrable de rendu les associations entre vos pseudos GitHub et vos noms réels.

## Démarrage

- Un élève du groupe fait un fork du repository https://github.com/SarahSch19/Git-CasPratique. Le nom du repo doit contenir le numéro de votre groupe, par exemple `Git-CasPratique-G1`.
- Il ajoute les deux autres ainsi que l'enseigante (`SarahSch19`) en tant que collaborateurs
- Chacun fait une copie en local du repo forké
- Chacun crée sa branche individuelle à partir de l'état initial du repository et la publie sur GitHub

- Chaque élève aura une Modification à faire (création, mise à jour d'un fichier).

### Ana
  - Modification : Créer un fichier index.html avec du contenu HTML simple

### Ayoub
  - Modification : Créer un fichier index.html avec du contenu HTML différent d'Ana

### Léo
  - Faire une modification dans le fichier README.md pour remplacer son contenu par les noms des contributeurs
    - Spécifier quel élève fait quelle partie (`Elève 1 = Jane Doe`, etc.)

S'il n'y a pas de troisième élève, ces tâches sont à répartir entre les deux élèves présents.

### Mise en commun
Dans l'étape suivante, résoudre tous les éventuels conflits qui adviennent. Si un conflit advient, le mentionner dans la description du commit (pas l'intitulé mais la description)
  - Ana : fusionner la branche de Ayoub 2 avec sa branche via un merge sans fast-forward
  - Ayoub : fusionner la branche de Léo avec sa branche via un merge avec fast-forward
  - Léo : lorsque Ana et Ayoub ont fini et publié leurs merges, récupérer les deux branches, et les rebase sur la sienne dans l'ordre suivant : branche d'Ana puis branche de Ayoub

Une fois ces trois étapes effectuées, sur GitHub :
  - Léo : créer une Pull Request de sa branche vers master et requêter la validation des deux autres élèves
  - Ayoub : approuver la pull request
  - Ana : demander des changements dans la pull request avec un commentaire
  - Ayoub : répondre au commentaire d'Ana'
  - Ana : résoudre le commentaire
  - Léo : fusionner les changements en utilisant le mode Squash and Merge proposé par GitHub

# Note de fin

Si vous avez du temps à la fin du TP, vous pouvez penser à regarder du côté des configurations de votre repository, pour peut-être rajouter une règle de protection de la branche.

*A vos terminaux !*
