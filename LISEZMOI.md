# Séparateurs Moodle — J'apprends, Je découvre, Je me teste, J'applique

Un seul fichier (`separateur.html`) affiche les 4 séparateurs. Moodle l'affiche dans un cadre (iframe).
Modifier ce fichier sur GitHub modifie les séparateurs dans **tous** les cours, Bac Pro et BTS.

## Contenu du dossier

| Fichier | Rôle |
|---|---|
| `separateur.html` | Le séparateur. Style en haut, textes / couleurs / GIF en bas. |
| `gif/` | Les 4 GIF animés 50×50. |
| `index.html` | Page de test qui affiche les 4 séparateurs dans une section verte. |

## 1. Mettre en ligne sur GitHub Pages

1. Sur GitHub, créer un dépôt **public** nommé `separateurs-moodle`.
2. Y déposer le contenu du dossier (glisser-déposer `separateur.html`, `index.html` et le dossier `gif`).
3. Dans le dépôt : **Settings › Pages** › Source : *Deploy from a branch* › Branche `main`, dossier `/ (root)` › **Save**.
4. Attendre 1 à 2 minutes, puis ouvrir `https://TONPSEUDO.github.io/separateurs-moodle/` : la page de test doit afficher les 4 séparateurs.

## 2. Code à coller dans Moodle

Dans une **Zone texte et média**, ouvrir le **code source** de l'éditeur et coller **une** de ces lignes
(remplacer `TONPSEUDO` par ton nom d'utilisateur GitHub) :

```html
<iframe src="https://TONPSEUDO.github.io/separateurs-moodle/separateur.html?p=decouvre" title="Je découvre" scrolling="no" style="width:100%;height:64px;border:0;display:block;"></iframe>
```

```html
<iframe src="https://TONPSEUDO.github.io/separateurs-moodle/separateur.html?p=apprends" title="J'apprends" scrolling="no" style="width:100%;height:64px;border:0;display:block;"></iframe>
```

```html
<iframe src="https://TONPSEUDO.github.io/separateurs-moodle/separateur.html?p=teste" title="Je me teste" scrolling="no" style="width:100%;height:64px;border:0;display:block;"></iframe>
```

```html
<iframe src="https://TONPSEUDO.github.io/separateurs-moodle/separateur.html?p=applique" title="J'applique" scrolling="no" style="width:100%;height:64px;border:0;display:block;"></iframe>
```

## 3. Modifier tous les séparateurs d'un coup

- **Police, taille, épaisseur des lignes** : bloc `RÉGLAGES COMMUNS` en haut de `separateur.html`.
- **Texte ou couleur d'une phase** : bloc `PHASES` en bas de `separateur.html`.
- **Changer un GIF** : remplacer le fichier dans `gif/` en gardant le même nom.

Après un dépôt sur GitHub, la mise à jour apparaît dans Moodle en quelques minutes
(actualiser avec Ctrl+F5 si l'ancienne version reste affichée).

⚠️ Ne pas changer les clés `decouvre`, `apprends`, `teste`, `applique` : ce sont elles que les liens Moodle utilisent.
Pour ajouter une nouvelle phase, ajouter une ligne dans `PHASES` avec une nouvelle clé.
