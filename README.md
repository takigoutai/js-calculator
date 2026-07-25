#  Interaktiver Taschenrechner (JS Calculator)

Ein einfacher, moderner und benutzerfreundlicher Web-Taschenrechner, entwickelt mit **HTML5**, **CSS3** und **JavaScript (ES6)**. 

Dieses Projekt wurde erstellt, um die Grundlagen der DOM-Manipulation, Event-Handling und das Erstellen von responsiven Benutzeroberflächen zu demonstrieren.

---

###  Funktionen (Features)

- **Grundlegende Rechenarten:** Addition, Subtraktion, Multiplikation und Division.
- **Benutzerfreundliche Steuerung:** 
  - `C` Taste zum Löschen des gesamten Displays.
  - `DEL` Taste zum Entfernen der letzten Eingabe.
- **Responsive Design:** Ein modernes Dark-Theme, das auf allen Bildschirmgrößen gut aussieht.
- **Fehlerbehandlung:** Fängt ungültige mathematische Ausdrücke ab und zeigt eine Fehlermeldung an.

---

###  Verwendete Technologien

- **HTML5:** Strukturierung der Anwendung und Elemente.
- **CSS3:** Layout (CSS Grid & Flexbox), Dark-Mode Styling und Animationen.
- **JavaScript (Vanilla JS):** Logik für die Berechnungen und Event-Handling.

---

###  Code-Vorschau (JavaScript Logik)

```javascript
// Funktion zur Ausführung der Berechnung
function calculate() {
    try {
        display.value = eval(display.value);
    } catch (error) {
        display.value = 'Fehler';
        setTimeout(() => clearDisplay(), 1500);
    }
}
