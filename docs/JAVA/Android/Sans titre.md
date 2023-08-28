
Anroid est un systeme d'exploitation mobile basé sur le noyau linux et développé par Google.
// Lire sur wikipedia la page 'Noyau linux'
// Présentation de xavier niel ( free ) et steve jobs ( 1er iPhone )

On le retrouve dans plusieurs supports : 
- Smartphones
- Tablettes
- TV , BoxTV
- En voiture, Google Auto


### Spécificités Android 

1. Open Source => A tout moment télécharger les sources et les modifier à votre goût. Apparition ddes "surcouches" afin de personnaliser l'OS pour les constructeurs.
2. Gratuit => Pour le constructeur. 
3. Facile à développer => Les API ou bibliothèques sont très complètes et facile d'accès. http://developer.android.com/
4. Facile à vendre => Une application est disponible sur le Play Store de google qui est une plateforme immense et très visitée. Avec un compte développeur, vous pouvez facilement lancer votre application.

**material.io** Pour une idée de l'ui / ux des bonnes pratique en app mobile

### Le bouton 'Overview' (le carré en bas du téléphone)

C'est une liste des app récemment utilisées. Les app que l'on a dans cette listes *ne tournent pas en fond de tâche*, elle n'utilisent pas de batterie du tout. Ce que l'on voit ce sont des screen shots des activités prises au moment du swipe.
Le fait de swiper supprime le cache, du coup les calculs antérieur prendront plus de temps donc mangeront plus de batterie => Ne pas swiper pour rien ! 

### Le bouton 'Home'

Quitte l'appli mais la laisse tourner en tâche de fond.

### Le bouton 'Retour'

Quitte et détruit l'application.


``` JAVA
Log.d("Tag", "Message sur Android studio")
```
