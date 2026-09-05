# Show Buzzer System 🚀

Willkommen beim **Show Buzzer System**! Diese Anwendung bietet eine interaktive Komplettlösung für Live-Quiz-Shows und Gewinnspiele. Mit Echtzeit-Buzzern, einer zentralen Admin-Steuerung, flexiblen Spieloptionen und nahtloser OBS-Integration behältst du jederzeit den Überblick.

## 📑 Inhaltsverzeichnis
1. [Allgemeine Übersicht](#allgemeine-übersicht)
2. [Spieler-Panel](#spieler-panel)
3. [Admin-Panel](#admin-panel)
4. [Leaderboard](#leaderboard)
5. [OBS-Integration](#obs-integration)
6. [Roadmap & Features](#roadmap--features)

---

## 🌍 Allgemeine Übersicht
<a id="allgemeine-übersicht"></a>

Das Show Buzzer System nutzt eine leistungsfähige **Neon PostgreSQL-Datenbank**, um Spielaktionen und Einstellungen zuverlässig zwischen Teilnehmern, Moderator und weiteren Ansichten zu synchronisieren.

* **Live-Synchronisation:** Buzzer-Events, Antworten, Punkte und Spielstände werden regelmäßig zwischen den verbundenen Geräten abgeglichen.
* **Plattform-unabhängig:** Das System läuft vollständig browserbasiert auf Smartphone, Tablet und Desktop – kein App-Download erforderlich.
* **Flexible Spielmodi:** Räume können individuell für Einzelspieler oder Teams sowie mit unterschiedlichen Buzzer-, Punkte- und Antwort-Einstellungen konfiguriert werden.
* **Runden-System:** Neue Spielrunden können jederzeit gestartet werden, ohne Teilnehmer, Teams oder bereits erspielte Punkte zu verlieren.
* **Zeitgesteuerte Runden:** Optional können Runden mit einem frei konfigurierbaren Zeitlimit gespielt werden.

---

## 🎮 Spieler-Panel
<a id="spieler-panel"></a>

Das Spielfeld für die Teilnehmer.

* **URL:** [show-buzzer.vercel.app/home](https://show-buzzer.vercel.app/home)
* **Funktionen:**
    * **Raum-Login:** Beitritt über einen individuellen Raum-Code.
    * **Spieler-Name:** Anmeldung mit eigenem Namen und optionaler Team-Zuordnung.
    * **Interaktiver Buzzer:** Ein responsiver, großflächiger Buzzer-Button für schnelle Eingaben.
    * **Live-Feedback:** Sofortige visuelle Rückmeldung über den eigenen Buzzer-Status.
    * **Antwortfeld:** Je nach Raum-Konfiguration können Antworten direkt übermittelt werden.
    * **Antwort-Status:** Bereits abgegebene Antworten werden eindeutig angezeigt und können entsprechend der Rundenlogik gesperrt werden.
    * **Punkteanzeige:** Je nach Einstellung können die eigenen Punkte bzw. Teampunkte angezeigt werden.
    * **Team-Anzeige:** Bei aktiviertem Team-Modus werden die eigene Gruppe und relevante Teammitglieder übersichtlich dargestellt.
    * **Runden-Timer:** Bei zeitgesteuerten Runden wird die verbleibende Zeit direkt im Spieler-Panel angezeigt.

---

## ⚙️ Admin-Panel
<a id="admin-panel"></a>

Das Kontrollzentrum für den Moderator.

* **URL:** [show-buzzer.vercel.app/admin](https://show-buzzer.vercel.app/admin)
* **Funktionen:**
    * **Raum-Verwaltung:** Erstellung, Konfiguration und Steuerung deiner Spielräume.
    * **Raum-Sicherheit:** Jeder Raum besitzt einen individuellen Raum-Code und ein geschütztes Admin-Passwort.
    * **Teilnehmer-Management:** Übersicht aller angemeldeten Spieler inklusive Team-Zuordnungen.
    * **Team-Verwaltung:** Erstellung und Verwaltung von Teams sowie Zuordnung der Spieler.
    * **Punktesystem:** Manuelle Punktevergabe mit frei konfigurierbaren Plus- und Minus-Werten.
    * **Individuelle Punktvergabe:** Punkte können weiterhin gezielt für einzelne Spieler gesetzt werden.
    * **Team-Punkte:** Optional können Punkte gemeinschaftlich auf Teamebene verwaltet werden.
    * **Buzzer-Steuerung:** Zentrales Zurücksetzen aller Buzzer für neue Spielrunden oder Fragen.
    * **Antwortverwaltung:** Übersicht und Verwaltung der eingereichten Antworten.
    * **Antwort-Sichtbarkeit:** Festlegen, ob Antworten niemandem, nur Teammitgliedern oder allen Spielern angezeigt werden.
    * **Punkte-Sichtbarkeit:** Festlegen, ob Punkte niemandem, nur Teammitgliedern oder allen Spielern angezeigt werden.
    * **Buzzer-Modus:** Auswahl zwischen nur einem erfolgreichen Buzzer oder der Möglichkeit für mehrere Spieler gleichzeitig.
    * **Text-Modus:** Auswahl zwischen Buzzer und Antwortfeld, nur Buzzer oder nur Antwortfeld.
    * **Zeitsteuerung:** Konfigurierbare Rundendauer mit automatischem Start und Ende.
    * **Spielstatus:** Räume können geöffnet, gesperrt, pausiert oder beendet werden.
    * **Spieler-Sichtbarkeit:** Spielernamen können für die Teilnehmeransicht ein- oder ausgeblendet werden.
    * **Neue Runde:** Startet eine neue Runde und setzt Buzzer sowie Antworten zurück, während Spieler, Teams und Punkte erhalten bleiben.
    * **Leaderboard-Konfiguration:** Aktivierung und Konfiguration einer öffentlichen Rangliste direkt über das Admin-Panel.
    * **Zugriffsschutz:** Leaderboards können über den Raum-Code, einen separaten Zugriffscode oder beide Varianten erreichbar gemacht werden.
    * **Freigabe-Link:** Für das Leaderboard kann direkt ein teilbarer Link generiert werden.

---

## 🏆 Leaderboard
<a id="leaderboard"></a>

Die öffentliche Rangliste für Zuschauer und Teilnehmer.

* **URL:** [show-buzzer.vercel.app/leaderboard](https://show-buzzer.vercel.app/leaderboard)
* **Funktionen:**
    * **Live-Rangliste:** Die aktuellen Punktestände werden automatisch aktualisiert.
    * **Team-Rangliste:** Bei aktiviertem Team-Scoring werden die Teams anstelle einzelner Spieler angezeigt.
    * **Spieler-Rangliste:** Ohne Team-Scoring werden die einzelnen Spieler mit ihren aktuellen Punkten angezeigt.
    * **Raum-Code:** Das Leaderboard kann über den Raum-Code aufgerufen werden, sofern diese Zugriffsmethode aktiviert wurde.
    * **Zugriffscode:** Alternativ kann ein separater Zugriffscode für das Leaderboard verwendet werden.
    * **Flexibler Zugriff:** Der Moderator kann zwischen Raum-Code, Zugriffscode oder beiden Zugriffsmöglichkeiten wählen.
    * **Kein Admin-Zugriff erforderlich:** Das Leaderboard ist als separate öffentliche Ansicht gedacht und benötigt kein Admin-Passwort.
    * **Automatische Aktualisierung:** Änderungen an den Punkteständen werden regelmäßig übernommen.

---

## 📺 OBS-Integration
<a id="obs-integration"></a>

Bringe deine Quiz-Show direkt in deinen Stream.

* **Einbindung:** Die OBS-Ansicht kann als **Browser-Quelle** in OBS Studio eingebunden werden.
* **Dynamische Darstellung:** Das System kann Informationen aus dem aktuellen Spielraum für Overlays bereitstellen.
* **Transparente Darstellung:** Unterstützt eine für Stream-Overlays geeignete Darstellung ohne störende Seitenelemente.
* **Status:** *Die OBS-Integration befindet sich aktuell in aktiver Entwicklung und wird weiter ausgebaut.*

---

## 🚧 Roadmap & Features
<a id="roadmap--features"></a>

Das System wird kontinuierlich weiterentwickelt. Bereits umgesetzte Funktionen werden dabei laufend erweitert und optimiert.

* [ ] **Erweiterte OBS-Overlays:** Umfangreiche und individuell konfigurierbare Darstellungen für Streams.
* [ ] **Automatisches Punkte-System:** Richtig/Falsch-Feedback inklusive automatischer Score-Vergabe.
* [ ] **Erweiterte Leaderboard-Optionen:** Weitere Darstellungsmöglichkeiten und Konfigurationsoptionen.
* [ ] **Erweiterte Spielregeln:** Noch mehr individuelle Einstellungen für unterschiedliche Quiz- und Show-Formate.
* [ ] **Statistiken:** Detaillierte Auswertungen zu Spielern, Teams, Buzzer-Events und Runden.
* [ ] **Weitere Spielmodi:** Unterstützung zusätzlicher Spielvarianten und Show-Formate.

---

*Entwickelt für spannende Live-Quiz-Events!*
