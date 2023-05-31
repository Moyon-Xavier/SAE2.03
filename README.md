# **SAE 2.03 by Illies Douhab / Xavier Moyon / Nathan Vasset**

Vous trouverez ci-joint un fichier commande.sh ainsi que un fichier SAE_2.03.md. Pour creer le fichier HTML et PDF executer la commande `./commande.sh` (assurez-vous d'etre dans le répertoire du fichier)

## **Guide D'instalation**
Ce guide présente les différentes étapes pour installer Debian.

### **Prérequis** 
Pour l'instalation de Debian 
- Une machine compatible debian 
- Un support d'installation tels que un DVD, ou une clef bootable préconfigurer, sinon vous pouvez la configurer en installant l'iso et creer une clef bootable grace au logicele [RUFUS](https://rufus.ie/fr/) 
- Une connection Internet est recommandé pour télécharger les paquets supplémentaires pendant l'installation 

Maintenant lancer votre machine avec votre support, executez le lors du lancement de la machine et suivez les étapes du MarkDown (SAE_2.03.md)

Pour pouvoir voir le fichier pandoc :
- Installtion de pandoc :  `sudo apt insyall pandoc `
- Installer PdfLatex : `sudo apt-get install texlive-fonts-recommended `
- Executer la commande `./commande.sh`


### **Questions de la sae**
Toutes les questions posées lors des SAE sont présentes dans le MarkDown entre les différentes étapes d'installation.

### **la commande `./commande.sh`**
la commande `./commande.sh` permet de créer les fichiers HTML et PDF grace a deux lignes de commande :
- `pandoc --standalone --toc --css=./style.css -o ./SAE_2.03_PDF.pdf ./SAE_2.03.md;`
- `pandoc --standalone --toc --css=./style.css -o ./SAE_2.03_HTML.html ./SAE_2.03.md --metadata title="SAE_2.03";`

`**./commande.sh` est un programme de convertion de fichier entre les formats de balisage 

