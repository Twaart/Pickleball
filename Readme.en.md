# Round Robin Pickleball – User Guide

🌐 [Français](Readme.md) · **English** · [Español](Readme.es.md) · [Deutsch](Readme.de.md)

A web tool for organizing a friendly pickleball **round robin** (partners change every round). It produces a card for each player showing, for every round, the court and the side: **Mur** (wall side) or **Rideau** (curtain side).

**Tool link:** https://claude.ai/artifact/9ij2y181uVvrZoX9d7uSkZ

> **Note:** the tool's interface is in French. Button and label names are given below in French, with the English meaning in parentheses.

---

## What the tool guarantees

- Each player plays **half of their rounds on the Mur side** and half on the Rideau side (within ±1 round if the number of rounds played is odd).
- **Partners change** every round: a player should not be paired with the same partner twice.
- **Opponents are spread as evenly as possible.**
- Players are distributed fairly across courts.

> For the original setup (12 players, 3 courts, no links), the schedule was verified by computation: no repeated partner and no repeated opponent over 4 rounds. With 6 and 8 rounds, some opponents necessarily meet more than once (there are more rounds than possible opponents).

---

## Basic use

1. **Choose the number of rounds** with the buttons **4 manches**, **6 manches** or **8 manches** (4, 6 or 8 rounds).
2. **Choose the view:**
   - **Cartes** (Cards): one card per player (round, court, side). Handy for handing out or displaying cards.
   - **Grille par manche** (Grid by round): for each round, the teams on every court (Mur side / Rideau side) and the players sitting out. Handy for the organizer.
3. **Print** with the **Imprimer** (Print) button. Settings and buttons are hidden when printing. Print rendering has not been tested: check the preview before printing.

The grey line under the buttons summarizes the schedule's quality (Mur/Rideau balance, repeated partners, opponents meeting more than once).

---

## Settings: "Joueurs, terrains et jumelages" (Players, courts and links)

Open the section to access the options.

### Number of players and courts

- **Joueurs** (Players): 4 to 40.
- **Terrains** (Courts): 1 to 10.
- You need **4 players per court** (2 vs 2). If there are more players than spots, the others **sit out** ("Pause") each round, shared out fairly. On the card, that round shows "—" and "Pause".
- If there are too many courts for the number of players, the extra courts are ignored (for example, 12 players on 5 courts use only 3). The page tells you so.
- Courts are named **T1, T2, T3…** and cannot be renamed.

### Player names

Type a name in each field. Names appear immediately on the cards and in the grid. An empty field shows "Joueur n" (Player n).

### Linking players

To make two players **partners in every round** (for example to practice together for a tournament):

1. Pick the two players in the two lists.
2. Press **Jumeler** (Link).
3. The schedule is recalculated in a few seconds.

Rules:

- A player can be linked **only once**.
- The number of links is limited to **2 per court in use** (for example, at most 6 links for 3 courts). Beyond that, the page shows a message.
- To remove a link, click the **×** on its chip.
- **Nouveau tirage** (New draw) reruns the calculation to get a different schedule. Useful when the ⚠ warning appears.

---

## Messages and warnings

| Message | Meaning |
|---|---|
| "Calcul de l'horaire en cours…" (Calculating the schedule…) | The calculation runs in your browser (a few seconds, longer with many players). |
| ⚠ *partenaire(s) répété(s)* (repeated partner(s)) | Some partners come back. This is sometimes unavoidable (see below). Try **Nouveau tirage**. |
| "Trop de jumelages…" (Too many links…) | Reduce the number of links or add courts. |
| ⚠ *Mur / Rideau non équilibrés* (not balanced) | The calculation did not reach balance. Use **Nouveau tirage**. |

**Why can partners repeat?** With few unlinked players, the number of possible partners is limited. For example, with 3 links among 12 players, 6 free players remain: each has only 5 possible partners, which is not enough for 6 rounds.

---

## Limitations

- Only the original setup (12 players, 3 courts, no links) uses the verified schedule. All other setups are calculated in the page by an optimized random search. It respects the Mur/Rideau balance and avoids repeated partners in most cases, but the result can vary from one draw to the next.
- Names, number of players, number of courts and links are stored **in your browser** (on your device only). They are not shared with other people who open the link.
- Custom schedules (anything other than the original setup) are recalculated when you reload the page.
- The separately provided PDFs (4, 6 and 8 rounds) do **not** contain names or links: only the web page takes them into account.

---

## Tips for tournament day

1. Enter the player names and any links.
2. Choose the number of rounds according to the time available.
3. If needed, press **Nouveau tirage** until you get a schedule with no warning.
4. Show the **Grille par manche** on a screen for the organizer, and hand out or display the **Cartes**.
