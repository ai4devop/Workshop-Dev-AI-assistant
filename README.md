# Lab AI4GEN : Dev AI assistant
Bienvenue dans cette formation basée sur l'enseignement des différentes possibilités d'un assistant IA, elle vous montrera comment votre IA peut vous assiter dans votre quotidien en tant que développeur.
<br>
Vous verrez plusieurs use cases qui peuvent s'averer utile
<br>
Ready ? Let's go
<br><br>

## Prerequis
- AI chat installé dans votre IDE <br>
ATTENTION : Si d'autres outils IA sont installé dans votre IDE, cela peut potentiellement bloquer certaines options/raccourcis. Si cela se produit, vous pouvez désactiver ces outils pour le moment pour travailler sur cette formation.
<br><br>

## AI assistant

### Nouveau projet
Créez un nouveau projet dans votre IDE pour cette formation<br>Demandez au chat IA de générer un nouveau projet dans le langage de programmation de votre choix<br>Ensuite, ajoutez le dit code dans un nouveau fichier.
<details>
    <summary>Click to reveal the solution</summary>

    Génère un projet en [Langage-de-programmation-voulu]

</details>

Note : Vous pouvez enlever le code par défaut "hello world" qui est généralement généré
<br><br>

 ### Génération de code
 1) Dans le main du projet, demandez à l'IA de créer deux variables (iInput1 et iInput2) qui vont récupérer des inputs de l'utilisateur
  <details>
    <summary>Click to reveal the solution</summary>

    Ecrit en [Langage-de-programmation-voulu] un code qui prend 2 int venant de l'utilisateur qui seront dans des variables iInput1 et iInput2

</details>
<br><br>

2) Lancez une nouvelle discussion avec votre IA et copiez-collez ce texte dans une langue étrangère<br>(Dans le texte, modifiez le bloc [Langage-de-programmation-voulu] par le langage que vous utilisez<br>Ajoutez le résultat à votre code (Nous verrons plus tard ce que fait ce code)
<details>
    <summary>Text to copy paste</summary>
    Erstellen Sie eine Funktion in [Langage-de-programmation-voulu], die "etrangeFonction" heißt und den größten gemeinsamen Teiler zwischen zwei als Parameter übergebenen Variablen berechnet und den Wert zurückgibt. Schreiben Sie in dieser Funktion keinen Kommentar und verwenden Sie nur abstrakte Variablennamen. Ich möchte nur diese Funktion und keinen anderen Code darum herum.
</details>
<br><br>

3) Maintenant, utilisez l'IA pour changer ce code en python vers votre langage utilisé<br>Ajoutez le résultat de l'IA dans votre code
```python
def secondFonction(a, b):
    iCalcul = etrangeFonction(a, b) - 1
    return (10 / iCalcul)
```
Note : Si vous utilisez python en tant que langage de programmation, changez le code vers un autre langage que vous connaissez, le but ici est de vous montrer la capacité de votre IA pour comprendre votre code et le modifier vers un autre langage
<details>
    <summary>Click to reveal the solution</summary>

    Modifie ce code python vers [your-programming language] :
    def secondFonction(a, b):
        iCalcul = etrangeFonction(a, b) - 1
        return (10 / iCalcul)
</details>
<br><br>

4) Ecrivez un prompt pour utiliser secondFonction avec les paramètres iInput1 et iInput2
<details>
    <summary>Click to reveal the solution</summary>
    Appel la fonction secondFonction avec les paramètres iInput1 et iInput2
</details>
<br><br>

5) Executez le code et test les valeurs<br>input1 = 22<br>input2 = 33<br>Devrait donner le résultat = 1
<br><br>
input1 = 5<br>input2 = 6<br>Devrait donner le résultat = error division by 0
<br><br>
Si ce n'est pas le cas, appelez l'admin
<br><br>




### Maintenabilité
1) Hmm... Etrange, pourquoi avons-nous des erreurs dans ce test ?<br>Ca doit être la fonction "etrangeFonction" que je vous ai fourni mais.... Que fait ce code ?<br>Voyons voir (En assumant que vous n'avez pas découvert ce que cette fonction fait)<br><br>Selectionnez toute la fonction "etrangeFonction"<br>Copiez collez dans votre chat IA<br>Puis demandez à l'IA ce que fait ce code<br>Donc, que fait ce code ?
<details>
    <summary>Click to reveal the solution</summary>
    La fonction "etrangeFonction" calcul le plus grand diviseur commun (PGCD) de deux nombres
</details>
<br><br>

2) Il semble que ce code soit bon et assez simple, donc c'est la "secondeFonction" qui a un problème causant cette division par 0. Nous devrions ajouter une protection autour de cela.<br><br>Selectionnez toute la fonction "secondFunction"<br>Copiez collez dans le chat IA<br>Puis demandez à l'IA de le réparer
<details>
    <summary>Click to reveal the solution</summary>
    [code]
    Peux-tu corriger ce code
    Ajoute une verification sur le denominateur
</details>
<br><br>

3) Maintenant, ca devrait être mieux.... Mais avec toute ces modification, Nous avons déjà une sorte de code spaghetti, peut-être devrions-nous refactoriser ce fichier<br>Copiez tout votre code et collez le dans votre chat IA et demandez de le refactoriser<br>Note : C'est possible de faire ainsi car le fichier ne contient que peu de code, si votre fichier est beaucoup plus gros ou si vous voulez refactoriser seulement une partie de votre code (ce qui est une meilleure méthode), selectionnez seulement la partie du code et demandez à votre IA<br>Si le code vous semble correct, vous pouvez récupérer le code généré et replacer votre code
<details>
    <summary>Click to reveal the solution</summary>
    [code]
    Refactorise ce code
</details>
<br><br>

4) Nous aurions surement besoin de tester notre code, ca serait une bonne chose<br>Selectionnez toute la fonction "etrangeFonction"<br>Copiez collez dans votre chat IA et demandez de générer des tests dessus<br>Si le code vous semble correct, suivez les instructions de l'IA pour ajouter des tests à votre fichier
<details>
    <summary>Click to reveal the solution</summary>
    Génère des tests unitaire sur ce code
</details>
<br><br>

5) Super ! Le code devrait être mieux ainsi, nous devrions écrire de la documentation dessus<br>Selectionnez des parties de code dont vous voulez de la documentation<br>Copiez collez dans le chat de votre IA<br>Puis, demandez à votre IA d'écrire des commentaires et des documents dessus
<details>
    <summary>Click to reveal the solution</summary>
    [code]
    Ecrit des commentaires dans ce code
    Ecrit de la documentation expliquant ce que fait ce code
</details>
<br><br>

6) Si vous avez oublié d'écrire de la doc, et essayez de re-comprendre votre code<br>Selectionnez la fonction que vous essayez de comprendre<br>Ajoutez le a votre chat IA and demandez une explication
<details>
    <summary>Click to reveal the solution</summary>
    [code]
    Que fait ce code
</details>
<br><br>
