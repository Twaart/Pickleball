# Round Robin Pickleball – Guía de uso

🌐 [Français](Readme.md) · [English](Readme.en.md) · **Español** · [Deutsch](Readme.de.md)

Herramienta web para organizar un **round robin** amistoso de pickleball (los compañeros cambian en cada ronda). Genera una tarjeta para cada jugador que indica, en cada ronda, la cancha y el lado: **Mur** (lado de la pared) o **Rideau** (lado de la cortina).

**Enlace de la herramienta:** https://github.com/Twaart/Pickleball/blob/2918a3beeff2d3c8ef754905c754ddcd4b3e9579/Round%20Robin%20Pickleball.html

> **Nota:** la interfaz de la herramienta está en francés. Los nombres de botones y etiquetas se indican abajo en francés, con su significado en español entre paréntesis.

---

## Lo que garantiza la herramienta

- Cada jugador juega **la mitad de sus rondas en el lado Mur** y la otra mitad en el lado Rideau (con una diferencia de ±1 ronda si el número de rondas jugadas es impar).
- Los **compañeros cambian** en cada ronda: se evita que un jugador vuelva a formar pareja con el mismo compañero.
- Los **rivales se reparten lo más equitativamente posible**.
- Los jugadores se distribuyen de forma justa entre las canchas.

> Para la configuración original (12 jugadores, 3 canchas, sin vínculos), el calendario se verificó por cálculo: ningún compañero repetido ni ningún rival repetido en 4 rondas. Con 6 y 8 rondas, algunos rivales se enfrentan necesariamente más de una vez (hay más rondas que rivales posibles).

---

## Uso básico

1. **Elija el número de rondas** con los botones **4 manches**, **6 manches** u **8 manches** (4, 6 u 8 rondas).
2. **Elija la vista:**
   - **Cartes** (Tarjetas): una tarjeta por jugador (ronda, cancha, lado). Útil para repartir o mostrar las tarjetas.
   - **Grille par manche** (Cuadro por ronda): para cada ronda, los equipos de cada cancha (lado Mur / lado Rideau) y los jugadores en pausa. Útil para el organizador.
3. **Imprima** con el botón **Imprimer** (Imprimir). Los ajustes y botones se ocultan al imprimir. El resultado impreso no se ha probado: revise la vista previa antes de imprimir.

La línea gris bajo los botones resume la calidad del calendario (equilibrio Mur/Rideau, compañeros repetidos, rivales que se enfrentan más de una vez).

---

## Ajustes: « Joueurs, terrains et jumelages » (Jugadores, canchas y vínculos)

Abra la sección para acceder a las opciones.

### Número de jugadores y de canchas

- **Joueurs** (Jugadores): de 4 a 40.
- **Terrains** (Canchas): de 1 a 10.
- Se necesitan **4 jugadores por cancha** (2 contra 2). Si hay más jugadores que plazas, los demás quedan **en pausa** («Pause») en cada ronda, repartidos de forma equitativa. En la tarjeta, esa ronda muestra «—» y «Pause».
- Si hay demasiadas canchas para el número de jugadores, las sobrantes se ignoran (por ejemplo, 12 jugadores en 5 canchas solo usan 3). La página lo indica.
- Las canchas se llaman **T1, T2, T3…** y no se pueden renombrar.

### Nombres de los jugadores

Escriba un nombre en cada campo. Los nombres aparecen de inmediato en las tarjetas y en el cuadro. Un campo vacío muestra «Joueur n» (Jugador n).

### Vincular jugadores

Para que dos jugadores sean **compañeros en todas las rondas** (por ejemplo, para entrenar juntos de cara a un torneo):

1. Elija a los dos jugadores en las dos listas.
2. Pulse **Jumeler** (Vincular).
3. El calendario se recalcula en unos segundos.

Reglas:

- Un jugador solo puede vincularse **una vez**.
- El número de vínculos está limitado a **2 por cancha en uso** (por ejemplo, 6 vínculos como máximo con 3 canchas). Si se supera, la página muestra un mensaje.
- Para quitar un vínculo, haga clic en la **×** de su etiqueta.
- **Nouveau tirage** (Nuevo sorteo) vuelve a ejecutar el cálculo para obtener otro calendario. Es útil cuando aparece la advertencia ⚠.

---

## Mensajes y advertencias

| Mensaje | Significado |
|---|---|
| «Calcul de l'horaire en cours…» (Calculando el calendario…) | El cálculo se hace en su navegador (unos segundos, más con muchos jugadores). |
| ⚠ *partenaire(s) répété(s)* (compañero(s) repetido(s)) | Algunos compañeros se repiten. A veces es inevitable (véase abajo). Pruebe **Nouveau tirage**. |
| «Trop de jumelages…» (Demasiados vínculos…) | Reduzca el número de vínculos o añada canchas. |
| ⚠ *Mur / Rideau non équilibrés* (no equilibrados) | El cálculo no logró el equilibrio. Use **Nouveau tirage**. |

**¿Por qué pueden repetirse los compañeros?** Con pocos jugadores sin vincular, el número de compañeros posibles es limitado. Por ejemplo, con 3 vínculos entre 12 jugadores quedan 6 jugadores libres: cada uno solo tiene 5 compañeros posibles, lo que no basta para 6 rondas.

---

## Limitaciones

- Solo la configuración original (12 jugadores, 3 canchas, sin vínculos) usa el calendario verificado. Todas las demás configuraciones se calculan en la página mediante una búsqueda aleatoria optimizada. Respeta el equilibrio Mur/Rideau y evita compañeros repetidos en la mayoría de los casos, pero el resultado puede variar de un sorteo a otro.
- Los nombres, el número de jugadores, el número de canchas y los vínculos se guardan **en su navegador** (solo en su dispositivo). No se comparten con otras personas que abran el enlace.
- Los calendarios personalizados (distintos de la configuración original) se recalculan al recargar la página.
- Los PDF proporcionados por separado (4, 6 y 8 rondas) **no** incluyen nombres ni vínculos: solo la página web los tiene en cuenta.

---

## Consejos para el día del torneo

1. Introduzca los nombres de los jugadores y los posibles vínculos.
2. Elija el número de rondas según el tiempo disponible.
3. Si hace falta, pulse **Nouveau tirage** hasta obtener un calendario sin advertencias.
4. Muestre la **Grille par manche** en una pantalla para el organizador y reparta o muestre las **Cartes**.
