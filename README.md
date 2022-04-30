# rapport
Le fonctionnement de flutter 
Première utilisation de Flutter.

La création de projet flutter peut se faire sous le terminal avec la commande :
- flutter create nom_du_projet ou sous vscode 
- CTRL +Shift+P 
- On écrit Flutter 
-On Choisi flutter new project
- On sélectionne le répertoire de notre application
-On donne un nom à notre projet et la magie de Vscode nous créer le projet avec toutes les dépendances et une
première application compteur que l'on peut lancer en appuyant sur F5 pour choisir son émulateur de débogage ou
cliquez sur debug dans le code .

Le fichier principal main.dart est essentiellement composé d'une

-importation du package material.dart qui contient tous nos utilitaires dont on aura besoin.

Flutter présente 2 spécificités principales : Les widgets : ils permettent de décrire simplement le rendu final. Chaque objet est défini indépendamment des contraintes parentes. C'est son emplacement dans le code qui permettra de définir ses contraintes extérieures.

void main() => runApp(MyApp()); Main est la méthode qui permet de lancer une application en Dart.
Dans cette fonction on fait appel a la méthode runApp avec comme argument la classe qui va nous permettre de définir
la base de notre application. RunApp : cette méthode est la porte d'entrée d'une application Flutter
Un classe stateless Widget permettant d'afficher des contenus statique qui retourne
un Scaffold un widget qui nous permet d'afficher des éléments en trois temps en haut avec appbar, en bas
avec bottom et au centre body.
Un stateful Widget nous permettra d'afficher des contenus dynamique sur notre application à exemple
dans l'application de base conteur, c'est un stateful Widget qui permet d'afficher l'évolution du compteur.


classe Scaffold est un widget extensible qui remplit l'espace disponible ou l'écran.
Il fournit une API pour afficher les principaux widgets de l'application tels que
 Drawer,
 SnackBar,
 Bottom-Sheet,
 FloatingActionButton,
 AppBar
 BottomNavigationBar, etc.

La propriété floatingActionButtonAnimator est utilisée pour créer des effets d'animation pour FloatingActionButton.

Dans certaines situations, un bouton peut être automatiquement ajouté à AppBar.leading ou AppBar.actions
pour aider l'utilisateur à ouvrir rapidement drawer,

drawer est un panneau affiché sur le côté gauche de body (si textDirection = TextDirection.ltr).
En général, il est masqué sur les appareils mobiles, vous devez donc le faire glisser de gauche à droite
pour le faire apparaître.

bottomNavigationBar est une barre de navigation affichée en bas de Scaffold.
Dans la plupart des cas d'utilisation, il s'agit d'un objet de BottomAppBar ou de BottomNativationBar.
