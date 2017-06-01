---
title:  "[Cordova / Ionic] Prendre des photos simplement sous Ionic"
---

Prendre ou récupérer des photos est une fonction courante dans une application mobile.
Pour le faire sous ionic deux options s'offrent à vous :

- Utiliser la fonction input file avec un masque de capture
- Utiliser le plugin natif cordova.


## Avec l'input file

Comme sur browser desktop, utiliser l'input[file] vous permet de sélectionner des fichiers du système.

Pour ne sélectionner que les images il conviendra de rajouter les attributs accept et capture

```
<input #fileInput type="file" (change)="fileChange($event)" accept="image/*" capture />
```

ensuite l'evenement `fileChange` vous permettra de récupérer la photo sous format base64.

```
fileChange(event) {
    let files = event.srcElement.files;
    let reader = new FileReader();
    var current = this;
    let loadingIndicator = this.loadingCtrl.create({ content: "Chargement de votre image...", duration: 15000 });
    try {
        reader.readAsDataURL(files[0]);
        /**
         * Check if an image has been uploaded, preventing error if image upload has been canceled
         */
        reader.onload = (event: any) => {
           // do something with image...
           let img = reader.result;
        };
    } catch (e) {
        loadingIndicator.dismiss();
    }
}
```

Et bim vous voila avec une image prete à utiliser dans votre application


## Avec le plugin cordova-plugin-media-capture

L'autre alternative est d'utiliser le plugin cordova de capture. Ce plugin vous permet une interaction plus poussée avec les images et l'appareil photo. Il permet notamment d'enregistrer de l'audio et de la video, que ne permet pas l'input file.
Par contre pour l'utiliser vous aller devoir rajouter des boutons pour chacune des sources possible (capture sur la camera et photo existant dans le filesystem).

Sous ionic2 vous pourrez utiliser le Action Sheet qui très proche du comportement natif sous iOS.



