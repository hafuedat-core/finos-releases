# 🚀 HAFÜDAT FINANCIAL OPERATING SYSTEM
**Quick Start Guide & Navigation (v1.9.9 – Global Edition)**

> *"Stop managing finances. Find financial clarity. / Finde finanzielle Klarheit."*

---

## 🔒 Unabhängige Verifizierung & Sicherheit
Da es im Internet immer wieder Nachahmungen gibt, legen wir Wert auf maximale Transparenz. Du kannst die Echtheit unseres offiziellen Systems jederzeit überprüfen:

* **Offizieller Zahlungsabwickler:** Digistore24 GmbH (Verifiziert auf Trustpilot).
* **Offizieller Checkout-Link:** `https://www.checkout-ds24.com/product/725138` *(Achte bei Online-Käufen immer auf die originale Domain und SSL-Verschlüsselung)*.

### Zero-Trust: Wie du die Echtheit von FinOS prüfst
Wir setzen auf Vertrauen durch Mathematik. Jeder Release ist kryptografisch abgesichert und absolut manipulationssicher:

1. **Der digitale Fingerabdruck (SHA-256):** 
   Prüfe nach dem Download, ob der Hash deiner Datei mit dem Original übereinstimmt:
   `ea59b9d38656ab62fc6644eb7fb339622713eb8dc8d6e5723dcf1b30`
2. **Die PGP-Signatur:** 
   Unsere Releases sind signiert. Du kannst die Signatur mit unserem öffentlichen Schlüssel prüfen.
   **Offizielle PGP Key-ID:** `4804E907FF70AA60`

*(Eine Anleitung zur lokalen Verifizierung im Terminal findest du weiter unten).*

---

## 🛸 Phase 1: Ingestion (Die Einrichtung & Architektur)
Damit FinOS präzise arbeiten kann, braucht es einmalig deine Daten. Nimm dir dafür 10 Minuten Zeit.

### 1. System-Start & Plattform-Wahl
* **Google Sheets:** Erstelle dir über *Datei > Kopie erstellen* zuerst deine eigene, private Version in deinem Drive.
* **Lokal / Linux / PC:** Nutze die Datei völlig autark auf deinem Rechner – voll kompatibel mit Excel oder LibreOffice.
* **Der Ordner-Ansatz für die Ewigkeit:** Lege dir auf deiner Festplatte einen Hauptordner "Haushaltsbuch" an. Kopiere diese schlanke, unverschlüsselte Master-Datei einfach für jedes neue Jahr. 

### 2. Basic Settings (TAB 4 - Die Grundkonfiguration)
* **Time Zone (Zelle B2):** Trage hier deine Zeitzone ein (z. B. 1 für Mitteleuropa/Berlin) für die Server-Drift-Korrektur.
* **Salary & Wage (Zellen B4:C5):** Definiere deine Einkommensbeträge und Payout Days.
* **Explanation Mode & Language (Zellen B7:B8):** Aktiviere den Erklärmodus und wähle deine Sprache.
* *Integritäts-Check (Zeile 13):* Grüne Häkchen zeigen dir, ob die Kernstrukturen fehlerfrei intakt sind.

### 3. Config & Einkommen (TAB 3)
* Liste hier alle deine Fixkosten auf (Miete, Strom, Abos, Versicherungen).
* **Smart-Logic:** Nutze "Von" und "Bis", wenn ein Vertrag mitten im Jahr endet. Die Engine berechnet ab dem Folgemonat automatisch 0 €.

---

## ⚡ Phase 2: Daily Ops (Der Alltag)
FinOS ist für die **3-Sekunden-Erfassung** gebaut. Keine stundenlange Buchhaltung.

* **📅 Smart-Date-Logik:** Du musst das Datum nicht tippen. Lässt du das Datumsfeld leer, trägt FinOS automatisch das heutige Datum ein.
* **💳 Ausgaben erfassen (TAB 1):**
  * **Kartenzahlung (Bank Stream):** Betrag in H3 bis I33 eintragen.
  * **Bargeld abheben (ATM Transfer):** Betrag in Spalte B eintragen (Geld wandert virtuell zu "Wallet").
  * **Bargeld-Ausgaben (Wallet Stream):** Betrag in C3 bis G33 eintragen.
  * **Debit / Sub-Account:** Aufladung im Bank-Bereich eintragen, eigentliche Ausgaben im Debit-Bereich (J3:K33).

---

## 🛠️ Phase 3: Wartung & Monats-Reset
FinOS läuft endlos (*"Eternal Year Engine"*). Du brauchst keine neue Datei für den nächsten Monat. Am letzten Tag des Monats:

1. **Archivierung (TAB 2):** 
   * Kopiere die Zahlen von Zeile 32 -> füge sie als reine Werte in Zeile 33 (Tresor) ein.
   * Kopiere die Zahlen von Zeile 34 -> füge sie als reine Werte in Zeile 35 (Carryover) ein.
2. **Wipe (TAB 1):** Markiere den gesamten Eingabebereich (B3 bis I33) und drücke Entf (Löschen).
3. **Neustart:** Das System springt automatisch auf den neuen Monat um.

---

## ⚠️ Kernel Protection (Integritäts-Schutz)
* Siehst du farbige Warnungen? Nutze sofort die "Rückgängig"-Funktion (Strg+Z).
* **Regel:** Schreibe nur in Felder mit hellgrauem Rahmen oder weißer Schrift. 

---

## 📞 Support & Rechtliches
* **Kontakt:** `hafuedat@posteo.eu` *(Bitte bei technischen Anfragen Bestell-ID angeben)*
* **Nutzungshinweise (EULA):** Diese Datei ist für die private Nutzung lizenziert. Der kommerzielle Resell der "Eternal-Year-Engine" ist untersagt.
* **Disclaimer:** FinOS ist ein mathematisches Werkzeug zur Visualisierung. Wir übernehmen keine Haftung für finanzielle Entscheidungen oder Dateneingabefehler.
