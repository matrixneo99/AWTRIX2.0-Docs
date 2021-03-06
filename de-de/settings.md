Über die Sidebar "Settings" können verschiedene Einstellungen für den Host und Matrix getätigt werden. Im Folgenden werden alle Möglichkeiten erklärt:

## Host

### Basic Settings

**Boot Animation**  
Zeigt beim ersten Verbindungsaufbau der Matrix eine Bootanimation an.
Diese nutzt die Draw API. Die bootanimation.json befindet sich im Ordner "config" und kann beliebig verändert werden.

**Switch Animation**  
Die aktiviert eine Wechselanimation zwischen den Apps. Hierbei wird die alte App heruntergedimmt und die neue hochgedimmt.

**Color Switch**  
Eine andere Form der Wechselanimation. Hier löscht ein farbiger Balken die aktive App von der Matrix.

**Uppercase Letters**  
Diese Funktion wandlelt alle Texte in Großbuchstaben um.

**Remove Accents**  
Einige Sprachen verwenden Akzente die die Matrix nicht darstellen kann. Diese Funktion ersetzt diese mit lesbaren Zeichen.

**Verbose Log**  
Diese Funktion erweitert den Log. Dies ist vorallem Hilfreich bei Bugreports.

**Analytics**  
Diese Funktion erlaubt die Übergabe der IP-Adresse an den AWTRIX Cloud Server. Es werden keine weiteren Einstellungen oder Informationen gesendet.
Anhand dieser IP Adresse kann ich einsehen in welchem Land AWTRIX läuft und wieviele insgesamt. Diese Information wird nicht an dritte weitergegeben und nicht gespeichert.
Die Information wird temporär zur Laufzeit meines Servers gehalten, und wird komplett gelöscht sobald ein AWTRIX Host länger als 10min offline ist.  
P.S. Jeder normale Webseiten Aufruf, Email-Versand und auch die Downloads der Icons hinterlässt am jeweiligen Server immer die IP-Adresse. Bei AWTRIX könnt ihr aber bestimmen ob ich diese zur Auswertung nutzen darf. Dies hilft mir zu sehen wie verbreitet mein Projekt bisher ist, dadurch kann ich AWTRIX auf bestimmte Länder anpassen und es motiviert mich natürlich massiv euch immer mehr Funktionen zu bieten.

**Textcolor**  
Hier kannst du die globale Textfarbe bestimmen.
Trage entweder deine gewünschte Farbe im Format rgb(R,G,B) ein oder nutze den Colorpicker auf der rechten Seite

**Brightness**  
Hier wird die Helligkeit der Matrix festgelegt (0-100%). Bitte bedenke: Je heller die Matrix, desto mehr Strom wird verbraucht und desto wärmer wird sie.

!> Die Matrix kann bei höchster Helligkeitsstufe und komplett weißen Pixeln bis zu 75 Watt beanspruchen! Um eine übermäßige Hitzeentwicklung zu vermeiden, empfiehlt sich eine **maximale** Helligkeit von 75%.

**App Duration**  
Legt die Zeit fest, wie lange eine App angezeigt wird, bevor zur Nächsten gewechselt wird.

**Scroll speed**  
Mit diesem Wert wird angebegen nach wievielen Millisekunden der Text um eine Y-Position verschoben wird. Ein niedriger Wert lässt den Text schneller scrollen, sorgt allerdings auch für eine höhere CPU Auslastung.

**Update interval**  
Dieser wert gibt an, nach wievielen Sekunden alle Apps ihre Daten aktualisieren.

**Volume**  
Stellt die Lautstärke des angeschlossenen DFPlayer ein.

**Timezone Offset (UTC)**  
Dies stellt die Differenz zur UTC Zeitzone ein.

### Communication

#### Webserver

**Port**  
ändert den Port über den das AWTRIX Webinterface aufgerufen wird

**Enable Login**  
Aktiviert die Anmeldemaske des AWTRIX Webinterfaces

**Login Password**  
Das Passwort für die Anmeldemaske (Standard: **awtrix**)

#### MQTT

Aktiviert den MQTT Client. Weitere Einstellungen sind selbsterklärend.

### Matrix connection

Du kannst die Matrix entweder über WiFi oder USB betreiben. Wenn du ein schwaches oder überlastetes WiFi hast, versuche bitte die Kommunikation der Matrix über USB an, um Ruckeln zu vermeiden.

!> Die Auswahl von ttyAMA0 kann beim RaspberryPi 3 und höher zum Abstutz führen da dieser Port vom Bluetooth belegt ist. Nutze stattdessen ttyS0!

### Premium

[Siehe hier](de-de/premium.md)

## Matrix

### LED Settings

**Color Correction**  
Es kann vorkommen das die Matrizen einen leichten Farbstich bei weißen Licht aufweisen. Dies ist auf Qualitätsunterschiede und die Kalibrierung der LEDs zurückzuführen.
Mit der Farbkorrektur kannst Sie die Farben der LEDs so einstellen, dass ein klares Weiß entsteht. **OvercastSky** funktioniert bei einem Rotstich am besten und ergibt ein strahlendes Weiß

**Auto Brightness**  
Wenn du einen LDR (Light Dependent Resistor) an die Matrix angeschlossen hast, kannst du hier die automatische Helligkeitsregelung einstellen. Wenn du die empfohlenen Komponenten verbaut hast, musst du an den Werten nichts ändern.

- **Resistor**
  Gibt den verwendeten Vorwiderstand an (1000ohm ist hier standard)
- **Minimum Lux**
  Der minimale Helligkeitswert der vom LDR gemessen werden kann
- **Maximum Lux**
  Der maximale Helligkeitswert der vom LDR gemessen werden kann
- **Minimum Brightness**
  Die minimale Helligkeit die nach der Berechnung möglich ist (0-100%)
- **Maximum Brightness**
  Die maximale Helligkeit die nach der Berechnung möglich ist (0-100%)
