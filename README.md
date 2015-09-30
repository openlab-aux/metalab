# openlab

Meta-Projektrepository für das Openlab

```
bash checkout <folder1> <folder2> …
```

## What

Dieses Repository soll es möglich machen, einen schnellen und guten Überblick über alle Projektrepositories des Obenlab zu bekommen.

Im Moment kann man mit obigem Kommando auf einen Schlag alle Software in den angegebenen Ordnern (oder alle Repos ohne Ordner) auschecken.

## How

In (fast) jedem Ordner gibt es eine `.repos`-Datei. Diese enthält Links zu den Repos. Das `checkout` Script automatisiert das Klonen.

Funktionieren sollte es auf jedem System mit bash, POSIX und git, also eventuell auch unter Windows. Es wird aber keine vollständige Kompatibilität angestrebt.

Projektsammelordner haben ein `+` als Prefix. Das dient dazu, sie von ausgecheckten Repos zu unterscheiden.

## Todo

- Eine Möglichkeit, Repositories wieder zu entfernen. Das sollte genauso wie das Hinzufügen funkionieren und Repositories mit (ungepushten) Änderungen überspringen, außer `--force` ist gegeben
- Einfügen von Beschreibungen der einzelnen Repos (kann in den `.repos`-Dateien hinter dem Link passieren, ab dem ersten Space kommt die Beschreibung).
- Dokumentation der einzelnen Projekte, mit Kommandozeilentool anzeigbar (Beschreibung, Readme, Wikilinks, …)
- Bash ist nicht die sicherste Sprache; eventuell kann man die Skripte in eine schönere Sprache umwandeln und Binaries einchecken.