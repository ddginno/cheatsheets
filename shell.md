# Shell Commands

## **Navigation**

Sie haben fünf Befehle gelernt, die häufig zum Navigieren im Dateisystem über die Befehlszeile verwendet werden. Was können wir bisher verallgemeinern?

* Die Befehlszeile ist eine Textschnittstelle für das Betriebssystem des Computers. Um auf die Befehlszeile zuzugreifen, verwenden wir das Terminal.

* Ein Dateisystem organisiert die Dateien und Verzeichnisse eines Computers in einer Baumstruktur. Es beginnt mit dem Stammverzeichnis. Jedes übergeordnete Verzeichnis kann mehrere untergeordnete Verzeichnisse und Dateien enthalten.

* Über die Befehlszeile können Sie durch Dateien und Ordner auf Ihrem Computer navigieren:

* **pwd** gibt den Namen des aktuellen Arbeitsverzeichnisses aus.
* **ls** listet alle Dateien und Verzeichnisse im Arbeitsverzeichnis auf.
* **cd** wechselt in das von Ihnen angegebene Verzeichnis.
* **mkdir** legt ein neues Verzeichnis im Arbeitsverzeichnis an.
touch erstellt eine neue Datei im Arbeitsverzeichnis.


***

## **Manipulation**

Optionen ändern das Verhalten von Befehlen:
* ls -a listet alle Inhalte eines Verzeichnisses auf, einschließlich versteckter Dateien und Verzeichnisse
* ls -l listet alle Inhalte im Langformat auf
* ls -t ordnet Dateien und Verzeichnisse zum Zeitpunkt der letzten Änderung an
Mehrere Optionen können zusammen verwendet werden, z. B. ls -alt

Über die Befehlszeile können Sie auch Dateien und Verzeichnisse kopieren, verschieben und entfernen:

* cp kopiert Dateien
mv verschiebt und benennt Dateien um
* rm entfernt Dateien
* rm -r entfernt Verzeichnisse
Platzhalter sind nützlich, um Gruppen von Dateien und Verzeichnissen auszuwählen

## **[Shell Abk. Worterklärung](https://explainshell.com/)**

*** 

# Cheat Sheet für **Shell Befehle**

#### Wechseln zu anderen Ordnern / Inhalt anzeigen etc.:

- `cd [Ordnername]` change directory
- `..` Weiterleitung in übergeordnete Ordner
- `z neu` = `cd ~/neuefische` z lernt oft benutzte Ordner und bietet so Abkürzung
- `ls` Liste aller Dateien und Unterordner eines Ordners
- `ls -la` Liste mit Details `l` (=long; untereinander auflisten) und durch `a` (=all) werden auch versteckte Dateien angezeigt
- `tree` Verzeichnisbaum anzeigen
- `curl` lädt Objekt über eine URL
- `cat` zeigt den Inhalt einer Datei

#### Neu, verschieben, kopieren, löschen, öffnen:

- `mkdir` Ordner erstellen
- `mkdir [Ordner/Unterordner]` Unterordner erstellen
- `mkdir -p [Ordner/Unterordner/Unterunterordner/...]` Ordnerpfad wird erzeugt
- `touch [Dateiname]` Datei erstellen
- `mv [alter Name] [neuer Name]` Ordner/Datei umbenennen
- `mv [alter Pfad] [neuer Pfad]` Ordner/Datei verschieben
- `mv [Ordner] *` verschieben des Ordners in den aktuellen Ordner
- `cp -R [src-directory] [target-directory]` kopiert alles aus dem Quellverzeichnis in das Zielverzeichnis
- `pbcopy` speichert Eingabe in die Zwischenablage (Bsp.: `cat ~/.ssh/id_rsa.pub | pbcopy`)
- `rm` remove (geht nur bei Dateien)
- `rm -rf` Ordner löschen; `r` = rekursiv (alles in allen Unterordnern); `f` = force (nicht jede Datei einzeln bestätigen); uch **Rimraf** genannt
- `rm -rf *` löschen aller Ordner und Dateien im aktuellen Ordner
- `code .` aktueller Ordner wird bei VS Code aufgerufen
- `open [Datei]` öffnet Datei mit dem Standardprogramm eines Betriebssystems
- `open .` öffnet Ordner im Finder/Explorer