# Stationslager-Erweiterung - by Tim-O
Station Storage Extension (SSE)

![Stationslager-Erweiterung](http://img3.imagebanana.com/img/cxjczx2c/sse.superfreighters.jpg)

Die Stationslager-Erweiterung erm�glicht es, den Frachtraum angedockter Schiffe als Erweiterung des Stationslagers zu benutzen. Schiffe, die an die Station angedockt sind und sie als Heimatbasis eingestellt haben, k�nnen in eine Lagererweiterung verwandelt werden. Sie werden dann dazu benutzt, �berproduktionen einzulagern und die Lager wieder aufzuf�llen, wenn eine Ware einmal nicht in ausreichender Zahl verf�gbar ist.

Die Stationslager-Erweiterung befindet sich unter den Stationskommandos. Man erkennt sie an ihrer gelben Farbe.

Korrespondierender Thread im Egosoft-Forum: [[SCR][13.03.2009] Stationslager-Erweiterung v beta.02](http://forum.egosoft.com/viewtopic.php?t=239411)

## Mindestvoraussetzungen:
* Eine Station und ein angedocktes Schiff mit der Station als Heimatbasis.

## Installation:
* Den Inhalt des Ordners `t` in den `X3 TC\t` Ordner kopieren
* Den Inhalt des Ordners `scripts` in den `X3 TC\scripts` Ordner kopieren

## Update:
* Den Inhalt des Ordners `t` in den `X3 TC\t` Ordner kopieren
* Den Inhalt des Ordners `scripts` in den `X3 TC\scripts` Ordner kopieren
* Im Spiel wird es nur eine Meldung geben, wenn das Skript gerade auf einer Station l�uft und daher neu gestartet werden musste. Die aktuelle Version ist aber im Konfigurationspanel in der oberen rechten Ecke sichtbar. Hier k�nnt ihr also nachsehen, ob das Update geklappt hat.

## Deinstallation:
* Im Spiel ein Kontrollpanel der Stationslager-Erweiterung �ffnen. (unter Stationskommandos)
* Den untersten Men�punkt "Deinstallieren" w�hlen und die sicherheitsabfrage mit "Ja" best�tigen.
* Warten, bis die Deinstallation als erfolgreich gemeldet wurde.
* Speichern.
* X3 verlassen.
* Alle zum Skript geh�rigen Dateien aus den Ordnern `X3 TC\scripts` und `X3 TC\t` l�schen (Siehe "Verwendete Ressourcen").
* Fertig.

## Beschreibung:
Schon immer genervt, dass eine Station oder ein Komplex nur so wenig von ihren Produkten lagern kann? Jetzt ist es damit vorbei! Die Stationslager-Erweiterung erm�glicht den automatischen Transfer von Waren auf und von angedockten Schiffen, die explizit bei der Lagererweiterung registriert wurden. Die Einstellungen erlauben das setzen einer oberen und unteren Grenze, zwischen denen die Lagererweiterung den Lagerstand zu halten versucht. �berproduktionen werden in den Frachtraum der Erweiterungsschiffe ausgelagert und M�ngel aus den ausgelagerten Waren ausgeglichen. F�r jede von der Erweiterung verwaltete Ware kann man au�erdem bevorzugte Schiffe w�hlen. Diese werden dann bei der Lagerung dieser Ware zuerst beladen und zuletzt wieder geleert.
Um ein Schiff f�r die Lagererweiterung zu verwenden, muss es an der Station angedockt sein und sie als Heimatbasis eingetragen haben. Man kann das Schiff nun unter der Rubrik "Erweiterungsschiffe verwalten" im Kontrollpanel der Lagererweiterung zur Liste der Erweiterungsschiffe hinzuf�gen. Das Schiff bleibt so lange bei der Erweiterung registriert, bis es aus der Liste entfernt, zerst�rt, oder einer anderen Heimatbasis zugeordnet wird.
Wenn man eine Fabrik/einen Komplex hat, der starke �berproduktion abwirft, kann die Lagererweiterung einem die Arbeit sparen, die es macht, wenn man st�ndig von Hand die Lager auf andere Schiffe ausleeren, oder eine komplexe Warentransportkette zu Lagerstationen aufbauen muss. Wenn die Lager der Erweiterungsschiffe doch einmal zu voll werden, kann die Lagererweiterung eine Warnung abgeben. Diese wird ausgel�st, wenn der genutzte Frachtraum der angedockten Erweiterungsschiffe eine einstellbare Grenze �berschreitet. Es sind sowohl Warnungen f�r den gesamten genutzten Frachtraum, als auch f�r den genutzten Frachtraum der bevorzugten Schiffe einer Ware m�glich. Wenn man bestimmte Waren wirklich nur auf den daf�r bestimmten Schiffen haben will, wird man so gewarnt, dass diese �berzulaufen drohen.

## Benutzung:
Die Benutzung der Stationslager-Erweiterung sollte sehr intuitiv sein. Das Benutzerinterface wurde so selbsterkl�rend wie m�glich entworfen. Viele Fenster haben oben eine kurze Beschreibung der Einstellungsm�glichkeiten, so dass man durch Anschauen und Ausprobieren eigentlich die Handhabung sehr schnell heraus haben sollte. Wenn es trotzdem Probleme geben sollte, scheut euch nicht, im Forum im Thread des Skripts zu fragen.

## Verwendete Ressourcen:

### Kommandoslot:
`COMMAND_TYPE_STATION_35 (1135)`

### Sprachdateien: 
`t\8223-L044.xml (page 8223)`
`t\8223-L049.xml (page 8223)`

`t\8910-L044.xml (page 8910)` <-------String Library von ChemODur!! http://forum.egosoft.com/viewtopic.php?t=233377
`t\8910-L049.xml (page 8910)` <-------String Library von ChemODur!! http://forum.egosoft.com/viewtopic.php?t=233377

### Skriptdateien:
`scripts\lib.chem.strings.xml` <-------String Library von ChemODur!! http://forum.egosoft.com/viewtopic.php?t=233377

`scripts\plugin.sse.consistency.check.xml`
`scripts\plugin.sse.core.xml`
`scripts\plugin.sse.find.ship.for.loading.xml`
`scripts\plugin.sse.find.ship.for.unload.xml`
`scripts\plugin.sse.get.ware.settings.xml`
`scripts\plugin.sse.pref.usage.docked.xml`
`scripts\plugin.sse.restart.core.xml`
`scripts\plugin.sse.total.usage.docked.xml`
`scripts\plugin.sse.ui.main.xml`
`scripts\plugin.sse.ui.manage.ships.xml`
`scripts\plugin.sse.ui.manage.wares.xml`
`scripts\plugin.sse.ui.notifications.xml`
`scripts\plugin.sse.ui.ware.select.ship.xml`
`scripts\plugin.sse.ui.ware.settings.xml`
`scripts\setup.plugin.sse.xml`
`scripts\uninstall.plugin.sse.xml`

## Changelog:

###13.03.2009: v beta.02

- Problem behoben, das einen Freeze ausl�sen konnte, wenn ein Schiff eine ware ausladen sollte, die es installiert hatte.
- Problem behoben, durch das "Ausladen und beenden" nicht korrekt beendete, wenn ein Schiff eine Ware installiert hatte, die es ausladen sollte.

###12.03.2009: v beta.01

- Erstausgabe
