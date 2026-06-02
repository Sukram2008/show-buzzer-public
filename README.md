# Show Buzzer System 🚀

Willkommen beim **Show Buzzer System**! Diese Anwendung bietet eine interaktive Komplettlösung für Live-Quiz-Shows und Gewinnspiele. Mit Echtzeit-Buzzern, einer zentralen Admin-Steuerung und nahtloser OBS-Integration behältst du jederzeit den Überblick.

## 📑 Inhaltsverzeichnis
1. [Allgemeine Übersicht](#allgemeine-übersicht)
2. [Spieler-Panel](#spieler-panel)
3. [Admin-Panel](#admin-panel)
4. [OBS-Integration](#obs-integration)
5. [Roadmap & Features](#roadmap--features)

---

## 🌍 Allgemeine Übersicht
<a id="allgemeine-übersicht"></a>
Das Show Buzzer System nutzt eine hochperformante **Supabase-Datenbank**, um alle Aktionen in Echtzeit zwischen den Teilnehmern und dem Moderator zu synchronisieren.

* **Echtzeit-Synchronisation:** Egal ob Buzzer-Events oder Punktevergabe – alle Änderungen sind sofort auf allen verbundenen Geräten sichtbar.
* **Plattform-unabhängig:** Das System läuft browserbasiert auf jedem Gerät (Smartphone, Tablet, Desktop) – kein App-Download erforderlich.

---

## 🎮 Spieler-Panel
<a id="spieler-panel"></a>
Das Spielfeld für die Teilnehmer.
* **URL:** [show-buzzer.vercel.app/home](https://show-buzzer.vercel.app/home)
* **Funktionen:**
    * **Raum-Login:** Sicherer Beitritt über einen individuellen Raum-Code.
    * **Interaktiver Buzzer:** Ein responsiver, großflächiger Buzzer-Button.
    * **Live-Feedback:** Sofortige visuelle Bestätigung bei erfolgreichem Buzzer-Event.
    * **Eingabefeld:** Ermöglicht die Übermittlung von Antworten oder weiteren Informationen direkt an das Admin-Panel.

---

## ⚙️ Admin-Panel
<a id="admin-panel"></a>
Das Kontrollzentrum für den Moderator.
* **URL:** [show-buzzer.vercel.app/admin](https://show-buzzer.vercel.app/admin)
* **Funktionen:**
    * **Raum-Verwaltung:** Erstellung, Konfiguration und effiziente Steuerung deiner Spielräume.
    * **Teilnehmer-Management:** Übersicht aller angemeldeten Spieler inklusive Team-Zuordnungen.
    * **Punktesystem:** Intuitive manuelle Punktevergabe und globale Reset-Funktionen.
    * **Buzzer-Steuerung:** Zentrales Zurücksetzen aller Buzzer-Events für neue Spielrunden oder Fragen.
    * **Sicherheits-Layer:** Beitritts-Status (Lock/Unlock) in Echtzeit steuern.

---

## 📺 OBS-Integration (BETA)
<a id="obs-integration"></a>
Bringe deine Quiz-Show direkt in deinen Stream.
* **URL-Generator:** *Coming soon*
* **Einbindung:** Füge den bereitgestellten Link einfach als **Browser-Quelle** in OBS Studio hinzu.
* **Dynamische Parameter:**
    * `transparent=true`: Aktiviert den modernen Glas-Look für Overlays.
    * `hideName=true`: Blendet Spielernamen für anonymisierte Ranglisten aus.
* **Status:** *Dieses Feature befindet sich aktuell in der aktiven Entwicklung.*

---

## 🚧 Roadmap & Features
<a id="roadmap--features"></a>
Wir entwickeln das System stetig weiter:

* [ ] **Zeitsteuerung:** Automatisierte Freigabe von Buzzern und Eingabefeldern über konfigurierbare Timer.
* [ ] **Erweiterter Team-Modus:** Komplexe Team-Logik und gemeinschaftliche Punkteverwaltung.
* [ ] **Automatisches Punkte-System:** Richtig/Falsch-Feedback inklusive automatischer Score-Vergabe.
* [ ] **Live-Ranglisten:** Automatisch generierte Bestenlisten als Overlay für den Stream.
* [ ] **Konfigurations-Hub:** Individuelle Anpassung der Gewichtung und Spielregeln pro Raum.

---

*Entwickelt für spannende Live-Quiz-Events!*
