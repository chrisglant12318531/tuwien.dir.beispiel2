# PixelPaws Webshop - Projektbeschreibung

Dies ist die Dokumentation für den Webshop des Start-Ups **PixelPaws**, entwickelt im Rahmen der Übung "Webshop Entwicklung".

## 🚀 Aufgabe 0: Das Unternehmen & Konzept

### Das Produkt
PixelPaws vertreibt **digitale 3D-Druckvorlagen (STL-Dateien)** für Haustierzubehör.
* **Funktionen:** Download von optimierten Druckdateien (z. B. personalisierbare Anhänger, ergonomische Futterstationen, Spielzeug).
* **Zielgruppe:** Haustierbesitzer mit Zugang zu 3D-Druckern (Maker-Community), die Wert auf Individualität und DIY legen.

### Das Unternehmen
* **Name:** PixelPaws GmbH
* **Standort:** Linz, Österreich
* **Mitarbeiter:** 3 (Gründerteam: Design, Entwicklung, Marketing)

### Geschäftsmodell
* **Einmalverkauf (Pay-per-Download):** Kunden kaufen die Lizenz für eine spezifische Datei zur privaten Nutzung. Kein Abo-Modell.

---

## ♿ Aufgabe 1: Barrierefreiheit (WCAG 2.2 AA)

Die Website wurde unter strenger Einhaltung der WCAG 2.2 AA Richtlinien entwickelt.

* **Technische Umsetzung:**
    * **Semantisches HTML:** Verwendung von `<main>`, `<nav>`, `<header>`, `<article>` und `<button>` für korrekte Screenreader-Interpretation.
    * **Skip-Link:** Ein `Skip to content` Link (sichtbar bei Fokus) erlaubt Tastaturnutzern, die Navigation zu überspringen.
    * **Fokus-Management:** Ein deutlich sichtbarer Fokus-Indikator (`outline: 3px solid #F1C40F`) wurde implementiert (`:focus-visible`).
    * **Farbkontraste:** Das Farbschema (Dunkelblau auf Weiß/Hellgrau) erfüllt die Kontrastrate von mindestens 4.5:1 für Fließtext.
    * **Navigation:** Die simulierten Seitenwechsel (`showPage()`) setzen den Fokus aktiv auf den neuen Inhalt (`tabindex="-1"`), damit Screenreader den Kontextwechsel bemerken.
* **Tools:** Überprüft mit *WAVE Evaluation Tool* und manueller Tastatur-Navigation.

---

## ⚖️ Aufgabe 2: Urheberrecht & Mediennachweis

Um die Urheberrechtsvorgaben der Übung strikt einzuhalten und keine Rechte Dritter zu verletzen, wurde folgende Strategie gewählt:

### 1. Bilder & Grafiken
Für die Produktbilder werden **dynamische Platzhalter (Mockups)** über den Dienst `placehold.co` verwendet.

* **Quelle:** [https://placehold.co](https://placehold.co)
* **Lizenz:** Public Domain / Zur freien Nutzung.
* **Begründung:** Da es sich um ein fiktives Start-Up handelt und ich noch keine eigenen physischen Prototypen der 3D-Modelle fotografiert habe, vermeide ich durch die Nutzung von Platzhaltern jegliche Urheberrechtsverletzung ("Fremdnutzung" von Bildern aus dem Internet). Dies demonstriert das Bewusstsein für die Problematik der Bildrechte (Lichtbildwerk § 72 UrhG).
    *In einem realen Szenario würden diese Platzhalter durch eigene Fotografien der selbst gedruckten Objekte ersetzt werden.*

### 2. Schriftarten
* **Font:** "Open Sans"
* **Quelle:** Google Fonts
* **Lizenz:** Open Font License (OFL). Die kommerzielle und private Nutzung ist gestattet.

### 3. Icons (SVG)
* **Logo-Icon:** Inline SVG (Pfade).
* **Quelle:** Angelehnt an Open Source Icon Sets (wie Feather Icons), aber direkt als SVG-Code eingebettet.
* **Lizenz:** MIT License (erlaubt Nutzung und Modifikation).

---

## ®️ Aufgabe 3: Marke & Nizza-Klassen

### Markenform
Das Logo "PixelPaws" ist eine **Wort-Bild-Marke**, bestehend aus dem stilisierten Pfoten-Symbol (Bild) und dem Schriftzug "PixelPaws" (Wort).

### Nizza-Klassifikation
Die Marke würde in folgenden Klassen angemeldet werden:
1.  **Klasse 9:** Herunterladbare Software; digitale Dateien; 3D-Druckvorlagen.
2.  **Klasse 35:** Einzelhandel mit herunterladbaren digitalen Dateien; Online-Marktplatz.

### Markenschutz-Check
Eine Vorprüfung über *TMview* ergab keine identischen Eintragungen für "PixelPaws" im Bereich 3D-Druck in der EU (fiktives Szenario für die Übung).

---

## 📝 Aufgabe 4: Lizenz (EULA)

Siehe Abschnitt "Lizenz" auf der Website.
* **Rechte:** Der Kunde erwirbt ein einfaches Nutzungsrecht für den privaten 3D-Druck.
* **Ausschluss:** Weiterverkauf der digitalen Datei oder gewerblicher Verkauf der gedruckten Objekte ist untersagt.
* **Haftung:** Haftung für Druckerschäden oder Verletzungen durch das Objekt wird ausgeschlossen (da DIY-Herstellung).

---

## 🔒 Aufgabe 5 & 6: Datenschutz & Gewerbe

### Datenschutz
Die Datenschutzerklärung (siehe Website Abschnitt "Datenschutz") berücksichtigt:
* Art. 6 DSGVO (Vertragserfüllung als Rechtsgrundlage für Download).
* Minimale Datenerhebung (Data Minimization).
* Hinweis: Cookies sind im Code nur gemockt (technisch notwendig für Warenkorb-Simulation).

### Impressum
Das Impressum erfüllt § 5 ECG und § 24 Mediengesetz:
* Firmenbuchnummer & Gericht.
* UID-Nummer.
* Mitgliedschaft bei der WKO.
* Kontaktmöglichkeiten (E-Mail, Telefon).

---

## 🛠 Installation & Nutzung

Da es sich um eine reine Frontend-Simulation (Single Page Application via Vanilla JS) handelt, ist keine Server-Installation notwendig.

1.  Lade die Datei `index.html` herunter.
2.  Öffne die Datei in einem beliebigen modernen Webbrowser (Chrome, Firefox, Edge).
3.  Die Navigation erfolgt über das Menü, der Warenkorb ist eine JavaScript-Simulation (`alert`).
