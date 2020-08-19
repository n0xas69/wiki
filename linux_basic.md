# Commandes basiques linux

### ```cd``` : Se déplacer dans le système

```bash
# on se déplace dans le dossier home
cd /home

# on se déplace dans le dossier log
cd /var/log
```

### ```ls``` : Lister les dossier/fichier

```bash
# affiche les dossiers et fichiers du chemin ou on est situé
ls

# affiche les fichiers de /home/noxas
ls /home/noxas

# affiche sous forme de liste les fichiers de /etc avec les droits
ls -l /etc
```

which
diff
du
head
less
sort
grep
find
watch

# Astuces

Liste les x fichier les plus gros du répertoire courant
```bash
du -a | sort -n -r | head -n 15
```
