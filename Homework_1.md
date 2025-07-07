# 1
*Consider some of the arguments for whether or not it is a good idea to open the source for some kinds of critical software.Examples could include:*

*- Medical devices, such as pacemakers, metering of life signs, controlling drug dosage through intravenous tubes etc.*
*- Electronic voting machines.*
*- Automobile software, include that for vehicle performance (emissions, braking, etc.) and autonomous vehicles.*

*Do you consider it less or more safe and/or secure if the source for these kinds of products is freely available?*

> **==Pro==: 
> Transparenz & Kontrolle -> Vertrauen**
> Offener Quellcode kann von Expertinnen überprüft werden. Schwachstellen wie back doors oder Designfehler werden ggf. schneller erkannt, wenn nicht nur die Entwickelnden den Code prüfen. Kann zu sichereren Systemen führen.
> Speziell bei Wahlcomputern könnte größeres Vertrauen geschaffen werden, wenn im Vorfeld unabhängige Tests bzw. Bug-Bounty-Programme möglich sind.
> **Optimierung, Innovation, Adaption/Interoperabilität**
> Andere können auf bestehendem Code aufbauen, ihn verbessern, an neue Anforderungen anpassen, um Funktionen erweitern.
> **Security through obscurity ist kein verlässlich starker Ansatz**
> Geheimhaltung führt nicht notwendigerweise zu mehr Sicherheit. Unter öffentlicher Beobachtung müssen robustere, gut getestete Schutzmechanismen verwendet werden.
> **==Contra:==
> Open Source-Code erleichtert Zugriff auf Schwachstellen**
> Das erste Pro-Argument ist gleichzeitig das erste gegen Open Source: zugänglicher Code ist einfacher auf Angriffsmöglichkeiten untersuchbar.
> Speziell im medizinischen, aber auch im Automotive-Bereich sind hier gezielte, potenziell lebensbedrohliche Angriffe denkbar. Das gilt allerdings - nach Überwindung erster Hürden - ebenso für proprietären Code.
> **Maintenance & Support**
> Speziell, wenn ein Projekt nicht über ausreichend (auch bezahlte) Entwickelnde verfügt, besteht die Gefahr, dass diese Punkte nicht gewährleistet werden können.
> **Compliance**
> ggf. können regulatorische Standards schlechter eingehalten werden, weil u.U. keine Ressourcen dafür zur Verfügung stehen
> **Widerspruch zu geistigem Eigentum, Geschäftsmodellen**
> Je nach Lizenz können sich für Urheber*innen wie auch Weterentwickelnde Konflikte hinsichtlich der Nutzungs-/Verwertungsrechte ergeben.

# 2
*List some (3+) of the open source projects you probably use day to day. Shortly describe what you use them for.*
> **bbbike.de**
> Fahrradroutenplaner für Berlin, geschrieben in Perl, nutzt Leaflet-API (OSM)
> **Linux Mint**
> Betriebssystem auf meinem Laptop, basiert auf Ubuntu
> **LibreOffice**
> für Text-/Tabellendokumente & Präsentationen
> **Posteo**
> zumindest Server-Software OpenSource, Mail-Provider
> **Moodle**
> für die Uni ;-)

# 3
*Create a profile of an Open Source project of your choice. Include the following information: Project Website URL, Code Repository, when established, License, what is the project good for, Impact on software industry, further interesting facts worth to know. Try to get this information from public sources via a web search.
>**Python**
> [https://python.org](python.org)
> [https://github.com/python/cpython](https://github.com/python/cpython)
> established in 1991, current version 3.15
> 
> [License:](https://github.com/python/cpython/blob/main/LICENSE)
>>Starting with Python 3.8.6, examples, recipes, and other code in the documentation are dual licensed under the PSF License Version 2 and the Zero-Clause BSD license. Some software incorporated into Python is under different licenses. The licenses are listed with code falling under that license. (https://github.com/python/cpython/blob/main/LICENSE)
> Python ist eine freie, quelloffene Programmiersprache.
> Besondere Merkmale:
> - klare, leicht verständliche & zu lernende Syntax
> - wird direkt interpretiert (keine Kompilierung nötig)
> - kann im interaktiven Modus schnell getestet werden
> - unterstützt sowohl
> 	-objektorientierte,
> 	-prozedurale als auch
> 	-funktionales 
> 	Programmieren
> - dynamische Typisierung (a kann während Laufzeit Integer, String etc. sein)
> - umfangreiche Standardbibiotheken
> - zahlreiche Frameworks (Django, NumPy...)
> - plattformunabhängig
> 
> Besonders für Datenanalyse & -wissenschaft, Machine Learning, Automatisierung, Scripting und für den schnellen Einstieg ins selbstständige Programmieren bekannt.