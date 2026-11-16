# Round Robin Pickleball – Benutzerhandbuch

🌐 [Français](Readme.md) · [English](Readme.en.md) · [Español](Readme.es.md) · **Deutsch**

Ein Webtool zur Organisation eines freundschaftlichen Pickleball-**Round-Robin** (die Partner wechseln in jeder Runde). Es erstellt für jeden Spieler eine Karte, die für jede Runde das Feld und die Seite zeigt: **Mur** (Wandseite) oder **Rideau** (Vorhangseite).

**Link zum Tool:** https://github.com/Twaart/Pickleball/blob/2918a3beeff2d3c8ef754905c754ddcd4b3e9579/Round%20Robin%20Pickleball.html

> **Hinweis:** Die Oberfläche des Tools ist auf Französisch. Die Namen der Schaltflächen und Beschriftungen stehen unten auf Französisch, mit der deutschen Bedeutung in Klammern.

---

## Was das Tool garantiert

- Jeder Spieler spielt **die Hälfte seiner Runden auf der Seite Mur** und die andere Hälfte auf der Seite Rideau (mit einer Abweichung von ±1 Runde, wenn die Zahl der gespielten Runden ungerade ist).
- Die **Partner wechseln** in jeder Runde: Ein Spieler soll möglichst nicht zweimal mit demselben Partner spielen.
- Die **Gegner werden so gleichmäßig wie möglich verteilt**.
- Die Spieler werden fair auf die Felder verteilt.

> Für die ursprüngliche Konfiguration (12 Spieler, 3 Felder, keine Verknüpfungen) wurde der Spielplan rechnerisch überprüft: keine wiederholten Partner und keine wiederholten Gegner in 4 Runden. Bei 6 und 8 Runden treffen manche Gegner zwangsläufig mehr als einmal aufeinander (es gibt mehr Runden als mögliche Gegner).

---

## Grundlegende Nutzung

1. **Anzahl der Runden wählen** mit den Schaltflächen **4 manches**, **6 manches** oder **8 manches** (4, 6 oder 8 Runden).
2. **Ansicht wählen:**
   - **Cartes** (Karten): eine Karte pro Spieler (Runde, Feld, Seite). Praktisch zum Verteilen oder Anzeigen der Karten.
   - **Grille par manche** (Übersicht pro Runde): für jede Runde die Teams auf jedem Feld (Seite Mur / Seite Rideau) und die pausierenden Spieler. Praktisch für den Organisator.
3. **Drucken** mit der Schaltfläche **Imprimer** (Drucken). Einstellungen und Schaltflächen werden beim Drucken ausgeblendet. Der Ausdruck wurde nicht getestet: Prüfen Sie die Druckvorschau, bevor Sie drucken.

Die graue Zeile unter den Schaltflächen fasst die Qualität des Spielplans zusammen (Mur/Rideau-Ausgleich, wiederholte Partner, Gegner, die mehr als einmal aufeinandertreffen).

---

## Einstellungen: „Joueurs, terrains et jumelages" (Spieler, Felder und Verknüpfungen)

Öffnen Sie den Abschnitt, um die Optionen zu sehen.

### Anzahl der Spieler und Felder

