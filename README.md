# Formation Git(Hub)

## Git - Notions de base
Git est un logiciel de "versionnage du code".
Il permet essentiellement d'écrire et de suivre l'histoire d'un code.
Cela se fait en marquant le code à des moments précis, c'est-à-dire figer une version du code.
Ce marquage s'appelle un _commit_.
Ainsi, au fur et à mesure du développement, on effectue un commit à chaque version du code qui nous apparait pertinent de conserver.
L'"histoire" de notre code est donc le suivi des commits que nous avons fait.


### Les commits
Les commits sont le coeur de git.
Un commit est une étampe (_stamp_) appliquée sur notre code à laquelle on ajoute un message.

Ci-dessous se trouve un exemple de commits. On y voit le nom de la personne l'ayant fait, la date et le message.
Il devient possible de récupérer l'état exact (i.e. version) à chacun des commits. 
La chaîne des commits correspond à l'histoire du code.
```shell
commit 00dae480110dafd2eda43a512196ecb7c691cae4
Author: Gabriel Couture <gabriel.couture@dfo-mpo.gc.ca>
Date:   Wed Oct 26 13:38:34 2022 -0400

    Correction du bug où species_code était une variable inconnue

commit f84dcd56cf14e7fec04a443d410874349d2a1ed9
Author: Gabriel Couture <gabriel.couture@dfo-mpo.gc.ca>
Date:   Tue Oct 25 16:27:18 2022 -0400

    Ajout de modal pour commenter un échantillon de crevette

commit d50036dd8eaa4200aa5b16b45e74a499063d3922
Author: Gabriel Couture <gabriel.couture@dfo-mpo.gc.ca>
Date:   Tue Oct 25 09:08:25 2022 -0400

    Correction des migrations qui génèrent des échecs
```

### Les branches
Une branche une histoire linéaire du code (une suite linéaire de commits).
Dans certaines situations, il peut être pertinent d'avoir plusieurs branches en parallèle,
notamment lorsque plusieurs personnes travaillent sur le même projet, mais des parties différentes du code.

Un projet contient typiquement une branche principale, _main_ ou _master_.

L'image suivante [1]

![exemple branches](./images/branches-harness.io.png)


# Utilisation de Git et de GitHub
Git est un logiciel qui s'utilise en ligne de commande (dans un terminal).
Cependant, il peut être plus simple de l'utiliser au travers
l'application GitHub Desktop (https://desktop.github.com/).


### Flot de travail
0. (Si ce n'est pas déjà fait) Cloner le projet 
1. Récupérer les derniers changements du répertoire ajoutés sur GitHub
1. Décider sur quelle branche faire ses ajouts/modifications dans le code
2. (Au besoin) Si aucune branche existante ne convient, en créer une nouvelle
3. (Au besoin) Basculer vers la branche choisie ou nouvellement créée
4. Écrire/modifier le code
5. Ajouter les changements dans le code désirés en préparation à un commit
6. Faire un commit
7. Pousser les changements sur GitHub
8. (Au besoin) À même GitHub, faire une _Pull Request_ (PR) pour _merger_ les changements de votre branche vers la branche principale (_main_ ou _master_)


TODO : détaillé comment faire les étapes ci-dessus via GitHub Desktop et via le terminal ... 

## Références
[1] Image tirée de https://harness.io/blog/git-branching
