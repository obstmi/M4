# Fallstricke, Verirrungen, Learnings und Best practices während unseres 1. Projektes

## Git

### Einrichten eines Tracking Branches "dev"
Dies ist notwendig, wenn remote bereits der dev-Branch existiert, mit dem auch lokal gearbeitet werden soll:
1. Überprüfen, ob Remote verbunden ist:
    git remote -v
2. Remote branches holen:
    git fetch origin
3. Dev-Branch lokal erstellen und mit Remote verbinden:
    git branch dev origin/dev 
    *oder*
    git checkout -b dev origin/dev
4. Nicht vergessen: in den dev-Branch wechseln (falls nicht schon implizit geschehen):
    git checkout dev
Siehe auch: https://stackify.com/git-checkout-remote-branch/

### Pushen von Verzeichnissen
Verzeichnisse können erst gepuscht werden, wenn sie nicht leer sind. Ansonsten bleiben sie im lokalen Repository.

### Adden von Dateien
* git add . --> wirkt nur auf das aktuelle Verzeichnis (und Unterordner?)

## GitHub

### Verwendung von ssh
* für "git remote add origin <GitHib-Verzeichnis>" __nicht__ den https-Link verwenden, sondern dieses Format: "git@github.com:username/repo.git"
Für die nachträgeliche Korrektur siehe:
https://help.github.com/en/github/using-git/changing-a-remotes-url#switching-remote-urls-from-https-to-ssh 

## MD
Markdown ist eine vereinfachte Auszeichnungssprache. Ein Ziel von Markdown ist, dass schon die Ausgangsform ohne weitere Konvertierung leicht lesbar ist.
* Cheatsheet: https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf