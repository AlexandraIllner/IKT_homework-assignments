![[diff_log.png]]![[log_status.png]]![[branch_merge.png]]![[meld.png]]![[exp_merge0.png]]

![[exp_merge1.png]]

![[exp_merge2.png]]Probleme:
Ich habe lange nicht verstanden, dass es nur um git commit, ohne Angabe einer Datei geht.

Fragen:
### 1
*einfacher/fast forward merge*
- aktueller Branch ist direkter Vorfahre, keine parallele Entwicklung (an denselben Dateien)
- der aktuelle Branch endet mit dem neu hineingemergten commit
*3-way merge*
- Git sucht gemeinsamen Vorfahren (letzter gemeinsamer Stand -> Base)
- Vergleich von
	1. Base
	2. HEAD = aktueller Branch, akt. Stand
	3. Source = Branch, der gemerged werden soll, akt. Stand
- beim merge werden die Entwicklungen zusammengeführt:
> 	(main) A---B---C---F
> 	               \	
> 	(feature)     D---E
- der merge erzeugt einen neuen commit (hier G)
- dieser hat zwei Vorfahren
### 2
In einem Versionskontrollsystem werden jedewede Änderungen an Dateien erfasst, dokumentiert und verwaltet. So kann jederzeit nachvollzogen werden, wann was von wem geändert wurde (Zeitstempel, Benutzerkennung).
Änderungen können rückgängig bzw. ein früherer Zustand wiederhergestellt werden.
Das ermöglicht die gemeinsame Arbeit an Projekten.
Probleme/Konflikte werden durchs System erkannt.
Jede Version des Projekts wird gespeichert.

### 3
Getrackte, geänderte Dateien werden beim commit als snapshot gespeichert. Alle unveränderten Dateien werden mittels hashes -> Verweisen auf existierende Objekte repräsentiert.
Jeder commit erhält eine eindeutige SHA1-ID.
SHA-Hashes ergeben sich aus dem Secure Hash Algorithm 1, einer kryptographischen Funktion, die aus Eingaben beliebiger Länge 160 Bit lange Werte berechnet (Darstellung als Hexadezimalzahl, 40 Stellen).
Eine identische Eingabe führt jedes Mal zum selben Hash-Wert.
Da auch die unveränderten Dateien lediglich durch Hash-Verweise auf ihre Vorfahren gespeichert werden, ist Git extrem effizient. diffs können zwar aufgerufen werden, werden aber nicht gespeichert.

### 4
Branching ermöglicht die Arbeit an unterschiedlichen Funktionen, ggf. durch verschiedene Entwickelnde, zur gleichen Zeit.
Indem von einem Zustand aus ein Branch erstellt wird, wird das Gesamtprojekt zunächst nicht verändert.
Beispiel:
Bei der Entwicklung einer Website kümmert sich Alice um die Login-Fkt., Bülent ums CMS und 3 weitere um die Datenbank-API. Bereits bestehende Komponenten bleiben unberührt, bis ein Branch ins Hauptprojekt gemerged wird. Ob dann noch alles funktioniert, kann auf einem Test-Branch ausprobiert werden.
Andere Use Cases:
Es sollen verschiedene Designs getestet werden.
Es gibt Ideen für neue Funktionen und unterschiedliche Ansätze zur Umsetzung.
