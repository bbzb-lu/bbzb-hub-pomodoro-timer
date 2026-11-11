# BBZB Pomodoro Timer

> **Umgezogen (11.11.2026):** Dieses Embed liegt jetzt im Repo [bbzb-lu/bbzb-tools](https://github.com/bbzb-lu/bbzb-tools/tree/main/embeds/pomodoro-timer/) unter `embeds/pomodoro-timer/` und läuft unter https://bbzb-tools.pages.dev/sharepoint/pomodoro-timer/. Dieses Repo wird archiviert und nicht mehr gepflegt.

Pomodoro-Timer fürs Lernen: 25 Minuten arbeiten, 5 Minuten Pause, vier Runden bis zur langen Pause.

## In SharePoint einbetten

Das **Einbetten**-Webpart verwenden und den folgenden Code einfügen
(Embed-Code, **nicht** das URL-Feld):

```html
<iframe
  src="https://bbzb-lu.github.io/bbzb-hub-pomodoro-timer/"
  width="480"
  height="350"
  frameborder="0"
  scrolling="no"
  style="border:none;overflow:hidden;">
</iframe>
```

Auf dem Handy skaliert SharePoint den Container auf etwa 350 × 250 herunter.
Das Embed ist für beide Grössen ausgelegt und braucht keine Scrollbalken.

## Entwicklung

Statische Seite, kein Build-Schritt. Lokal testen:

```bash
python3 -m http.server 4321
# → http://localhost:4321
```

Über `file://` blockieren Browser die lokalen Schriften — immer über HTTP testen.

Design-Vorgaben, Assets und Prüfskript stehen in der Vorlage:
[bbzb-hub-template](https://github.com/bbzb-lu/bbzb-hub-template)
