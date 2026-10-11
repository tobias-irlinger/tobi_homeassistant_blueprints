# Home Assistant Blueprints

Automations-Blueprints für Home Assistant. Import per Klick auf den Button oder über
*Einstellungen → Automationen & Szenen → Blueprints → Blueprint importieren* mit der jeweiligen URL.

## Sensor-Wächter (veraltete Werte)

Version 1.1.1 · benötigt Home Assistant 2024.10 oder neuer

Meldet Geräte, deren Sensoren seit einer einstellbaren Zeit nichts mehr gesendet haben – auch wenn der angezeigte Wert noch plausibel aussieht (Prüfung über `last_reported`).

[![Blueprint importieren](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Ftobias-irlinger%2Ftobi_homeassistant_blueprints%2Fblob%2Fmain%2Fblueprints%2Fautomation%2Fsensor_watchdog.yaml)

Quelle: [`blueprints/automation/sensor_watchdog.yaml`](blueprints/automation/sensor_watchdog.yaml)

## Gang Lichtsteuerung

Version 1.4.1 · benötigt Home Assistant 2024.8 oder neuer

Ganglicht über Bewegungsmelder mit Lux-Schwelle, getrennten Zeitfenstern für Arbeitstage und Wochenende/Feiertage (Workday) und manuellem Schalter mit Wiedereinschaltverzögerung.

[![Blueprint importieren](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Ftobias-irlinger%2Ftobi_homeassistant_blueprints%2Fblob%2Fmain%2Fblueprints%2Fautomation%2Fgang_licht_steuerung.yaml)

Quelle: [`blueprints/automation/gang_licht_steuerung.yaml`](blueprints/automation/gang_licht_steuerung.yaml)

## Pufferspeicher-Pumpensteuerung mit Ventilschutz

Version 12.2 · benötigt Home Assistant 2024.6 oder neuer

Schaltet die Umwälzpumpe nach Heizbedarf der Thermostate, optional abhängig von der Puffertemperatur; mit Hysterese, Wiedereinschaltverzögerung und wöchentlichem Ventilschutz.

[![Blueprint importieren](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Ftobias-irlinger%2Ftobi_homeassistant_blueprints%2Fblob%2Fmain%2Fblueprints%2Fautomation%2Fpumpensteuerung.yaml)

Quelle: [`blueprints/automation/pumpensteuerung.yaml`](blueprints/automation/pumpensteuerung.yaml)

## PID-Mischkreisregelung für Kachelofen-Pufferspeicher

Version 5.2 · benötigt Home Assistant 2024.6 oder neuer

Regelt die Vorlauftemperatur über einen Mischer-Stellmotor (AUF/ZU) per PID, mit Heizkurve, Smart Start, Sicherheitsgrenzen und Fühlerüberwachung. Arbeitet mit der Pumpensteuerung zusammen.

[![Blueprint importieren](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Ftobias-irlinger%2Ftobi_homeassistant_blueprints%2Fblob%2Fmain%2Fblueprints%2Fautomation%2Fpid_mischkreis.yaml)

Quelle: [`blueprints/automation/pid_mischkreis.yaml`](blueprints/automation/pid_mischkreis.yaml)

## Hinweis

Die Heizungs-Blueprints (Pumpensteuerung, PID-Mischkreis) schalten echte Hardware. Nach dem Einrichten
den Status-Helfer und die Automations-Traces beobachten, bevor die Regelung unbeaufsichtigt läuft. Nutzung auf eigene Verantwortung.

## Lizenz

[MIT](LICENSE)
