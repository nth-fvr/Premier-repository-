# 📒 Mon carnet de bord

**Nom :Février  

**Prénom :Nathan 

**Adresse de mon site : https://nthfvr.pythonanywhere.com

> Modifiez ce fichier directement sur GitHub (icône crayon ✏️) pour répondre aux questions de chaque exercice.
> Écrivez avec vos propres mots : une réponse courte et juste vaut mieux qu'un long copier-coller ! 🙂

---

## 🟢 Exercice 1 — Mon premier déploiement

1. Où se trouve physiquement le code qui fabrique votre page : sur votre ordinateur, sur GitHub ou sur PythonAnywhere ?

   > _Ma réponse : Sur Github 

2. Pourquoi votre voisin(e) peut-il voir votre site, alors que vous n'avez rien installé sur son ordinateur ?

   > _Ma réponse : parce que le site est hebergé sur pythonanywhere 

---

## 🟢 Exercice 2 — Les URL et les routes

1. Dans l'URL `https://www.google.com/maps`, quel est le nom de domaine ? Quel est le chemin ?

   > _Ma réponse :_ le nom de domaine est www.google.com et le chemin est /maps.

2. Que veut dire le message *Not Found* ? Qui l'a envoyé : votre navigateur ou le serveur ?

   > _Ma réponse :_ Not Found veut dire que la page demandée n'a pas été trouvée. C'est le serveur qui envoie ce message au navigateur.

