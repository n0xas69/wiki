# Commandes shell basiques

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




