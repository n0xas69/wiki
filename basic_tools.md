# Commandes et outils basiques

## input / ouput
```>``` redirige le STDOUT (standard output)  
```2>``` redirige le STDERR (standard error)  
```<``` redigire le STDIN (standard input)


Redirige dans un fichier, écrase le contenu du fichier
```bash
echo test > fichier.txt 
```

Redirige dans un fichier à la suite du contenu
```bash
echo test >> fichier.txt
```

Si on veux qu'une commande ne retourne pas d'erreur, on peu se servir de /dev/null en ridigeant le STDERR dessus :
```bash
ls kejfiuf Documents 2> /dev/null
```
Dans ce cas le dossier "kejfiuf" n'existe pas, mais la commande ne retournera que "Documents"

Le pipe permet de passer la sortie d'une commande en entré d'une autre commande, ex :
```bash
cat fichier.txt | grep test
```

## Historique

Dès qu'un utilisateur ouvre un shell, un fichier .bash_history est créé à la racine de son répertoire home. Il contient l'historique des commandes tapé.
Pour le lire il suffit de taper ```history```

la combinaison ```ctrl+r``` permet de chercher et taper une commande déjà effectuer.

## vi / vim

Vi est l'éditeur de text par défaut sur toute les distrib linux, connaître les commandes de bases est important :

```esc``` : basculer en mode commande
```i``` : basculer en mode insert pour taper du text
```:n``` : ou n est le numéro de ligne ou placer le curseur
```dd``` : supprimer la ligne
```u``` : annule le dernier changement (équivalent ctrl-z)
```yy``` : copie la ligne
```p``` : colle la ligne
```o``` : créer une nouvelle ligne
```:q!``` : quitte sans sauvegarder
```:wq``` : quitte en sauvegardant


