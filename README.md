# Tic-Tac-Toe
[Tic-Tac-Toe](https://de.wikipedia.org/wiki/Tic-Tac-Toe) oder Drei gewinnt, ist ein einfaches Zweipersonen-Strategiespiel, das du bestimmt schon selber gespielt hast.

## Spielablauf
Das Spielfeld besteht aus neun Felder, die quadratisch (3x3) angeordnet sind.
Die Spieler markieren abwechselnd eines der noch freien Felder mit einem Kreuz (:x:) bzw. Kringel (:o:).

Gewonnen hat, wer drei :x: bzw. :o: in einer Zeile, Spalte oder Diagonale – auch Mühle genannt – gekennzeichnet hat. Sind alle Felder belegt und keiner der Spieler hat gewonnen, so endet das Spiel unentschieden.

### X hat gewonnen
![X hat gewonnen](https://wikimedia.org/api/rest_v1/media/math/render/svg/595038905e2e65568a90ec43d36a9c2a537c1d0a)

### Unentschieden
![Unentschieden](https://wikimedia.org/api/rest_v1/media/math/render/svg/5ba8a4fc55e4259c807ef326b28088e6e46d5e42)

# Deine Aufgaben

## 1.) Vervollständige das Struktorgramm
Ein Nassi-Shneiderman-Diagramm oder auch **Struktogramm** ist ein Diagrammtyp zur Darstellung von Programmentwürfen im Rahmen der Methode der strukturierten Programmierung.  
Ein Struktogramm besteht immer aus den nachfolgenden Strukturblöcken, die ineinander geschachtelt oder miteinander kombiniert werden können:
### Anweisung
![](https://upload.wikimedia.org/wikipedia/commons/1/1e/LineareAnw.png)  
Jede Anweisung (Befehlsfolge), die das Programm abarbeiten soll, wird in einen rechteckigen Strukturblock geschrieben.
### Fallunterscheidung
![](https://upload.wikimedia.org/wikipedia/commons/7/73/ZweifAusw.png)  
Wenn die Bedingung zutreffend (wahr) ist, wird der Anweisungsblock 1 durchlaufen.
Trifft die Bedingung nicht zu (falsch), wird der Anweisungsblock 2 durchlaufen (if then else). Ein Anweisungsblock kann aus einer oder mehreren Anweisungen bestehen.
### Schleife mit Ausgangsbedingung
![](https://upload.wikimedia.org/wikipedia/commons/d/da/FussgesteuerteSchleife.png)  
Der Schleifenkörper (Anweisungsblock 1) wird mindestens einmal durchlaufen, auch wenn die Bedingung von Anfang an nicht zutreffend (falsch) war!  
Die Bedingung, ob Anwendungsblock 1 erneut wiederholt werden soll, wird erst nach dem Durchlauf (dem Ausführen von Anwendungsblock 1) geprüft. Daraus ergibt sich, dass Anwendungsblock 1 mindestens einmal durchlaufen werden muss.

### Struktogramm Tic-Tac-Toe vervollständigen
Wir haben begonnen ein Struktogramm für das Spiel Tic-Tac-Toe zu erstellen.  
An einigen Stellen `(1), (2), (3), (4), (5), (6), (7)` war sich dein zukünftiger Ausbilder Malte nicht sicher. **Kannst Du ihm helfen?**

*Bitte notiere deine Lösungen und füge diese bei Fertigstellung in deine E-Mail an uns ein.*

![tic-tac-toe-struktogramm](./docs/tic-tac-toe-struktogramm.jpg)

## 2.) Programmierung vorbereiten
Nachdem Du jetzt weißt, wie Tic-Tac-Toe funktioniert, wollen wir zusammen programmieren.  
Keine Sorge, wenn Du bislang nur wenig oder gar nicht programmiert hast, wir steigern uns langsam 😉  
Wir wollen deinen Quellcode sehen können und mir dir an deinem Quellcode arbeiten können, daher verwenden wir um den Quellcode kostenfrei auszutauschen, die Plattform GitHub.

### Bitte erledige die folgenden Schritte
- [ ] Du [verfügst bereits über einen GitHub-Account](https://github.com/login) **oder** [du erstellst dir einen kostenfreien GitHub-Account](https://github.com/join).
- [ ] Nachdem Du dich bei Github.com angemeldet hast:
- [ ] Kopiere unseren Quellcode in deinen GitHub-Account. Dazu musst du nur den [folgenden Link klicken](https://github.com/gitpod-io/template-php-laravel-mysql/generate).
  - **Bitte stelle die Sichtbarkeit des neue Repositories - wie voreingestellt - auf `Public`.**
- [ ] Im neu erstellten GitHub-Repository scrollst du runter, bis du diese Anleitung siehst.
- [ ] Du machst nun an dieser Stelle aus deinem soeben erstellten Repository weiter.
- [ ] [Du öffnest Gitpod](https://gitpod.io/)
- [ ] Klicke `Continue with GitHub` und melde dich mit deinen GitHub-Zugangsdaten an.
- [ ] Erstelle durch einen Klick auf `New Workspace` eine neue Programmierumgebung.
- [ ] Wähle im sich öffnenden Dialog die Adresse deines eben erstellten Repository aus.
- Die Arbeitsumgebung GitPod hat sich geöffnet.
- [ ] Öffne dort nun diese Anleitung. Klicke dazu mit einem Rechtsklick auf die Datei `REDAME.md` und dann auf `Open Preview`.
- [ ] Fahre mit der Anleitung in deiner Gitpod-Programmierumgebung fort.

## 3.) Copyright anpassen
Deine Tic-Tac-Toe Webanwendung besteht aus einem Frontend und einem Backend.  
Als Frontend verwenden wir das Tool `Swagger` mit dem man Schnittstellen mit einer grafischen Oberfläche einfach ausprobieren kann.  
Swagger haben wir dir bereits im Browserfenster geöffnet.  
Als Backend verwenden wir eine [PHP-Anwendung](https://www.php.net/manual/en/) auf Basis des Frameworks [Laravel](https://laravel.com/docs/9.x).  

Wir haben eine Funktion vorbereitet, die das Copyright des Spiels ausgibt.

**Bitte probiere die API-Methode zur Anzeige des Copyrights in Swagger aus:**
- [ ] Klicke in Swagger dazu auf `/copyright`.
- [ ] Klicke auf den Button `Try it out`.
- [ ] Sende die Anfrage indem Du auf `Execute` drückst.
- Du siehst im Abschnitt `Response body` die Antwort mit dem aktuellen Copyright.

**Verändere das Copyright:**  
- [ ] Öffne die Datei [app/app/App/Http/Controllers/CopyrightController.php](app/app/App/Http/Controllers/CopyrightController.php) in Gitpod.
- [ ] In Zeile 18 wird das Copyright als String gespeichert.
- [ ] Benutze den verlinkten ASCII Generator um dein Copyright zu erstellen.
- [ ] Ersetze das Copyright `By MÜNSMEDIA GmbH` durch dein eigenes Copyright.
- [ ] Probier Dein neues Copyright mit Swagger aus!
- [ ] Du musst deine Änderung nun noch speichern - **committen** genannt.
  - Klicke dazu in der linken Seitenleiste auf den Reiter `Source Control` oder drücken die Tasten <kbd>Strg</kbd>+<kbd>⇧</kbd>+<kbd>G</kbd> gleichzeitig.
  - Gib oben eine Textnachricht ein, die deine Änderung bestmöglich beschreibt. **Bitte schreibe die Nachricht auf Englisch**.
  - Speichere die Nachricht mit <kbd>⏎</kbd>
  - Klicke den Button `Sync changes` um deine Änderungen auf GitHub hochzuladen
  - 🎉 Du hast deinen ersten Git-Commit soeben gemacht!