# Dome DJ-Kontrollbogen – Prototyp

Vier Kontrollbögen entsprechend „DJ Kontrollbögen Dome 2027.docx“.

## Testen

Im Verzeichnis `dome-pruefapp` einen lokalen Webserver starten, z. B. `python -m http.server 8000`, dann im Browser `http://localhost:8000` öffnen. Für Smartphone-Installation die Dateien auf einen HTTPS-fähigen statischen Webhost hochladen. Der erste Aufruf braucht Internet; nach dem Laden der PWA-Ressourcen funktioniert die Kontrolle offline. Das Mailprogramm braucht zum Versenden wieder Internet.

## Funktionen

- Main Stage, Main FOH, Stadl, La Vie
- Eindeutiger Bogen je Veranstaltungsdatum und Bereich **pro Gerät**
- Lokale Speicherung in IndexedDB, automatische Zwischenspeicherung
- Archiv auch für fehlerfreie Prüfungen
- Digitale Bestätigung per Namen und Kontrollkästchen
- E-Mail-Entwurf nur bei technischem Defekt oder Soundcheck-Schaden; Versand manuell über Mailprogramm
- JSON-Export/Import zur Datensicherung

## Grenzen

- Kein zentraler Abgleich zwischen Geräten; kein geräteübergreifender Duplikatschutz.
- Keine verlässliche Versandbestätigung; „E-Mail vorbereiten“ bedeutet nicht „gesendet“.
- Keine fälschungssichere Signatur oder revisionssichere Speicherung.
- Für tatsächlichen Betrieb: Prüfen, ob Name und Bestätigung als Abnahme ausreichen, sowie Datenschutz und betriebliche Vorgaben klären.
- Die App zeigt die in der Vorlage erwähnten Abläufe an, übernimmt aber keine arbeitsrechtlich relevanten Sanktionsformulierungen.
