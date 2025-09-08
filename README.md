# Instructions : Code pour suite de Syracuse

On définit la suite d'entiers $$(u_n)_{n\in\mathrm{N}}$$ de la manière suivante :

Le terme initial $$u_0$$ est donné puis pour tout $$n>1$$:

Si $$u_n$$ est pair, $$u_{n+1} = u_n/2$$

Si $$u_n$$ est impair, $$u_{n+1} = 3u_n + 1$$

Une conjecture (résultat non encore démontré) affirme que cette suite finit toujours par 1 quelque soit l'entier $$u_0$$ choisi initialement.

1. Ecrire un programme (dans syracuse.c) qui permet de tester cette conjecture. Un $$u_0 > 1$$ sera choisi par l'utilisateur et on vérifiera qu'il existe un rang p pour lequel $$u_p = 1$$. On note que l'opérateur % peut être utilisé ici (a%b donne le reste de la division de l'entier a par l'entier b).

2. Tracer avec Python les valeurs successives de la suite en fonction de l'itération, pour un $$u_0$$ donné. On pourra prendre $$u_0$$ nombre premier de manière à avoir plus d'itérations.

On appelle altitude de $$u_0$$ le nombre entier maximal atteint lors des itérations successives de la suite, en partant de la valeur initiale $$u_0$$. On appelle temps de vol de $$u_0$$ le nombre d'itérations nécessaires avant d'atteindre 1, en partant de la valeur initiale $$u_0$$.

3. Compléter le programme précédent pour calculer et afficher l'altitude et le temps de vol d'un entier $$u_0$$ choisi par l'utilisateur.

4. Ecrire et tester une fonction qui ne renvoie rien mais qui permet pour un entier $$u_0$$ donné d'afficher son altitude et son temps de vol.


# Instructions : Utiliser Git pour cloner, modifier, commit, et push

## 1. Cloner le dépôt

La première étape est de cloner ce dépôt Git sur votre machine locale.

Ouvrez un terminal et exécutez la commande suivante :

```bash
git clone <URL du dépôt>
```

Cela va télécharger tous les fichiers du dépôt sur votre ordinateur.

Ensuite, accédez au dossier cloné :

```bash
cd nom_du_dépôt
```

---

## 2. Créé le fichier `syracuse.c`

Ouvrez un nouveau fichier `syracuse.c` dans un éditeur de texte comme Visual Studio Code, Notepad++, ou autre.

Implementez le programme comme indiqué ci-dessus

Sauvegardez vos modifications après les avoir faites.

---

## 3. Ajouter les modifications à Git (staging)

Vous devez indiquer à Git que vous avez crée ce fichier. Vous ferez pareil pour toute modification de fichier ultérieure. Utilisez la commande suivante pour ajouter ces modifications à l'index de Git :

```bash
git add syracuse.c
```

Cette commande indique à Git de préparer le fichier (nouveau ou modifié) pour un commit.

---

## 4. Effectuer un commit

Une fois les modifications ajoutées à l'index, vous pouvez faire un commit pour enregistrer ces modifications dans l'historique Git. Tapez la commande suivante avec un message descriptif de vos changements :

```bash
git commit -m "Ajout du fichier syracuse.c"
```

Le commit crée un instantané de vos modifications, avec un message expliquant ce que vous avez fait.

---

## 5. Pousser les modifications vers GitHub

Maintenant que vous avez commité vos changements, il est temps de les envoyer (ou "pousser") vers le dépôt distant sur GitHub. Utilisez la commande suivante :

```bash
git push origin main
```

Cela envoie vos modifications sur la branche `main` du dépôt distant (`origin` fait référence au dépôt GitHub d'où vous avez cloné).

---

## 6. Vérifier sur GitHub

Une fois la commande `git push` exécutée, allez sur la page du dépôt GitHub et actualisez la page pour vérifier que vos modifications ont bien été envoyées. Vous devriez voir vos nouveaux commits et les modifications du fichier `README.md`.

---

### Explication des commandes dans le guide :
1. **`git clone`** : Clone le dépôt depuis GitHub vers votre machine.
2. **`git add`** : Prépare (ou "stage") les fichiers modifiés pour être committés.
3. **`git commit -m`** : Enregistre les changements avec un message descriptif.
4. **`git push origin main`** : Envoie les changements vers le dépôt distant GitHub.
