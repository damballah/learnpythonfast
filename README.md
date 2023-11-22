# LEARN PYTHON FAST (VERY FAST)
#### _Temps de lecture approximatif de ce texte : 15-20 minutes._

Cette idée d'un condensé ultra-court pour apprendre le langage Python m'est venue du fait qu'au lycée, en seconde particulièrement, le Python est enseigné par des professeurs sur la base du volontariat. Le problème, c'est que, par exemple, pour les professeurs de mathématiques, ils ne vont faire QUE des maths. Or, avec le Python, on fait bien plus que "uniquement" des maths. J'ai donc voulu monter un document simple à suivre, avec les fondements de base de la programmation tout court :

-Les variables
-Les conditions
-Les Boucles
-Lecture/Ecriture dans des fichiers
-Creation de fonctions
-Création d'objets (class)

Donc, voici un aperçu du langage Python pour apprendre très rapidement
et grossièrement, les "vraies" bases... Issu d'une discussion avec ChatGpt : 
https://chat.openai.com/share/c7cf9f64-6953-4283-8522-18f7f83b451d

___

Introduction :

Python est un langage de programmation largement utilisé dans divers domaines, de la création d'applications web à l'analyse de données et à l'intelligence artificielle. Sa popularité repose sur sa syntaxe simple et lisible, ce qui en fait un excellent choix pour les débutants et les développeurs expérimentés. Comprendre les fondamentaux de Python est essentiel pour tirer pleinement parti de ses capacités.

La programmation est un moyen puissant de résoudre des problèmes, d'automatiser des tâches et de créer des applications innovantes. Ce cours vise à introduire les principaux concepts de programmation en Python, du travail avec des variables à la création de fonctions et d'objets.

___

### Section 1 : Les Variables

#### 1.1. Qu'est-ce qu'une Variable ?

En programmation, une variable est un conteneur symbolique permettant de stocker des données. Elle est utilisée pour représenter des valeurs qui peuvent changer tout au long de l'exécution d'un programme. En Python, la création d'une variable est simple : vous lui attribuez un nom et lui assignez une valeur.

```
python# Déclaration d'une variable
age = 25

# Affichage de la variable
print(age)

```

Dans cet exemple, la variable `age` stocke la valeur 25. Cette valeur peut être modifiée tout au long du programme, offrant une flexibilité dynamique.

#### 1.2. Types de Variables en Python

Python prend en charge différents types de variables. Les entiers (`int`) sont utilisés pour représenter des nombres entiers, les décimaux (`float`) pour les nombres à virgule flottante, et les chaînes de caractères (`str`) pour le texte.

```
python# Différents types de variables
entier = 10
decimal = 3.14
chaine = "Bonjour"

# Affichage des variables
print(entier, decimal, chaine)

```

Les types de variables déterminent le type de données que la variable peut stocker. Cela offre une flexibilité dans la manipulation de différents types de valeurs.

#### 1.3. Exemples et Analogies

Pour comprendre les variables, considérons-les comme des boîtes dans lesquelles vous rangez des objets. Chaque boîte a une étiquette (le nom de la variable) et contient quelque chose (la valeur de la variable).

```
python# Exemple d'analogie
nom = "Alice"
age = 30
print("Nom:", nom, "Age:", age)

```

Ici, la variable `nom` contient la chaîne de caractères "Alice", et la variable `age` contient le nombre 30.

### Section 2 : Les Conditions

#### 2.1. Introduction aux Conditions

Les structures conditionnelles permettent d'exécuter des blocs de code en fonction de certaines conditions. Cela permet au programme de prendre des décisions dynamiques.

```
python# Utilisation de la condition
temperature = 25

if temperature > 30:
    print("Il fait chaud.")
else:
    print("La température est agréable.")

```

Dans cet exemple, le programme affiche un message différent en fonction de la valeur de la variable `temperature`. Si la température est supérieure à 30, il affiche "Il fait chaud", sinon, il affiche "La température est agréable".

#### 2.2. Opérateurs de Comparaison

Les opérateurs de comparaison (==, !=, <, >, <=, >=) permettent de comparer des valeurs. Ils retournent un résultat booléen (Vrai ou Faux) en fonction de la condition.

```
python# Opérateurs de comparaison
a = 5
b = 10

if a == b:
    print("a est égal à b")
elif a < b:
    print("a est inférieur à b")
else:
    print("a est supérieur à b")

```

Ici, le programme compare les valeurs de `a` et `b` et affiche le résultat en conséquence.

#### 2.3. Instructions If, Else, et Elif

Les instructions `if`, `else`, et `elif` permettent de créer des branches conditionnelles. Si une condition n'est pas satisfaite, le programme peut passer à une autre condition.

```
python# Instructions If, Else, et Elif
heure = 14

if heure < 12:
    print("Bonne matinée!")
elif 12 <= heure < 18:
    print("Bonne après-midi!")
else:
    print("Bonne soirée!")

```

Ici, le programme souhaite une bonne matinée, après-midi ou soirée en fonction de la valeur de la variable `heure`.

### Section 3 : Les Boucles

#### 3.1. Introduction aux Boucles

Les boucles permettent de répéter des blocs de code plusieurs fois, évitant ainsi la redondance et économisant du temps.

```
python# Boucle While
compteur = 0
while compteur < 5:
    print("Tour", compteur)
    compteur += 1

```

Cette boucle `while` répète le bloc de code tant que la condition (compteur < 5) est vraie. Ici, elle affiche "Tour" suivi du numéro du tour.

#### 3.2. Boucle While

La boucle `while` continue tant que la condition spécifiée est vraie. Elle est souvent utilisée lorsque le nombre d'itérations n'est pas connu à l'avance.

```
python# Boucle While
nombre = 1
while nombre <= 5:
    print(nombre)
    nombre += 1

```

Ici, la boucle `while` affiche les nombres de 1 à 5.

#### 3.3. Boucle For

La boucle `for` parcourt une séquence (comme une liste) et exécute un bloc de code pour chaque élément de la séquence.

```
python# Boucle For
for lettre in "Python":
    print(lettre)

```

Cette boucle `for` affiche chaque lettre de la chaîne "Python".

### Section 4 : Lecture et Écriture de Fichiers

#### 4.1. Ouverture et Fermeture de Fichiers

La manipulation de fichiers en Python implique l'ouverture et la fermeture de connexions avec eux.

```
python# Ouverture et fermeture de fichiers
fichier = open("exemple.txt", "w")
fichier.write("Contenu du fichier.")
fichier.close()

```

Ici, le programme ouvre un fichier en mode écriture ("w"), écrit du contenu, puis ferme le fichier. Le mode "w" écrase le contenu existant du fichier.

#### 4.2. Lecture de Fichiers

La lecture de fichiers se fait avec la fonction `open()` et la méthode `read()`.

```
python# Lecture de fichiers
fichier = open("exemple.txt", "r")
contenu = fichier.read()
print(contenu)
fichier.close()

```

Le programme ouvre le fichier, lit son contenu avec `read()`, l'affiche, puis ferme le fichier.

#### 4.3. Écriture dans un Fichier

L'écriture dans un fichier utilise la fonction `open()` avec le mode d'écriture ("a" pour ajouter) et la méthode `write()`.

```
python# Écriture dans un fichier
fichier = open("exemple.txt", "a")
fichier.write("\nNouvelle ligne.")
fichier.close()

```

Ici, le programme ajoute une nouvelle ligne au fichier existant.

### Section 5 : Création de Fonctions

#### 5.1. Qu'est-ce qu'une Fonction ?

Une fonction est un bloc de code réutilisable qui accomplit une tâche spécifique. Elle favorise la modularité du code, car elle peut être appelée à partir de différentes parties du programme.

```
python# Fonction simple
def saluer():
    print("Bonjour!")

# Appel de la fonction
saluer()

```

La fonction `saluer()` affiche simplement "Bonjour!" lorsque vous l'appelez.

#### 5.2. Déclaration de Fonction

Les fonctions sont déclarées avec le mot-clé `def`, suivi du nom de la fonction et de ses paramètres éventuels.

```
python# Déclaration de fonction avec paramètres
def multiplier(a, b):
    return a * b

# Appel de la fonction
resultat = multiplier(3, 4)
print(resultat)

```

La fonction `multiplier()` prend deux paramètres, multiplie les valeurs et renvoie le résultat.

#### 5.3. Paramètres et Retour de Fonction

Les paramètres permettent de passer des informations à une fonction, et le mot-clé `return` est utilisé pour renvoyer une valeur.

```
python# Fonction avec paramètres et retour
def carre(nombre):
    return nombre ** 2

# Appel de la fonction
res = carre(5)
print(res)

```

La fonction `carre()` prend un nombre en paramètre, calcule son carré avec `nombre ** 2`, puis renvoie le résultat.

### Section 6 : Création d'Objets

#### 6.1. Introduction aux Objets

En Python, tout est un objet. Les objets sont des instances de classes, définissant la structure et le comportement des objets.

```
python# Création d'une classe
class Animal:
    def __init__(self, nom):
        self.nom = nom

    def parler(self):
        pass

# Création d'un objet
chien = Animal("Rex")

```

Ici, la classe `Animal` a une méthode `parler()`. Un objet `chien` est créé à partir de cette classe, avec le nom "Rex".

#### 6.2. Déclaration de Classe

Les classes définissent les propriétés et les méthodes des objets. Elles sont déclarées avec le mot-clé `class`.

```
python# Déclaration de classe avec méthode
class Voiture:
    def __init__(self, marque, modele):
        self.marque = marque
        self.modele = modele

    def afficher_details(self):
        print(f"{self.marque} {self.modele}")

# Création d'un objet
ma_voiture = Voiture("Toyota", "Corolla")
ma_voiture.afficher_details()

```

La classe `Voiture` a une méthode `afficher_details()` qui affiche la marque et le modèle de la voiture.

#### 6.3. Création d'Objets

Les objets sont créés à partir de classes à l'aide de la syntaxe "nom\_objet = NomClasse()".

```
python# Création d'objets à partir d'une classe
class Rectangle:
    def __init__(self, longueur, largeur):
        self.longueur = longueur
        self.largeur = largeur

# Création d'objets
rectangle1 = Rectangle(5, 10)
rectangle2 = Rectangle(3, 8)

```

Ici, deux objets de la classe `Rectangle` sont créés avec différentes longueurs et largeurs.

### Conclusion

La programmation en Python repose sur des concepts clés tels que les variables, les conditions, les boucles, la manipulation de fichiers, les fonctions et les objets. Ces concepts offrent une base solide pour résoudre des problèmes et créer des applications. Il est crucial de comprendre ces concepts fondamentaux pour progresser en programmation. Encouragez les élèves à pratiquer régulièrement, à explorer davantage Python et à participer à des projets pour renforcer leurs compétences. La programmation est une compétence puissante et créative qui s'améliore avec la pratique continue.
