# Schichtplaner

Persönlicher Planer für das Zeitkonto (FSK) im Konti-Schichtmodell
2 Früh / 2 Spät / 2 Nacht / 4 frei.

- Jahresübersicht mit FSK-Verlauf, Monats- und Wochenansicht
- Tageseditor für Schicht, Urlaub, Krank, T-Zug, Zusatzschicht und mehr
- Automatische #-Tage, Feiertage Bayern
- Urlaubs- und T-Zug-Übersicht
- Login über Supabase (E-Mail + Passwort), jeder sieht nur seine eigenen Daten

## Einrichtung

1. `schichtplaner_setup.sql` einmalig im Supabase SQL Editor ausführen
   (die Datei liegt nicht im Repository).
2. In `index.html` ganz unten `SB_URL` und `SB_KEY` eintragen
   (Supabase → Project Settings → API, anon/publishable Key).
3. GitHub Pages aktivieren: Settings → Pages → Branch `main`, Ordner `/ (root)`.

Der anon/publishable Key darf öffentlich im Code stehen. Geschützt sind die
Daten durch den Login und die Sicherheitsregeln (Row Level Security) der Tabelle.

Ohne eingetragenen Key läuft das Tool lokal ohne Login.
