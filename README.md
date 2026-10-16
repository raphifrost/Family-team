# REDLINE — Familien- und Teamplaner

Eine unabhängige schwarz-rote Website mit Terminkalender, getrennten Spalten für Mitglieder, Aufgaben und Erinnerungen.

## Website

Nach erfolgreicher GitHub-Pages-Bereitstellung: https://raphifrost.github.io/Family-team/

## Aktueller Stand

Die Website ist zunächst als **lokale Demo** online. Du kannst Termine, Aufgaben und zusätzliche Beispielmitglieder anlegen. Diese Inhalte werden im Browser des jeweiligen Geräts gespeichert und **nicht zwischen Personen geteilt**.

Für echtes gemeinsames Arbeiten müssen wir ein **eigenständiges neues Supabase-Projekt** anlegen und die geschützte Datenbank verbinden. Hierfür gibt es bereits eine vorbereitete Online-Version mit RLS und Einladungslinks. Die bestehende Frost-Skaters-Datenbank wird nicht verwendet.

**Erinnerungen:** Browser-Hinweise benötigen die geöffnete Website. Kalenderexport mit Erinnerung ist möglich; echte Push-Nachrichten bei geschlossener Website erfordern einen zusätzlichen Dienst.

## GitHub Pages

Ein GitHub-Actions-Workflow liegt unter `.github/workflows/deploy.yml` und versucht Pages automatisch zu aktivieren. Falls nötig, gehe auf **Settings → Pages** und wähle **GitHub Actions** als Build and Deployment-Quelle.

**Sicherheit:** Versende Einladungslinks nach Datenbankaktivierung nur an vertrauenswürdige Personen. Keine geheimen Zugangsdaten ins Repository laden.
