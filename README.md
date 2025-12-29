# 📋 FL-FeV - Fahrerlaubnis-Verordnung Editor

**Fahrlehrer-Ausbildung FL-BE_07/25**  


---

## 📚 Über dieses Repository

Dieses Repository enthält die Daten für den **FeV Editor** - ein professionelles Werkzeug zur systematischen Aufbereitung der Fahrerlaubnis-Verordnung (FeV) für die Fahrlehrer-Ausbildung.

Der Editor ermöglicht die strukturierte Erfassung von Gesetzestexten zu Führerscheinklassen, Eignungsprüfungen, Prüfungsverfahren, Praxisbeispielen und deren Synchronisation über GitHub.

---

## 📂 Repository-Struktur

```
FL-FeV/
├── README.md       (diese Datei - Projektbeschreibung)
└── data.json       (FeV-Daten, automatisch synchronisiert vom Editor)
```

---

## 🔄 Daten-Synchronisation

Die Datei `data.json` wird **automatisch** vom FeV Editor synchronisiert:

- ✅ Jedes Speichern im Editor aktualisiert diese Datei
- ✅ Änderungen werden mit Zeitstempel versioniert
- ✅ Team-Kollaboration möglich (mehrere Nutzer, ein Repository)

**⚠️ WICHTIG:** Die `data.json` sollte **nicht manuell bearbeitet** werden!  
Alle Änderungen bitte nur über den FeV Editor vornehmen.

---

## 🛠️ Verwendung

### 1. Repository-Setup (einmalig)
- Repository erstellt: ✅ `710Deckel/FL-FeV`
- README.md hochgeladen: ✅

### 2. Editor-Verwendung
- HTML-Datei lokal öffnen (`fev-editor.html`)
- GitHub Token eingeben (einmalig, gleicher Token wie andere Tools!)
- Paragraphen hinzufügen und speichern
- Automatische Synchronisation erfolgt

### 3. Token-Anforderungen
Der verwendete Token benötigt folgende Berechtigungen:
- ✅ `repo` (Full control of private repositories)

**Hinweis:** Du kannst denselben Token für alle Fahrlehrer-Tools verwenden!

---

## 📋 Datenstruktur

Die `data.json` enthält alle FeV-Paragraphen im folgenden Format:

```json
{
  "paragraphen": [
    {
      "id": "timestamp",
      "gesetz": "FeV",
      "nummer": "§ 6",
      "titel": "Einteilung der Fahrerlaubnisklassen",
      "gesetzestext": "...",
      "quelle": "https://...",
      "praxisbeispiele": [
        {
          "titel": "Beispiel",
          "klasse": "B",
          "beschreibung": "...",
          "wichtigkeit": "CRITICAL"
        }
      ]
    }
  ]
}
```

---

## 🎯 Features des Editors

- **2-Spalten-Layout:** Gesetzestext | Praxisbeispiele
- **GitHub Auto-Sync:** Automatische Synchronisation
- **Template-System:** Vordefinierte Beispiele für Führerscheinklassen, MPU, Prüfungen
- **Badge-System:** CRITICAL (rot) | HIGH (orange) | BANAL (grün)
- **PDF-Export:** Professionelle Druckausgabe
- **Import/Export:** JSON-Backup-System
- **Keyboard Shortcuts:** Strg+S zum Speichern
- **Lila Theme:** Speziell für Fahrerlaubnis-Themen

---

## 📋 Wichtige FeV-Bereiche

Der Editor deckt alle wichtigen Bereiche der Fahrerlaubnis-Verordnung ab:

- **§ 6 - Führerscheinklassen:** A, A1, A2, AM, B, B96, BE, C, C1, D, D1, L, T
- **§ 11 - Eignung:** MPU, medizinische Gutachten, Drogentests
- **§ 18 - Prüfung:** Theorie, Praxis, Grundfahraufgaben
- **§ 20 - Probezeit:** Verlängerung, Aufbauseminare
- **§ 28 - Umtausch:** Alte Führerscheine
- **§ 31 - Internationaler Führerschein**

---

## 🔗 Weitere Fahrlehrer-Tools

Dieses Repository ist Teil einer systematischen Tool-Suite für die Fahrlehrer-Ausbildung:

- [📘 FL-StVO](https://github.com/710Deckel/stvo-teleprompter) - StVO Teleprompter mit Erläuterungen
- [🚛 FL-FPersV-EG-VO](https://github.com/710Deckel/FL-FPersV-EG-VO) - Fahrpersonalverordnung & EU-Verordnung
- [⚖️ FL-StVG](https://github.com/710Deckel/FL-StVG) - Straßenverkehrsgesetz
- [🔧 FL-StVZO](https://github.com/710Deckel/FL-StVZO) - Straßenverkehrs-Zulassungs-Ordnung
- [📋 FL-FeV](https://github.com/710Deckel/FL-FeV) - Fahrerlaubnis-Verordnung (dieses Repository)
- [🚗 FL-FZV](https://github.com/710Deckel/FL-FZV) - Fahrzeug-Zulassungsverordnung

---

## 📝 Lizenz & Verwendung

**Projekt:** Fahrlehrer-Ausbildung FL-BE_07/25  
**Ersteller:** Justin Lee Probis   
**Zweck:** Ausbildung und Podcast "Fahrlehrer Inside"

Dieses Tool und die Daten sind für **Ausbildungszwecke** erstellt.

---

## 📞 Kontakt & Feedback

Bei Fragen, Problemen oder Verbesserungsvorschlägen:
- GitHub Issues in diesem Repository
- Feedback über das Tool (Thumbs Down Button)

---

**Erstellt mit ❤️ für die Fahrlehrer-Ausbildung**

*Letzte Aktualisierung: Dezember 2024*
