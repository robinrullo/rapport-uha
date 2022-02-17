# Template de rapport étudiant UHA 4.0

## Installation
Il est nécessaire d'installer latex et [pygments](https://pygments.org/docs/cmdline/) (pour la colorization du code) pour générer le PDF.

## Utilisation

Il est également nécessaire d'ajouter l'option `-shell-escape` lors de la génération du pdf.
![image](https://user-images.githubusercontent.com/25304220/154548705-81940618-fe8c-4789-918c-35121866a583.png)

### Auto-refresh
Lancer cette commande dans `vim`, le PDF sera regénéré automatiquement.
![image](https://user-images.githubusercontent.com/25304220/154555133-554fc6a5-0fb7-4dcd-a5c1-ad61e8514ef5.png)

```vim
autocmd BufWritePost *.tex silent! execute "!pdflatex -shell-escape % >/dev/null 2>&1" | redraw!
```

[SKIM](https://skim-app.sourceforge.io/) permet de visualiser le pdf avec l'auto-refresh en activant ces paramètres dans le viewer:
![image](https://user-images.githubusercontent.com/25304220/154555904-3a77e7db-62ba-4dd2-837d-8861b8cd6d8e.png)

