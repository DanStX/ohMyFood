### DOSSIER VENDORS
Et last but not least, la plupart des projets comportent un dossier vendors/ qui regroupe tous les fichiers CSS provenant de bibliothèques et frameworks externes — Normalize, Bootstrap, jQueryUI, FancyCarouselSliderjQueryPowered, etc. Le fait de les mettre ainsi de côté dans un dossier séparé est une bonne façon d’indiquer qu’ils ne sont pas de vous et ne relèvent pas de votre responsabilité.

#### Exemple :

        _normalize.scss
        _bootstrap.scss
        _jquery-ui.scss
        _select2.scss

Si vous devez remplacer une section d’un fichier vendor, je recommande de créer un 8e dossier nommé vendors-extensions/ dans lequel vous aurez des fichiers nommés en fonction du vendor qu’ils remplacent.

Par exemple, vendors-extensions/_boostrap.scss serait un fichier contenant toutes les règles CSS qui re-déclarent le CSS par défaut de Bootstrap. Vous éviterez ainsi de modifier les fichiers vendors eux-mêmes, ce qui n’est pas conseillé.