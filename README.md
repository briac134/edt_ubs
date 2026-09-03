# Mon Planning UBS

Page web qui affiche l'emploi du temps Université Bretagne Sud à partir du lien d'export iCal généré par l'ENT. Le lien est enregistré dans le navigateur : une fois collé, il reste disponible au prochain rechargement.

## Récupérer le lien iCal depuis l'ENT

1. Se connecter à l'ENT UBS et ouvrir la rubrique **Planning / Emploi du temps**.
2. Dans le planning affiché, voir le menu **Options** (sous le menu de sélection de l'emploi du temps).
3. Cliquer sur le bouton **Exporter**.
4. Choisir l'export au format **iCalendar** et la période de temps voulu.
5. Copier le lien généré. Il ressemble à :
   ```
   https://planning.univ-ubs.fr/jsp/custom/modules/plannings/anonymous_cal.jsp?data=...,1
   ```

Ce lien est personnel : il donne accès en lecture à l'emploi du temps sans authentification. Il ne doit pas être partagé ni publié dans un dépôt public.

## Utiliser la page

1. Ouvrir https://briac134.github.io/edt_ubs/ 
2. Coller le lien copié dans le champ prévu.
3. Cliquer sur **Charger**.

Le lien est alors sauvegardé localement (`localStorage`) et sera réutilisé automatiquement aux prochaines ouvertures, même après fermeture de l'onglet. Le bouton **Oublier** permet de l'effacer.

## Remarque

Le lien iCal peut être régénéré côté ENT si besoin (nouvel export). Dans ce cas, il suffit de coller le nouveau lien dans la page pour remplacer l'ancien.
