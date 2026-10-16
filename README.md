# REDLINE – gemeinsamer Familienkalender

Eigenständige Website (keine Verbindung zu Frost Skaters), mit Schwarz-Rot-Design.

## Website

https://raphifrost.github.io/Family-team/

> **GitHub Pages muss aktiv sein.** Falls die Adresse noch einen 404-Fehler zeigt: Im Repository unter **Settings → Pages** bei **Build and deployment** die Quelle **Deploy from a branch**, Branch **main**, Ordner **/(root)** auswählen und speichern. Die automatische Veröffentlichungs-Action ist zusätzlich vorhanden.

## Gemeinsam nutzen

1. Auf jedem Gerät die Website öffnen.
2. Jeweils mit einer eigenen E-Mail-Adresse einen Anmeldelink anfordern.
3. Wenn der Link nicht auf REDLINE zurückleitet: **den vollständigen Link aus der eigenen E-Mail kopieren**, auf der REDLINE-Seite ins Feld „Anmeldelink aus E-Mail einfügen“ eintragen und dort bestätigen. Geheimen Login-Link nicht in Chats verschicken.
4. Die erste Person erstellt ein Team (z. B. „Familie“) und trägt ihren Anzeigenamen ein.
5. Im Team-Bereich auf **Einladungslink verschicken** tippen. Nur an vertrauenswürdige Personen schicken.
6. Zweite Person öffnet den Link, meldet sich an und tritt dem Team mit Anzeigenamen bei.
7. Kalender und Aufgaben werden zwischen allen Mitgliedern dieses Teams synchronisiert. Neue Termine lassen sich jeweils anderen Mitgliedern zuweisen.

## Bisherige Termine von den Handys

Auf einem Handy, auf dem zuvor **Demo-Termine** erstellt wurden, bietet REDLINE nach Team-Beitritt **„Alte Termine übernehmen“** an. Die Person entscheidet selbst, ob sie ihre eigenen bisherigen Termine ins gemeinsame Team übertragen will. Diese werden dann für das Team sichtbar und standardmäßig dieser Person zugeordnet. Beispieltermine werden nicht importiert. Die lokalen Daten bleiben erhalten.

Alternative: **Mein Account → Alte Demo-Termine übernehmen**.

## Erinnerungen

Solange die Seite geöffnet ist: Browser-Erinnerungen nach Berechtigung. Über die Kalender-Exportfunktion können Termine auch in den Geräte-Kalender übernommen werden. **Echte Push-Benachrichtigungen bei geschlossener Website sind noch nicht eingerichtet.**

## Technik und Datenschutz

- Neues, eigenständiges Supabase-Projekt **REDLINE** (Region Frankfurt, Deutschland). 
- Tabellen: `redline_teams`, `team_members`, `team_events`, `team_tasks`.
- Alle Teamtabellen haben Row Level Security, eingeladene Benutzer müssen angemeldet sein.
- Ein Teamcode ist eine geheime Einladung; andere Teams haben keinen Zugriff.
- Nur ein **öffentlicher Publishable Key**, kein Service-Key, ist in der Seite hinterlegt.
- Ein Anmeldelink aus einer E-Mail ist geheim und darf nicht weitergegeben werden.
- Der GitHub-Code ist öffentlich; **Termine und Aufgaben sind nicht in GitHub gespeichert**.
