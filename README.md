# Transduktor

Mealy- und Moore-Automaten zeichnen, animieren, prüfen, umwandeln und minimieren. Alles steckt in einer einzigen `index.html` und läuft komplett im Browser: kein Server, kein Login, keine Daten, die irgendwohin hochgeladen werden.

## Funktionen

- Zeichnen mit Maus, Trackpad oder Finger: Doppelklick legt einen Zustand an, mit dem Plus am Zustand ziehst du eine Kante, und Beschriftungen lassen sich verschieben, um Kanten zu biegen.
- Übergangstabelle zum direkten Bearbeiten und eine Text-Kurzschreibweise (`q0 -> q1 : 1/n`), beide immer synchron mit dem Diagramm.
- Animation: Ein Token läuft über die Kanten, Eingabe- und Ausgabeband laufen mit, und die aktuelle Formel `δ(q, a)`, `λ(q, a)` steht live daneben.
- Prüfung auf Vollständigkeit, Determinismus und unerreichbare Zustände, jeweils mit Knopf zum Beheben.
- Mealy ↔ Moore umwandeln, Minimieren mit allen Zwischenschritten P0, P1, …
- Testfälle mit erwarteter Ausgabe und 5 Übungsaufgaben mit automatischer Kontrolle.
- Export als SVG, PNG, TikZ für LaTeX und JSON. Teilen per Link, der ganze Automat steckt dabei im Link.
- Hell- und Dunkelmodus, Touch-Bedienung, Rückgängig und Wiederholen, automatisches Speichern im Browser.

## Auf GitHub Pages veröffentlichen

1. Auf github.com ein neues öffentliches Repository anlegen, zum Beispiel `transduktor`.
2. Die Dateien aus diesem Ordner hochladen (`index.html`, `README.md`, `.nojekyll`). Das geht über „Add file → Upload files“.
3. Unter **Settings → Pages** bei „Source“ *Deploy from a branch* wählen, Branch `main`, Ordner `/ (root)`, speichern.
4. Nach etwa einer Minute ist die Seite unter `https://DEIN-NAME.github.io/transduktor/` erreichbar.

Die Schriften (Fira Sans, Fira Mono, Crimson Pro) kommen von Google Fonts. Ohne Internet greift die Seite auf Systemschriften zurück und funktioniert trotzdem.
