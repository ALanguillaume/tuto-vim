# Tuto vim - ThinkR by Languille

## Les **modes** pour se mettre dans le mood

Vim est un éditeur modal. Les touches ont différentes fonctions
en fonction du mode activé.

Par défaut vim se lance en mode NORMAL.

Le mode NORMAL vous permet de vous déplacer.

`i` me permet de passer en mode INSERT et d'inśerer du texte.

`Esc` me permet de repasser en mode NORMAL.

En mode normal, je peux aussi executer des commandes grâce `:`.

`:w` write -> enregistrer 
`:wq` write + quit -> enregistrer et quitter


## Apprendre à marcher

```
	    ^
	    k		   
  < h	  l >	
	    j		
	    v
```
Les flèches ça marche aussi.

## J'ai glissé chef !

`x`: supprimer un caractère

___

La vaache est ddans le préé.
___

`u`: annuler le changement
`Ctrl+R`: Rétablir le changement

## On va bouger, bouger !

Quand vous êtes en mode normal, chaque touche correspond à un mouvement donné.

### On commence petit petons

À l'échelle du mot.

`w`: avancer d'un mot
`e`: aller à la fin du mot
`b`: aller au début du mot

`3w`: J'avance de 3 mots etc.. 

___

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
___

### On va plus loin


`0`: reculer au début de la ligne
`$`: avancer à la fin de ligne

___

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
___

### Parchutage en INSERT mode

`a` : caractère suivant
`A` : fin de la ligne
`I` : Début de la ligne
`o` : Début de la ligne suivante
`O` : Début de la ligne précédente

___
i
Il manque un point à la fin de cette ligne
Il manque une majuscule au début de cette ligne.

Je veux commencer à écrire en dessous.

Je veux commencer à écrire au dessus.
___


### Les bottes de 7 lieux

`gg`: Début du document
`G`: Fin du document
`{` et `}`: Sauter un bloc de ligne
`[` et `]`: Sauter un paragraphe


## Copier/Supprimer des trucs

`y` + motion : "yank" copier
`d` + motion : "delete" supprimer

___

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
___

`dd` Supprime la ligne entière

## Changer des trucs

`c`:
 - `a` (around) ou `i` inside
 - un symbole `(`, `"`, `'`, `{`...
 
``` r
golem_add_external_resources <- function() {
  add_resource_path(
    "www",
    app_sys("app/www")
  )

  tags$head(
    favicon(),
    bundle_resources(
      path = app_sys("app/www"),
      app_title = "cartobleau"
    )
    # Add here other external resources
    # for example, you can add shinyalert::useShinyalert()
  )
}
```

## Faire des bonds

### Sur une ligne

`f` + `lettre` : avancer jusqu'à la lettre
`F` + `lettre` :

### Dans tous le document

`/` Recherche rapide. `n` et `N` servent à parcourir les résultats.

Chercher le mot golem.


## Remplacer des trucs

Sur une ligne :
`:s/regex/remplacement/g`

Sur tout le fichier :
`:%s/regex/remplacement/g`



## Miscellanées

### Faire de jolis titres de sections dans mes scripts R

Se mettre au bout de la ligne puis `80A-Esc` puis `d80|`.


#### Mon titre de section

### Trier par ordre alphabétique

### Se filmer entrain de la faire.

grapefruit
clementine
feijoa
jambul
nut
chili pepper
cherimoya
pomegranate
gooseberry
purple mangosteen
bell pepper
peach
dragonfruit
blueberry
eggplant
passionfruit
pomelo
guava
olive

## Explorer des dossiers

```
vim .

```

## Bindings pour votre IDE favori

* Avec VSCode installez l'extension VSCodeVim
* Avec Rstudio: Global Options > Code > Editing > General > Keybindings :
    Choisir vim

## Il n'ya pas un vim chaque personne à son propre vim

Voir .vimrc

## Pour apprendre 

```
vim tutor

```


