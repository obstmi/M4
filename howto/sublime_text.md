# Tipps für Sublime Text 3

## Installation eines Pakets zum Formatieren von HTML/CSS/JS

Im Terminal ausführen:

```
sudo apt install curl
curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
sudo apt install nodejs
```

Im Sublime Text:

```
Tools/Install Package Control...
Preferences/Package Control
```

Dann im den Fenster, das sich geöffnet hat, tippen:

```
Install Package <Enter>
HTML-CSS-JS Prettify <Enter>
```

Dann wieder im Menü:

```
Preferences/Package Settings/HTML-CSS-JS Prettify/Prettify Preferences - Default
```

In der Datei ändern: 

```
        // Indentation size
        "indent_size": 4,
```

auf

```
        // Indentation size
        "indent_size": 2,
```

und speichern und schließen.

Anschließen kann man mit `<Ctrl><Shift>H` den Code formatieren.

Das ist folgendes Plugin: [HTML-CSS-JS Prettify](https://packagecontrol.io/packages/HTML-CSS-JS%20Prettify)


## Einstellungen zur Einrückung des Codes

Die folgenden Einstellungen im Menü sorgen dafür, dass Sublime Text den Code mit 2 Leerzeichen einrückt:

```
View/Indentation/Indent Using Spaces
View/Indentation/Tab Width: 2
```

Anschliendend bei den Dateien, die noch eine andere Einrückung haben:

```
View/Indentation/Convert Indentation to Spaces
```