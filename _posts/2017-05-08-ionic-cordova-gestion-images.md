---
title:  "[Cordova / Ionic] Gérer la rotation images sous cordova / Ionic"
---

En développant une application mobile Ionic pour un client, je suis tombé sur une problématique un peu particulière de IOS : l'orientation des images.


## Le problème

Sous iOS, lorsque que vous prenez une photo, l'appareil enregistre un certain nombre d'orientations, notamment l'orientation de l'image.
Jusque la pas de problème. La ou ca se corse, c'est que l'orientation normale de votre téléphone devrait être "en paysage tourné vers la gauche". Les informations d'orientations sont donc définies à partir de cette base. Le problème est que l'imense majorité des utilisateurs font leur photos (et videos) en tenant le téléphone droit.
Les informations sont donc "erronnées". Sur le device cela ne pose pas vraiment de problème car les clients natifs de visualisation (eg. photo roll, photo view etc), font la rotation correctement.

Par contre si vous regardez votre image dans une logiciel qui ne gère pas automatiquement l'orientation (disons un site web, ou une application dans une webview façon Cordova), et bien la l'image est dans un angle bizarre !



## Solutions

La solution peut être très simple comme un peu plus compliquée. Si vous avez pris votre photo en utilisant le plugin cordova ()[], la solution est simple. Il suffit de rajouter la mention `fixOrientation:true` dans votre appel de lancement de la capture.

```
{
fixOrientation:true
}
```

Si par contre vous êtes appuyer sur l'input file. Il va vous falloir opérer la rotation manuellement.



### La rotation manuelle

Pour effectuer la rotation de votre image, vous allez avoir besoin de duex outils. Un extracteur d'informations EXIF o

## Conclusion

Dans notre cas, nous avons choisi de partir sur confluence, afin de ne pas perdre de temps et d'avoir l'esprit tranquille.

