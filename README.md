# sfgz_display
Shows Course-Datas on a screen with clock

Since sfgz_kursverwaltung 9.1.08 this part is outsourced to this own new extension **sfgz_display**.

----


Zeigt Kursdaten in enem Display

Seit sfgz_kursverwaltung 9.1.08 wurde dieser Teil ausgelagert und mit dieser neuen Extension **sfgz_display** relaisiert.

## Import-Funktionen
Die Kurse werden automatisch angezeigt, die Belegungen müssen erfasst/ausgewählt werden.

### Kurse
Importiert Kurse ab Kursverwaltung Extension sfgz_kurs. (Aktuell)
### Belegungen
Importiert Vorgabe-Belegungen ab 3 möglichen Quellen und kombiniert sie.
- Raumplanung-DB Extension mffrps (veraltet)
- Raumplanung-Kalender url raumplanung @sfgz.ch (Aktuell)
- hochgeladener Datei XLSX, CSV... (Zukunft)


## Zeit-Funktionen

### Datenhygiene
Löscht automatisch alle alten Belegungen, das Alter wird in der Extension-Configuration angegeben (Einstellungen / Extension Configuration).

### Permacontent
Wenn eine **Endzeit** angegeben wurde, wird der Text bis zu jenem Datum angezeigt. Er wird an eventuell bestehenenden Text angehängt. Es werden alle Belegung- und Kurseinträge ausgeblendet.

### FIXME 
Permacontent kann nur solange bearbeitet werden bis einen Tag vor Ablauf. Am Ablauf-Tag und später ist eine Bearbeitung nicht möglich