3. Que se passe-t-il si deux fonctions portent le même nom dans `flask_app.py` ? (Indice : essayez, puis lisez l'Error log.)

   > _Ma réponse :_ Python remplace la première fonction par la deuxième

---

## 🔵 Exercice 3 — Le langage HTML

1. Quelle est la différence entre ce que le serveur **envoie** et ce que le navigateur **affiche** ?

   > _Ma réponse :_ 

2. À quoi servent les balises `<h1>`, `<p>`, `<ul> ` et `<li>` ?

   > _Ma réponse :_ <h1>: c'est pour le titre principal `, `<p>: c'est pour faire des paragraphes `,<ul>  créer une liste a puce. <li> : sert a créer des éléments de listes

3. Pourquoi l'image s'affiche-t-elle alors qu'elle n'est pas sur votre serveur ?

   > _Ma réponse :_ parce que l'image est hébergée sur un autre serveur. Le navigateur utilise son URL pour la trouver.

---

## 🔵 Exercice 4 — Les templates

1. Pourquoi est-ce une bonne idée de séparer le code Python et le HTML ? (Pensez à une équipe avec un développeur et un graphiste.)

   > _Ma réponse :_ cela permet au développeur de s'occuper du fonctionnement du site et au graphiste de s'occuper de son apparence, c'est plus simple pour tout le monde 

2. Les `{{ prenom }}` sont-ils remplacés par le serveur ou par le navigateur ? Comment l'avez-vous vérifié ?

   > _Ma réponse :_ ils sont remplaces par le serveur. On peut le vérifier en affichant le code source de la page : le prénom apparaît directement à la place de {{ prenom }}.

---

## 🔵 Exercice 5 — Le CSS et les liens

1. Quelle est la différence de rôle entre le HTML et le CSS ?

   > _Ma réponse :_ Le HTML sert à organiser le contenu de la page, tandis que le CSS sert à gérer son apparence

2. Pour afficher votre page `/presentation`, combien de fichiers le navigateur doit-il télécharger ? (Vous pourrez le vérifier à l'exercice suivant !)

   > _Ma réponse :_ Deux fichiers principaux : le fichier HTML de présentation et le fichier CSS, si il y a une image dans la page alors le navigateur doit aussi la télécharger 

3. Pourquoi faut-il parfois faire **Ctrl + F5** pour voir les changements de CSS ?

   > _Ma réponse :_ pour recharger la page pour recharger les fichiers 

---

## 🟣 Exercice 6 — Espionner le navigateur

1. Que signifie HTTP ? Qui envoie la **requête** et qui envoie la **réponse** ?

   > _Ma réponse :_ HTTP signifie HyperText Transfer Protocol. Le navigateur envoie la requête au serveur qui va renvoyer une réponse.

2. Combien de requêtes votre page `/presentation` a-t-elle déclenchées ? Lesquelles ?

   > _Ma réponse :_ 

3. Que signifie le code `200` ? Et le code `404` de la favicon ?

   > _Ma réponse :_ Le code 200 signifie que la requête a réussi. Le code 404 signifie que la ressource demandée n'a pas été trouvée, ici l'icône du site appelée favicon

4. Pourquoi les modifications faites dans l'onglet Éléments ne sont-elles pas visibles par les autres visiteurs ?

   > _Ma réponse :_ Parce qu'elles modifient seulement la page affichée dans mon propre navigateur et ca change pas les fichiers présents sur le serveur.

---

## 🟣 Exercice 7 — Envoyer des informations dans l'URL

1. Dans l'URL `https://www.youtube.com/results?search_query=chat`, quel est le nom du paramètre ? Quelle est sa valeur ?

   > _Ma réponse :_ Le nom du paramètre est search_query et sa valeur est chat.

2. Pourquoi le serveur plante-t-il avec `a=bonjour` ? Que faudrait-il faire pour l'éviter ?

   > _Ma réponse :_ Le serveur peut planter si le code essaie de convertir bonjour en nombre. Il faut vérifier la valeur reçue et gérer les erreurs avec try/except.

3. Pourquoi est-il dangereux d'afficher **tel quel** ce que l'utilisateur envoie ?

   > _Ma réponse :_ Parce qu'un utilisateur peut envoyer du code HTML ou JavaScript malveillant. Cela pourrait modifier la page ou exécuter du code dans le navigateur.

---

## 🟣 Exercice 8 — Les formulaires

1. Quelle est la différence visible entre GET et POST ?

   > _Ma réponse :_ Avec GET, les données apparaissent dans l'URL. Avec POST, elles sont envoyées dans le corps de la requête et ne sont pas visibles directement dans l'URL.

2. Pour un formulaire de **recherche**, quelle méthode choisiriez-vous ? Et pour un formulaire de **connexion avec mot de passe** ? Pourquoi ?

   > _Ma réponse :_ Pour une recherche, je choisirais GET, car les mots recherchés apparaissent dans l'URL et peuvent être partagés. Pour une connexion, je choisirais POST, car le mot de passe n'apparaît pas dans l'URL.

3. Les données envoyées en POST sont-elles vraiment « secrètes » ? (Pensez à ce que vous avez vu dans l'onglet Réseau.)

   > _Ma réponse :_ Non, car elles peuvent être visibles dans l'onglet Réseau du navigateur.

---

## 🔴 Exercice 9 — Les codes de statut

1. Quelle est la différence entre une erreur `4xx` et une erreur `5xx` ? Qui est « fautif » dans chaque cas ?

   > _Ma réponse :_ Les erreurs 4xx viennent d'une mauvaise demande du client, par exemple une page qui n'existe pas (404). Les erreurs 5xx viennent d'un problème du serveur

2. Comment fonctionne une redirection ? Qui fait la deuxième requête : le serveur ou le navigateur ?

   > _Ma réponse :_ Le serveur indique au navigateur une nouvelle adresse grâce à l'en-tête Location. C'est ensuite le navigateur qui fait une deuxième requête vers cette adresse.

3. Donnez un exemple de situation où un vrai site utilise une redirection.

   > _Ma réponse :_ Lorsqu'on n'est pas connecté à un site et qu'on essaie d'accéder à une page réservée aux membres, le site peut nous rediriger vers la page de connexion.

---

## 🔴 Exercice 10 — Ce que le serveur sait de vous

1. Citez trois informations que le serveur connaît sur vous, sans que vous ayez rien rempli.

   > _Ma réponse :_ 

2. À quoi peut servir l'en-tête `Accept-Language` pour un site comme Wikipédia ?

   > _Ma réponse :_ 

3. Dans l'Access log, retrouvez une requête qui a reçu un code `404`. Quelle page était demandée ?

   > _Ma réponse :_ 

4. Après cet exercice, que pensez-vous de la notion de « navigation anonyme » ?

   > _Ma réponse :_ 

---

## 🔴 Exercice 11 — Le Web des machines : API et JSON

1. Quelle est la différence entre une page HTML et une réponse JSON ? À qui chacune est-elle destinée ?

   > _Ma réponse :_ 

2. Dans la page `/horloge`, quel code s'exécute sur le **serveur** et quel code s'exécute dans le **navigateur** ?

   > _Ma réponse :_ 

3. Citez une application de votre téléphone qui, selon vous, utilise une API. Quelles données échange-t-elle ?

   > _Ma réponse :_ 

---

## 🏁 Pour conclure

En quelques phrases, expliquez à un ami ce qui se passe entre le moment où il tape une adresse dans son navigateur et celui où la page s'affiche :

> _Ma réponse :_ 
