ESP Filament Tracker

Ein leichtgewichtiger, Web-basierter Filament-Manager für ESP32 und ESP8266. Verwalte dein 3D-Druck-Material, behalte den Überblick über Restmengen und drucke QR-Code-Etiketten direkt von deinem Mikrocontroller.
✨ Features

    Dual-Plattform Support: Kompatibel mit ESP32 und ESP8266.

    Web-Interface: Komplett responsive Oberfläche (Dark/Light Mode) für Desktop und Smartphone.

    QR-Code Generator: Erstellt Etiketten für deine Spulen, die direkt zum Bearbeitungsmenü führen.

    Inventar-Management: Speichert bis zu 250 Filamente mit Details wie Hersteller, Material, Farbe, Temperatur-Settings und Gewicht.

    Verbrauchsrechner: Ziehe einfach das Gewicht des verbrauchten Filaments nach einem Druck ab.

    WiFi-Captive-Portal: Einfache Einrichtung der WLAN-Daten über einen Access Point.

    Backup & Restore: Lade deine Datenbank als Binärdatei herunter und stelle sie jederzeit wieder her.

    Mehrsprachig: Unterstützt Deutsch und Englisch.

🛠 Hardware-Anforderungen

    Mikrocontroller: ESP32 oder ESP8266 (z.B. NodeMCU, Wemos D1 Mini).

    Speicher: Nutzt das SPIFFS (Serial Peripheral Interface Flash File System) zur Datenspeicherung.

🚀 Installation

    Stelle sicher, dass du die Arduino IDE oder PlatformIO installiert hast.

    Installiere die benötigten Boards (ESP32 oder ESP8266) über den Board-Verwalter.

    Kopiere den Code aus der .ino Datei in ein neues Sketch.

    Wähle dein Board aus und klicke auf Upload.

    Wichtig: Der ESP nutzt SPIFFS. Beim ersten Start wird das Dateisystem automatisch formatiert.

Erstmalige Einrichtung (WiFi)

    Nach dem Flashen öffnet der ESP einen Access Point namens Filament-Tracker-Setup.

    Verbinde dich mit deinem Smartphone/PC mit diesem Netzwerk.

    Die Setup-Seite sollte automatisch erscheinen (Captive Portal). Wähle dein WLAN aus und gib das Passwort ein.

    Der ESP startet neu und ist nun unter seiner IP-Adresse in deinem Netzwerk erreichbar.

📂 Dateistruktur & Datenspeicherung

Der Tracker speichert zwei Dateien im internen Flash-Speicher:

    /wifi.txt: Enthält deine WLAN-Zugangsdaten.

    /data.bin: Eine Binärdatei, die das gesamte Filament-Inventar (struct Filament) enthält.

🖥 Screenshots / UI

    Dashboard: Übersicht aller Spulen mit Fortschrittsbalken (Restmenge).

    Edit-Modus: Anpassen von Temperaturen und Gewichten.

    QR-Label: Druckfertige Ansicht für dein Filament-Regal.

📝 Lizenz

Dieses Projekt ist unter der MIT-Lizenz veröffentlicht. Du kannst es gerne für private Zwecke nutzen und modifizieren.