- **Joueurs** (Spieler): 4 bis 40.
- **Terrains** (Felder): 1 bis 10.
- Pro Feld werden **4 Spieler** benötigt (2 gegen 2). Gibt es mehr Spieler als Plätze, **pausieren** die übrigen („Pause") in jeder Runde, fair verteilt. Auf der Karte zeigt diese Runde dann „—" und „Pause".
- Gibt es zu viele Felder für die Spielerzahl, werden die überzähligen Felder ignoriert (z. B. nutzen 12 Spieler auf 5 Feldern nur 3). Die Seite weist darauf hin.
- Die Felder heißen **T1, T2, T3 …** und können nicht umbenannt werden.

### Spielernamen

Geben Sie in jedes Feld einen Namen ein. Die Namen erscheinen sofort auf den Karten und in der Übersicht. Ein leeres Feld zeigt „Joueur n" (Spieler n).

### Spieler verknüpfen

Damit zwei Spieler **in jeder Runde Partner** sind (z. B. um gemeinsam für ein Turnier zu trainieren):

1. Wählen Sie die beiden Spieler in den beiden Listen aus.
2. Drücken Sie **Jumeler** (Verknüpfen).
3. Der Spielplan wird in wenigen Sekunden neu berechnet.

Regeln:

- Ein Spieler kann nur **einmal** verknüpft werden.
- Die Zahl der Verknüpfungen ist auf **2 pro genutztem Feld** begrenzt (z. B. höchstens 6 Verknüpfungen bei 3 Feldern). Darüber hinaus zeigt die Seite eine Meldung.
- Um eine Verknüpfung zu entfernen, klicken Sie auf das **×** des entsprechenden Etiketts.
- **Nouveau tirage** (Neue Auslosung) startet die Berechnung neu und liefert einen anderen Spielplan. Das ist nützlich, wenn die Warnung ⚠ erscheint.

---

## Meldungen und Warnungen

| Meldung | Bedeutung |
|---|---|
| „Calcul de l'horaire en cours…" (Spielplan wird berechnet…) | Die Berechnung läuft in Ihrem Browser (einige Sekunden, bei vielen Spielern länger). |
| ⚠ *partenaire(s) répété(s)* (wiederholte(r) Partner) | Einige Partner kehren wieder. Das ist manchmal unvermeidbar (siehe unten). Versuchen Sie **Nouveau tirage**. |
| „Trop de jumelages…" (Zu viele Verknüpfungen…) | Verringern Sie die Zahl der Verknüpfungen oder fügen Sie Felder hinzu. |
| ⚠ *Mur / Rideau non équilibrés* (nicht ausgeglichen) | Die Berechnung hat den Ausgleich nicht erreicht. Verwenden Sie **Nouveau tirage**. |

**Warum können sich Partner wiederholen?** Bei wenigen nicht verknüpften Spielern ist die Zahl der möglichen Partner begrenzt. Beispiel: Bei 3 Verknüpfungen unter 12 Spielern bleiben 6 freie Spieler; jeder hat nur 5 mögliche Partner, was für 6 Runden nicht reicht.

---

## Einschränkungen

- Nur die ursprüngliche Konfiguration (12 Spieler, 3 Felder, keine Verknüpfungen) verwendet den überprüften Spielplan. Alle anderen Konfigurationen werden in der Seite durch eine optimierte Zufallssuche berechnet. Sie beachtet den Mur/Rideau-Ausgleich und vermeidet wiederholte Partner in den meisten Fällen, aber das Ergebnis kann von Auslosung zu Auslosung variieren.
- Namen, Spieler- und Feldzahl sowie Verknüpfungen werden **in Ihrem Browser** gespeichert (nur auf Ihrem Gerät). Sie werden nicht mit anderen Personen geteilt, die den Link öffnen.
- Individuelle Spielpläne (alle außer der ursprünglichen Konfiguration) werden beim Neuladen der Seite neu berechnet.
- Die separat bereitgestellten PDFs (4, 6 und 8 Runden) enthalten **keine** Namen oder Verknüpfungen: Nur die Webseite berücksichtigt sie.

---

## Tipps für den Turniertag

1. Geben Sie die Spielernamen und eventuelle Verknüpfungen ein.
2. Wählen Sie die Rundenzahl passend zur verfügbaren Zeit.
3. Drücken Sie bei Bedarf **Nouveau tirage**, bis Sie einen Spielplan ohne Warnung erhalten.
4. Zeigen Sie die **Grille par manche** für den Organisator auf einem Bildschirm und verteilen oder zeigen Sie die **Cartes**.
