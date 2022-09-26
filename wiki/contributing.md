# Contributing Guide


Toutes les demandes d'extraction et suggestions sont très appréciées et encouragent

> Bienvenue ! Nous aimons recevoir des contributions de notre communauté, alors merci d'être passé! Il existe de nombreuses façons de contribuer, notamment en soumettant des rapports de bogue, en améliorant la documentation, en soumettant des demandes de fonctionnalités, en examinant de nouvelles soumissions ou en contribuant au code qui peut être intégré au projet.

Ce document décrit notre processus de développement. Le respect de ces directives montre que vous respectez le temps et les efforts des développeurs qui gèrent ce projet. En retour, vous serez respecté dans la résolution de votre problème, l'examen de vos modifications et l'intégration de vos contributions.

**Table of Contents:**

1. [Code of Conduct](#code-of-conduct)
2. [Important Resources](#important-resources)
2. [Questions](#questions)
3. [Feature Requests](#feature-requests)
4. [Improving Documentation](#improving-documentation)
5. [Reporting Bugs](#reporting-bugs)
6. [Contributing Code](#contributing-code)
	1. [Getting Started](#getting-started)
	1. [Finding an Issue!](#finding-an-issue)
	1. [Development Process](#development-process)
1. [Pull Request Guidelines](#pull-request-process)
	1. [Processus de vérification](#processus-de-vérification)
	1. [Répondre aux commentaires](#répondre-aux-commentaires)


## Code of Conduct

Aller lire le Code of Conduct

## Important Resources

* wiki
* projets

## Questions

si vous avez des questions, n'hésitez pas à nous contacter avec les issues.

## Feature Requests

Utiliser les templates et les labels de Feature Requests

## Reporting Bugs

Utiliser les templates et les labels de Reporting Bugs

## Improving Documentation

Utiliser les templates et les labels Improving Documentation

## Contributing Code

* [How to Contribute to an Open Source Project on GitHub][2]
* [Make a Pull Request][3]
* [First Timers Only][4]


### Getting Started

Suivez le Guide installation

Fournissez des instructions pour votre flux de travail (par exemple, bifurquez le référentiel)

> Vous devrez bifurquer le référentiel principal pour travailler sur vos modifications. Accédez simplement à notre page GitHub et cliquez sur le bouton "Fork" en haut. Une fois que vous avez forké le référentiel, vous pouvez cloner votre nouveau référentiel et commencer à apporter des modifications.

> Dans git, il est préférable d'isoler chaque sujet ou fonctionnalité dans une « branche thématique ». Alors que les commits individuels vous permettent de contrôler la façon dont les petites modifications individuelles sont apportées au code, les branches sont un excellent moyen de regrouper un ensemble de commits tous liés à une fonctionnalité, ou d'isoler différents efforts lorsque vous travaillez sur plusieurs sujets à la fois. en même temps.

> Même s'il faut une certaine expérience pour avoir une bonne idée de la façon de diviser les commits, une branche thématique doit être limitée à un seul problème

```
# Checkout the master branch - you want your new branch to come from master
git checkout master

# Create a new branch named newfeature (give your branch its own simple informative name)
git branch newfeature

# Switch to your new branch
git checkout newfeature
```

### Finding an Issue

Choisissez un problème non attribué que vous pensez pouvoir résoudre et ajoutez un commentaire indiquant que vous essayez de le faire.

Fournir des notes sur différents types de problèmes ou d'étiquettes

### Development Process

Quel est votre processus de développement ?

> Ce projet suit le modèle de développement de produit en [git flow](http://nvie.com/posts/a-successful-git-branching-model/).

Parlez des branches sur lesquelles les gens devraient travailler. Concrètement, où est le point de départ ? `maître`, `développement`, etc.

> Vous devriez utiliser la branche master pour la version la plus stable ; veuillez consulter régulièrement les [notes de version](https://github.com/openopps/openopps-platform/releases). Nous faisons des publications toutes les semaines ou toutes les deux semaines et envoyons des notes. Si vous voulez suivre les dernières modifications, nous travaillons dans la branche `dev`. Si vous utilisez dev, gardez un œil sur les commits et/ou rejoignez notre stand-up quotidien.

## Processus de demande d'extraction

Avez-vous des conventions d'étiquetage ?

Ajoutez des notes pour pousser votre branche :

> Lorsque vous êtes prêt à générer une pull request, soit pour un examen préliminaire, soit pour envisager de fusionner dans le projet, vous devez d'abord repousser votre branche thématique locale vers GitHub :

```
git push origin newfeature
```

Inclure une note sur la soumission du PR :

> Une fois que vous avez validé et poussé toutes vos modifications sur GitHub, accédez à la page de votre fork sur GitHub, sélectionnez votre branche de développement et cliquez sur le bouton pull request. Si vous avez besoin d'apporter des modifications à votre pull request, envoyez simplement les mises à jour à votre branche. Votre pull request suivra automatiquement les changements sur votre branche de développement et la mise à jour.

1. Assurez-vous que toutes les dépendances d'installation ou de construction sont supprimées avant la fin de la couche lors d'une
   construire.
2. Mettez à jour le fichier README.md avec les détails des modifications apportées à l'interface, cela inclut le nouvel environnement
   variables, ports exposés, emplacements de fichiers utiles et paramètres de conteneur.
3. Augmentez les numéros de version dans tous les exemples de fichiers et le fichier README.md à la nouvelle version
   Pull Request représenterait. Le schéma de version que nous utilisons est [SemVer](http://semver.org/).
4. Vous pouvez fusionner la demande d'extraction une fois que vous avez l'approbation de deux autres développeurs, ou si vous
   n'avez pas la permission de le faire, vous pouvez demander au deuxième examinateur de le fusionner pour vous.

### Processus de vérification

Qui l'examine ? Qui doit signer avant qu'il ne soit accepté ? Quand un contributeur doit-il s'attendre à avoir de vos nouvelles ? Comment les contributeurs peuvent-ils obtenir un accès au commit, le cas échéant ?

> L'équipe principale examine régulièrement les demandes d'extraction lors d'une réunion de triage hebdomadaire que nous organisons dans un Google Hangout public. Le hangout est annoncé dans les mises à jour de statut hebdomadaires qui sont envoyées à la liste puppet-dev. Les notes sont publiées sur le référentiel de triage de la communauté Puppet Community et incluent un lien vers un enregistrement YouTube du hangout. Une fois les commentaires reçus, nous attendons des réponses dans les deux semaines. Après deux semaines, nous pouvons fermer la pull request si elle ne montre aucune activité.

> À l'exception des correctifs critiques, urgents ou très mineurs, nous essayons de laisser les pull requests ouvertes presque toute la journée ou toute la nuit si quelque chose arrive tard dans la journée, afin que plusieurs personnes aient la possibilité de réviser/commenter. Quiconque examine une pull request doit laisser une note pour informer les autres que quelqu'un l'a examinée. Pour les commits plus importants, nous aimons avoir un +1 de quelqu'un d'autre dans l'équipe principale et/ou d'autres contributeurs. Veuillez noter que si vous avez examiné le code ou testé localement - un +1 en lui-même sera généralement interprété comme si vous pensiez que c'était une bonne idée, mais que vous n'aviez pas examiné en détail.

Peut-être aussi fournir les étapes que votre équipe utilisera pour vérifier un PR. Ou discutez des étapes exécutées sur votre serveur CI si vous en avez un. Cela aidera les développeurs à comprendre comment enquêter sur les échecs ou tester le processus par eux-mêmes.

### Répondre aux commentaires

Once a PR has been submitted, your changes will be reviewed and constructive feedback may be provided. Feedback isn't meant as an attack, but to help make sure the highest-quality code makes it into our project. Changes will be approved once required feedback has been addressed.

If a maintainer asks you to "rebase" your PR, they're saying that a lot of code has changed, and that you need to update your fork so it's easier to merge.

To update your forked repository, follow these steps:

```
# Fetch upstream master and merge with your repo's master branch
git fetch upstream
git checkout master
git merge upstream/master

# If there were any new commits, rebase your development branch
git checkout newfeature
git rebase master
```

If too much code has changed for git to automatically apply your branches changes to the new master, you will need to manually resolve the merge conflicts yourself.

Once your new branch has no conflicts and works correctly, you can override your old branch using this command:

```
git push -f
```

Note that this will overwrite the old branch on the server, so make sure you are happy with your changes first!
