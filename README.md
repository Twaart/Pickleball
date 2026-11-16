# Round Robin Pickleball – Guide d'utilisation

🌐 **Français** · [English](Readme.en.md) · [Español](Readme.es.md) · [Deutsch](Readme.de.md)

Outil web pour organiser un tournoi amical de pickleball en **round robin** (partenaires qui changent à chaque manche). Il produit les cartes de chaque joueur : à chaque manche, le terrain et le côté (**Mur** ou **Rideau**).

**Lien de l'outil :** 

---

## Ce que l'outil garantit

- Chaque joueur joue **la moitié de ses manches côté Mur** et l'autre moitié côté Rideau (à ±1 manche près si le nombre de manches jouées est impair).
- Les **partenaires changent** à chaque manche : on évite qu'un joueur retombe avec le même partenaire.
- Les **adversaires sont répartis le plus également possible**.
- Les joueurs sont répartis de façon équitable sur les terrains.

> Pour la configuration d'origine (12 joueurs, 3 terrains, sans jumelage), l'horaire a été vérifié par calcul : aucun partenaire répété et aucun adversaire répété en 4 manches. En 6 et 8 manches, certains adversaires se croisent forcément plus d'une fois (il y a plus de manches que d'adversaires possibles).

---

## Utilisation de base

1. **Choisir le nombre de manches** avec les boutons **4 manches**, **6 manches** ou **8 manches**.
2. **Choisir l'affichage :**
   - **Cartes** : une carte par joueur (manche, terrain, côté). Utile pour distribuer ou afficher les cartes.
   - **Grille par manche** : pour chaque manche, les équipes de chaque terrain (côté Mur / côté Rideau) et les joueurs en pause. Utile pour l'organisateur.
3. **Imprimer** avec le bouton **Imprimer** (les réglages et boutons sont masqués à l'impression). Le rendu à l'impression n'a pas été testé : vérifiez l'aperçu avant d'imprimer.

La ligne grise sous les boutons résume la qualité de l'horaire (équilibre Mur/Rideau, partenaires répétés, adversaires qui se croisent plus d'une fois).

---

## Réglages : « Joueurs, terrains et jumelages »

Ouvrez la section pour accéder aux options.

### Nombre de joueurs et de terrains

- **Joueurs :** de 4 à 40.
- **Terrains :** de 1 à 10.
- Il faut **4 joueurs par terrain** (2 contre 2). S'il y a plus de joueurs que de places, les autres sont **en pause** à chaque manche, avec une répartition équitable. Sur la carte, la manche affiche alors « — » et « Pause ».
- S'il y a trop de terrains pour le nombre de joueurs, les terrains en trop sont ignorés (par exemple, 12 joueurs sur 5 terrains n'en utilisent que 3). La page l'indique.
- Les terrains sont nommés **T1, T2, T3…** (ils ne peuvent pas être renommés).

### Noms des joueurs

Saisissez un nom dans chaque champ. Les noms apparaissent immédiatement sur les cartes et dans la grille. Un champ vide affiche « Joueur n ».

### Jumeler des joueurs

Pour que deux joueurs soient **partenaires à toutes les manches** (par exemple pour s'entraîner en vue d'un tournoi) :

1. Choisissez les deux joueurs dans les deux listes.
2. Appuyez sur **Jumeler**.
3. L'horaire est recalculé en quelques secondes.

Règles à connaître :

- Un joueur ne peut être jumelé **qu'une seule fois**.
- Le nombre de jumelages est limité à **2 par terrain utilisé** (par exemple 6 jumelages au maximum pour 3 terrains). Au-delà, la page affiche un message.
- Pour retirer un jumelage, cliquez sur le **×** de la pastille correspondante.
- **Nouveau tirage** relance le calcul pour obtenir un autre horaire. C'est utile si l'avertissement ⚠ s'affiche.

---

## Messages et avertissements

| Message | Signification |
|---|---|
| « Calcul de l'horaire en cours… » | Le calcul se fait dans votre navigateur (quelques secondes, davantage avec beaucoup de joueurs). |
| ⚠ *partenaire(s) répété(s)* | Certains partenaires reviennent. C'est parfois inévitable (voir ci-dessous). Essayez **Nouveau tirage**. |
| « Trop de jumelages… » | Réduisez le nombre de jumelages ou ajoutez des terrains. |
| ⚠ *Mur / Rideau non équilibrés* | Le calcul n'a pas atteint l'équilibre. Utilisez **Nouveau tirage**. |

**Pourquoi des partenaires peuvent-ils se répéter ?** Avec peu de joueurs non jumelés, le nombre de partenaires possibles est limité. Par exemple, avec 3 jumelages sur 12 joueurs, il reste 6 joueurs libres : chacun n'a que 5 partenaires possibles, ce qui est insuffisant pour 6 manches.

---

## Limites

- Seule la configuration d'origine (12 joueurs, 3 terrains, sans jumelage) reprend l'horaire déjà vérifié. Toutes les autres configurations sont calculées dans la page par une recherche aléatoire optimisée. Elle respecte l'équilibre Mur/Rideau et évite les partenaires répétés dans la plupart des cas, mais le résultat peut varier d'un tirage à l'autre.
- Les noms, le nombre de joueurs, le nombre de terrains et les jumelages sont mémorisés **dans votre navigateur** (sur votre appareil seulement). Ils ne sont pas partagés avec les autres personnes qui ouvrent le lien.
- Les horaires personnalisés (autres que la configuration d'origine) sont recalculés si vous rechargez la page.
- Les PDF fournis séparément (4, 6 et 8 manches) ne contiennent **pas** les noms ni les jumelages : seule la page web les prend en compte.

---

## Conseil d'utilisation le jour du tournoi

1. Saisissez les noms des joueurs et les éventuels jumelages.
2. Choisissez le nombre de manches selon le temps disponible.
3. Si besoin, appuyez sur **Nouveau tirage** jusqu'à obtenir un horaire sans avertissement.
4. Ouvrez la **Grille par manche** sur un écran pour l'organisateur, et distribuez ou affichez les **Cartes**.
