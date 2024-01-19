# Das Internet vergisst doch - Handreichung für die Archivierung von wissenschaftlichen Webseiten
Autoren: Andreas Frech (LMU) und Yves Vincent Grossmann (MPDL)

Version 1.0 - 18.01.2024

## Einleitendes
### Problembeschreibung
Entgegen des häufig kolportierten Satzes „Das Internet vergisst nichts!“ und des ebenso häufig angemahnten „Rechts auf Vergessen“ verschwinden Informationen oft leise und unbemerkt, aber stetig aus dem Netz. Diese Phänomene werden als „content drift“ (Änderung von Webinhalten unter der gleichen Adresse), „link rot“ (Verfall von Webseitenlinks) oder „reference rot“ (Verfall von Zitierungen eines Webinhalts) bezeichnet. Sie betreffen das gesamte Spektrum des Internets, von einzelnen Webseiten, über Publikationen bis hin zu Social-Media-Anbietern. Zwar ist es richtig, dass besonders Social-Media-Posts über einen mittelfristig relevanten Zeitraum erhalten bleiben, jedoch ist eine langfristige Verfügbarkeit selbst bei großen Marktteilnehmern alles andere als gewährleistet. Im März 2019 wurde bekannt, dass die Social-Media-Plattform [„MySpace“](https://de.wikipedia.org/wiki/Myspace#Geschichte ) durch einen missglückten Serverumzug ca. 50 Millionen Fotos, Videos und Audiodateien verlor, die in den Jahren 2003 bis 2016 hochgeladen wurden. 490.000 mp3s konnten im April 2019 durch das Internet Archive wiederhergestellt werden; die Mehrheit der Daten blieb jedoch verloren. In den 2000er Jahren war MySpace die zentrale Anlaufstelle für Musiker und Musikliebhaber gleichermaßen im Internet und das Verschwinden von sowohl Daten als auch der Plattform selbst war lange so undenkbar wie bei anderen großen zeitgenössischen, inzwischen heftig ins Wanken geratenen Plattformen. Jede einzelne Webseite im Internet benötigt Hardware-Komponenten wie Webserver, Speichermedien und Netzwerkinfrastruktur und dazu passende Betriebssysteme, Datenbank- und Webserver-Software. Zur Darstellung der Inhalte werden zusätzlich Programmiersprachen, Skripte und Stylesheets verwendet. Jeder einzelne dieser Komponenten unterliegt einem technologischen Alterungsprozess und bedarf aufwendiger Pflege und Wartung. Viele dieser Softwarekomponenten werden nutzerfreundlich in Content-Management-Systemen wie z.B. WordPress zusammengefasst, die selbst wiederum diesen Alterungsprozessen unterliegen und gewartet werden müssen. Es entsteht das Paradox von einer (scheinbaren) Überfülle auf der einen und Knappheit, d.h. dem schnellen Quellenverlust, auf der anderen Seite (Roy Rosenzweig[^9]). Bei der Erstellung einer neuen Webseite ist es also wichtig, von Anfang an die Bedeutung der Datenarchivierung im Blick zu haben. Dies ermöglicht die langfristige Bewahrung der auf der Seite veröffentlichten Informationen. 
### Ziel des Dokuments
Webdesigner bauen eine Webseite gewöhnlich unter den Gesichtspunkten Nutzerfreundlichkeit, Performance und Suchmaschinenoptimierung. Zunehmend wichtiger wird es jedoch auch, für langfristige Zugänglichkeit und möglichst vollständige Langzeitarchivierung zu gestalten, was sich auf Struktur, Inhalt, Funktionalität und Front-End-Präsentation auswirkt. Wie also sollte eine Webseite aufgebaut sein, die möglichst langfristig – also mit einem Zeithorizont jenseits von 10 Jahren, wie es die [Standards zur Sicherung guter wissenschaftlicher Praxis](https://wissenschaftliche-integritaet.de/kodex/archivierung/ ) der DFG empfehlen  – relevante Informationen bereitstellen soll, sei es online oder in einem Webarchiv? Und was sollte vor der Web-Publikation dabei berücksichtigt werden?
### Zielgruppen
> **Projektverantwortliche**
> Die Handreichung soll vor allem bei der Konzeption von Projekten unterstützen, damit die Projektinhalte möglichst langfristig online verfügbar gehalten werden können.
>> Wichtige Kapitel "Erste Schritte", "Informationsmodelle", "Dateiformate und Datenbanken", "Graphische Darstellungen", "Maschinen-Lesbarkeit", "Webseiten-Archivierung in den Leitlinien zur guten wissenschaftlichen Praxis", "Rechtliche Fragestellungen", "Datenschutz", "Checkliste für die Webseitenarchivierung"

> **Technische Mitarbeiter, Webdesigner**
> Die Handreichung soll Entwickler und Webdesigner Hinweise geben, welche technischen Parameter und Designentscheidungen Einfluss auf die Langzeitverfügbarkeit und Archivierbarkeit einer Webseite haben.
>> Wichtige Kapitel "Technisches", "Dateiformate und Datenbanken" "Graphische Darstellungen", "Maschinen-Lesbarkeit"

> **Institutionen**
> Die Handreichung kann zur Erarbeitung interner Standards und Vorgaben dienen, um eigene Webseiten langfristig verfügbar zu halten. Auch kann sie bei der Kommunikation mit Archivierungsinfrastruktureinrichungen hilfreich sein. Dies gilt gleichermaßen bei der Vergabe von Aufträgen, wo sie zur Ableitung von Anforderungen herangezogen werden kann.
### Erste Schritte und wesentliche Fragen
Hier sind einige Punkte, die Sie berücksichtigen sollten:
* Definieren Sie klare Ziele für Ihre Webseite und bedenken Sie was wie vermittelt werden soll. Welche Informationen müssen, sollen oder können erhalten werden?
* Je einfacher der Aufbau der Webseite, desto leichter und sicherer kann die langfristige Verfügbarkeit sichergestellt werden.
* Liegt der Schwerpunkt der Webseite auf dem Inhalt oder Darstelllung und Benutzererfahrung?
* Dynamisch generierte Inhalte können langfristig oft nur schwer oder gar nicht erhalten bleiben.
* Organisieren Sie Ihre Daten auf der Webseite systematisch und verwenden Sie klare Metadaten für eine bessere Suchbarkeit.
* Setzen Sie ein System zur Versionierung von Inhalten ein, um Veränderungen und Entwicklungen Ihrer Webseite nachvollziehbar zu machen.
* Achten Sie auf Zugriffskontrollen und Datenschutzmaßnahmen, um sensible Daten zu schützen.
* Implementieren Sie regelmäßige Backup-Routinen, um die Sicherheit Ihrer Daten zu gewährleisten.
* Erwägen Sie die Speicherung von wichtigen Daten, wie z.B. Datenbanken hinter einer Webseite, auf unabhängigen archivierenden Plattformen, die auf die langfristige Datensicherung spezialisiert sind.
* Überwachen Sie regelmäßig die technologische Alterung eingesetzter Systeme Ihrer Webseite und passen Sie Ihre Archivierungsmethoden an.
* Wählen Sie einen zuverlässigen Webhosting-Anbieter und sorgen Sie für ausreichend Speicherplatz, um zukünftige Datenmengen zu bewältigen.
* Strukturieren Sie Ihre Daten im Voraus für eine mögliche Datenmigration, wenn ein Wechsel des Hosting-Anbieters erforderlich ist oder die Webseite dauerhaft an andere übergeben wird.
* Erwägen Sie die Zusammenarbeit mit Organisationen, die auf die langfristige Archivierung von Daten spezialisiert sind.
* Dokumentieren Sie ausführlich, wie Ihre Daten archiviert und verwaltet werden, um zukünftigen Generationen die Nutzung der Informationen zu erleichtern.
* Bilden Sie Ihr Team und Stakeholder über die Bedeutung der Datenarchivierung aus und sensibilisieren Sie sie für bewährte Praktiken.

Indem Sie diese Schritte bei der Erstellung Ihrer Webseite berücksichtigen, stellen Sie sicher, dass Ihre digitalen Informationen und kulturelles Erbe für die Zukunft bewahrt werden und langfristigen Mehrwert zu bieten.

## Informationsmodelle
Verwenden Sie klare und konsistente Informationsmodelle, um die Struktur und Organisation Ihrer Webseite zu definieren und stellen Sie sicher, dass die Informationsmodelle flexibel genug sind, um zukünftige Änderungen und Erweiterungen zu ermöglichen. Die Wahl des Informationsmodells für die Darstellung von Daten einer Webseite hat einen direkten Einfluss auf die digitale Datenarchivierung; dies sollte auch berücksichtigt werden, wenn unterschiedliche Informationsmodelle auf einzelnen Webseiten eines Internetauftritts verwendet werden. Jedes dieser Informationsmodelle besitzt eigene signifikante Eigenschaften, die erhalten werden müssen, damit die Informationen erhalten und dauerhaft sinnvoll nutzbar bleiben.
### Wesentliche Fragen
> Welche Informationsmodelle existieren?
> Welches sind die kritischen Aspekte bei der Archivierung?

Hier sind exemplarisch verschiedene Informationsmodelle aufgeführt und wie sie sich auf die Archivierung der digitalen Inhalte auswirken:

**Hierarchisches Informationsmodell**
Hierarchische Modelle strukturieren Informationen in einer Baumstruktur mit Haupt- und Unterkategorien. Wie z.B. in einem Web-Shop können Produkte in Kategorien und Unterkategorien organisiert werden. Die Hierarchie könnte sein: Elektronik (Hauptkategorie) → Smartphones (Unterkategorie) → Android (Unterkategorie).
 > Bei der Archivierung ist es wichtig, die Hierarchie und Struktur beizubehalten. Sowohl die Haupt- als auch die Unterkategorien sollten klar erkennbar sein. Metadaten, die die Beziehungen zwischen den Kategorien beschreiben, sind hilfreich.

**Netzwerk-Informationsmodell**
Das Netzwerk-Modell ermöglicht nichtlineare Navigation, bei der Benutzer von einem Punkt zum anderen springen können. Wikipedia ist ein Beispiel, bei dem Artikel miteinander verknüpft sind. Benutzer können von einem Artikel zum nächsten über interne Links navigieren.
> Die Archivierung erfordert die Erfassung von Hyperlinks und Verweisen, um die Navigation und Verknüpfungen der Webseite zu erhalten. Es ist wichtig, dass Benutzer nahtlos zwischen den verknüpften Inhalten wechseln können.

**Tabellarisches Informationsmodell**
Tabellenstrukturen ordnen Informationen in Spalten und Zeilen an. In einem Preisvergleichsportal können die Produkte in Zeilen und deren Eigenschaften in Spalten angezeigt werden.
> Die Archivierung erfordert die Aufrechterhaltung der Tabellenstruktur, um sicherzustellen, dass Informationen in den gleichen Spalten und Zeilen wie auf der Webseite angezeigt werden.

**Ebenenbasiertes Informationsmodell:**
Ebenenbasierte Modelle ermöglichen die interaktive Navigation durch verschiedene Ebenen von Informationen, wobei jede Ebene spezifische Aspekte der Informationen repräsentiert, wodurch komplexe Informationen in klar verständliche Schichten unterteilt werden und eine verständliche Darstellung ermöglicht. Ein Beispiel ist eine interaktive Infografik, bei der Benutzer auf verschiedene Teile der Grafik klicken, um detaillierte Informationen anzuzeigen. Oft steht hier die Art und Weise der Darstellung im Vordergrund.
> Die Archivierung muss die Interaktivität und die Navigation zwischen den Ebenen bewahren, um das ursprüngliche Benutzererlebnis wiederherzustellen. Dies erfordert eine sorgfältige Erfassung von Interaktionen.

**Listenbasiertes Informationsmodell**
Listen bieten Informationen in einer klaren, linearen Struktur. Ein FAQ-Abschnitt auf einer Webseite ist ein Beispiel für eine listenbasierte Darstellung.
> Bei der Archivierung ist es wichtig, die Reihenfolge und den Listenstil beizubehalten. Die Informationen sollten in der gleichen geordneten Abfolge wiederhergestellt werden.

**Kartenbasiertes Informationsmodell**
Kartenmodelle werden für geografische Informationen und Standorte verwendet. Beispiele sind Karten-Dienste, bei denen Benutzer auf Standorte klicken, um weitere Details anzuzeigen.
> Die Archivierung kartenbasierter Modelle erfordert die Beibehaltung des geografischen Kontexts, Koordinaten und der interaktiven Kartenfunktionen.

**Zeitbasiertes Informationsmodell**
Zeitbasierte Modelle betonen die chronologische Abfolge von Informationen. Beispiele sind Zeitachsen, Zeitreihendatenbanken oder Gantt-Diagramme, wo die zeitliche Dimension ein wesentlicher Aspekt der zu organisierenden Daten ist und wichtig für das Verständnis von Abläufen, Entwicklungen und Trends ist.
> Die Archivierung muss die chronologische Reihenfolge und die zeitlichen Beziehungen der Informationen bewahren. Das Wiederherstellen von Ereignissen und Updates ist wichtig.

Die Archivierung dieser Modelle erfordert sorgfältige Planung und Dokumentation, um die ursprüngliche Struktur und Funktionalität der Webseite zu bewahren. Je nach Modell müssen spezifische Anforderungen und Beziehungen berücksichtigt werden.
## Technisches
### Grundsätzliches
Bei der Archivierung und Nutzung von Webarchiven muss klar sein, dass die archivierte Webseite in den meisten Fällen nur eine Annäherung an die originale Seite ist. Wenn nicht alle Bereiche einer Webseite archiviert werden können, etwa durch nicht zugängliche Bereiche, eingebundene Inhalte, dynamisch generierte Inhalt etc., können für die Auswertung und Nutzung des Archivs "blinde Flecken"[^8] entstehen. Um diesen "blinden Flecken" entgegenzuwirken wird die Orientierung und Einhaltung von technisches Standards empfohlen. Dies kann insgesamt den Zugang, die Archivierung und das Finden von Inhalten verbessern.

### Wesentliche Fragen
> Welche Webstandards können für die Webseitenarchivierung relevant sein?
> Welche technischen Aspekte sollten beim Aufbau einer Webseite berücksichtigt werden?
> Mit welchen Metadaten sollte die Webseite ausgezeichnet werden?

#### Überblick Webseitenarchivierung
Webseitenarchivierung bedeutet Inhalt, Struktur, Funktionalität und die Front-End-Präsentation(en) einer Website mithilfe unterschiedlicher Ansätze oder Webarchivierungstools zu erhalten und später erneut zu präsentieren. Es gibt verschiedene Arten, die je nach den Anforderungen und Zielen unterschiedlich eingesetzt werden. Die gängigsten Arten sind

**1. Statische Archivierung**

***HTML-Speicherung***
Es werden statische HTML-Schnapshots der Webseite erstellt und gespeichert.

***Screenshot-basiert***
Hierbei werden Screenshots der Webseite zu verschiedenen Zeitpunkten erstellt, um die visuellen Veränderungen im Laufe der Zeit zu dokumentieren. Da es sich lediglich um Abbildungen der Webseite handelt, ist eine Suche oder Interaktion nicht möglich. Dynamisch generierte Inhalte oder auf Nutzerinteraktion ausgelegte Inhalte können derzeit oft nur mit Screenshots bzw. Screencasts und zusätzlichen Text- bzw. Audiobeschreibungen dokumentiert werden.

**2. Dynamische Archivierung**

***Crawling und Scraping***
Webcrawler durchsuchen aktiv das Internet oder bestimmte Internetauftritte, folgen Verlinkungen und extrahieren Inhalte von Webseiten. Die archivierten Webseiten werden oft als WARC-Dateien gespeichert und haben oft nicht den vollen Funktionsumfang der originalen Webseite.

**3. Archivierungsprojekte und -organisationen:**
Es gibt Organisationen, die sich auf die Archivierung von Webinhalten spezialisiert haben, wie die Wayback Machine von der Internet Archive Foundation.

**4. Content-Management-Systeme (CMS)**
Einige Content Management Systeme bieten Funktionen zur Versionierung von Inhalten an, die eine Art von Archivierung ermöglichen. Die Nachhaltigkeit und das Format des Archivs sind nicht standardisiert und müssen gegen die Archivanforderungen geprüft werden.

### W3C-Standards
Das World Wide Web Consortium (W3C) hat einige Standards entwickelt, deren Einhaltung die langfristige Verfügbarkeit gewährleisten können. Diese Standards sorgen für eine bessere Struktur und Konsistenz von Webseiten, was wiederum die Archivierung erleichtert. 

Relevante [W3C-Standards](https://www.w3.org/standards/):

1. **[HTML (Hypertext Markup Language)](https://html.spec.whatwg.org/multipage/)**
HTML ist der grundlegende Baustein des Webs und wird vom W3C standardisiert. Die Verwendung aktueller HTML-Versionen, wie HTML5, sorgt für eine klare und einheitliche Struktur von Webseiten, was die Archivierung vereinfacht.

2. **[CSS (Cascading Style Sheets)](https://www.w3.org/Style/CSS/)**
CSS ist ein weiterer Standard des W3C und wird verwendet, um das visuelle Erscheinungsbild von Webseiten zu gestalten. Die Trennung von Inhalt (HTML) und Darstellung (CSS) erleichtert die Erfassung des eigentlichen Inhalts bei der Archivierung.

3. **[XML (Extensible Markup Language)](https://www.w3.org/XML/)** 
XML ist ein Standard zur Strukturierung von Daten, der auch bei der Archivierung von strukturierten Informationen auf Webseiten hilfreich sein kann.

4. **[Web Annotations](https://www.w3.org/TR/annotation-model/)**
Dieser W3C-Standard ermöglicht das Hinzufügen von Kommentaren, Anmerkungen und Metadaten zu Webinhalten. Dies kann bei der Dokumentation und Interpretation von archivierten Inhalten hilfreich sein.

5. **[Web Components](https://www.w3.org/TR/?filter-tr-name=&tags%5B%5D=browser)**
Web Components sind eine Sammlung von W3C-Standards, die die Erstellung wiederverwendbarer Webkomponenten erleichtern. Dies kann die Pflege und Wartung von Webarchiven rationalisieren.

6. **[Linked Data](https://www.w3.org/TR/?tags[0]=data)**
Linked Data-Prinzipien fördern die Vernetzung von Daten im Web. Diese Vernetzung kann bei der Archivierung dazu beitragen, Beziehungen zwischen verschiedenen Webinhalten besser zu verstehen.

7. **[Zeichensätze](https://www.w3.org/International/questions/qa-what-is-encoding.de)**
Zur korrekten Darstellung der Inhalte und Indexierung in Suchmaschinen ist die Zeichenkodierung, also der eindeutigen Zuordnung von Buchstaben, Ziffern, Sonderzeichen und Symbolen, eindeutig anzugeben. Die Inhalte sollten standardmäßig in UTF-8 codiert werden.

Diese W3C-Standards tragen dazu bei, die Struktur und Konsistenz von Webinhalten zu gewährleisten, was wiederum die Erfassung und Archivierung von Webseiten vereinfacht. Die Verwendung dieser Standards unterstützt die Langzeitarchivierung und erleichtert die spätere Rekonstruktion von Webinhalten.

### Robots
Bestimmte Arten von Anweisungen in der ```robots.txt```-Datei können zwar gut für Suchmaschinen-Crawler sein, aber sie können verhindern, dass Archivierungscrawler wichtige Webseiteninhalte erfassen, die für eine genaue Wiederherstellung der Webseite entscheidend sind. Zum Beispiel könnte die Anweisung an Crawler, bestimmte Verzeichnisse wie CSS und JavaScript auf einer Webseite zu meiden, für Suchmaschinen-Crawler nicht viel ausmachen, aber sie würden einen großen Unterschied in der Qualität der archivierten Aufzeichnung machen.

### Sitemaps, Links und Navigation
Ein Webcrawler kann nur Webseiten erfassen, die ihm bekannt sind. Er funktioniert, indem er Links folgt, was bedeutet, dass er letztendlich nur Seiten archivieren kann, die über Links zugänglich sind. Daraus folgt, dass ein Benutzer, der eine archivierte Webseite nutzt, nur durch das Folgen von Links navigieren kann, da serverseitige Funktionen wie die Suche im Archiv nicht funktionieren. Vermeiden Sie daher, sich ausschließlich auf JavaScript oder andere Techniken zu verlassen, die Links verschleiern könnten, um zu einer bestimmten Seite zu navigieren, und erwägen Sie die Erstellung[^12] einer umfassenden Sitemap, um sicherzustellen, dass der Crawler nichts übersieht und später im Webarchiv problemlos durchsucht und navigiert werden kann. Dies erleichtert die Erfassung und den späteren Zugriff auf Ihre Webseite und deren Inhalte. 
Eine Sitemap ist eine strukturierte Liste oder Datei, die Informationen über die Organisation, Hierarchie und Inhalte einer Website enthält. Eine spezielle Art von Sitemap ist eine XML-Sitemap, die v.a. für Suchmaschinen erstellt wird und in XML formatiert ist. Sie enthält Informationen über alle relevanten URLs auf der Website, einschließlich Metadaten wie die Zeit der letzten Aktualisierung, die Häufigkeit der Änderungen und die Priorität der Seiten. Sie ist vor allem für Suchmaschinen gedacht und erleichtert ihnen das effiziente Crawlen und Indexieren der Webseite, ist aber genauso nützlich für Archivierungs-Crawler.

#### Stabile URLs und Weiterleitung
Um Kontinuität und Zugänglichkeit von Webseitenaufnahmen in Webarchiven zu gewährleisten, ist es entscheidend, stabile URLs beizubehalten und bei Bedarf Weiterleitungen zu verwenden. Die Stabilität einer URL über die Zeit ermöglicht es, eine lückenlose Serie von Webseiten-Snapshots zu erstellen. Wenn eine URL geändert und keine Weiterleitung zur neuen Adresse eingerichtet wird, sinkt die Wahrscheinlichkeit, dass die neue URL beim nächsten Archivierungs-Crawl gespeichert wird. Dies führt praktisch dazu, dass der Zugriff auf die archivierte Webseite vor der URL-Änderung von denen nach der Änderung getrennt wird. Webarchivierungstools sind empfindlich gegenüber der URL-Stabilität, was auch bedeutet, dass URLs mit Sitzungs-IDs von früheren Aufnahmen derselben Ressource getrennt sein können.

### Metadaten
Verbesserung von Metadaten heben die Lesbarkeit des Inhalts für Suchmaschinen, seine Auffindbarkeit sowie zeitliche Einordnung in Webarchiven. Die Zeitstempel, die mit archivierten Inhalten in einem Webarchiv verknüpft sind, geben an, wann der Crawler die Seite besucht hat, jedoch nicht unbedingt, wann sie veröffentlicht oder aktualisiert wurde. Die Angabe des Veröffentlichungsdatums oder des letzten Updates über den HTTP Last-Modified-Antwortheader und/oder den Text im Dokument hilft dann den Nutzern, den zeitlichen Kontext des Inhalts besser zu verstehen. Zeitstempel sind auch in rechtlichen Verfahren wertvoll, da sie belegen, wann der Inhalt möglicherweise veröffentlicht oder aktualisiert wurde.
Die Verwendung von seitenbezogenen Titeln und Beschreibungselementen ```<META>``` erleichtert die Kuratierung von Webseiten durch Webarchive, und verbessert die Darstellung von Suchergebnis-Zusammenfassungen.

### Webseitentest auf Archivfähigkeit
Auf der Seite [ArchiveReady.com](https://archiveready.com/) kann die Archivierbarkeit der Webseite anhand von u.a. HTML-Validität, Seitenstruktur, Robots.txt, Verlinkung und Sitemap getestet werden. Die Tests in ArchiveReady.com sind bei weitem nicht erschöpfend, geben aber einen ersten Überblick und gute Anhaltspunkte, wo Schwachstellen der getesteten Webseite hinsichtlich Webarchivierung sind.

## Dateiformate und Datenbanken
Obwohl eine Webseite als eine Einheit wahrgenommen wird, besteht sie aus einer Vielzahl von Dateien und Dateitypen. Die langfristige Pflege einer Webseite bedeutet daher auch die langfristige Pflege dieser Typenvielfalt. Offene Standards und Formate sind daher beim Aufbau einer Webseite proprietären Formaten vorzuziehen. Unabhängig von der Offenheit des Standards spielen auch die allgemeine Verbreitung, Bekanntheit und Dokumentation eine Rolle.

### Wesentliche Fragen
> Welche Dateiformate werden für die Webseite verwendet?
> Wie nachhaltig sind die eingesetzten Dateiformate?
> Wie ist der Prozess der Datenmigration organisiert?

### Nachhaltigen Dateiformate

Empfehlenswert für die Einschätzung von Dateiformaten sind die Nachhaltigkeitsfaktoren der der US-Amerikanischen Library of Congress.[^7] Diese empfiehlt sieben Faktoren für die Einschätzung von Dateiformaten: 

**1. Offenlegung**
Hierbei geht es um die Frage, in wie fern vollständige Spezifikationen und Werkzeuge zur Validierung der technischen Vollständigkeit existieren und ob sie (frei) zugänglich sind.

**2. Annahme durch Nutzende**
Dies bezieht sich darauf, wie verbreitet das Format ist. Dies umfasst auch die Verwendung als sogenanntes Masterformat, also für die Bereitstellung an Endnutzenden aber auch als Transportformat zwischen technischen Anwendungen.

**3. Transparenz**
Hiermit ist die Offenheit der digitalen Darstellung für eine direkte Analyse gemeint; beispielsweise die Lesbarkeit mit einem reinen Texteditor.

**4. Selbstdokumentation**
Die dokumentierenden Objekte enthalten grundlegende beschreibende, technische und andere administrative Metadaten.

**5. Externe Abhängigkeiten**
Grad der Abhängigkeit eines bestimmten Formats von einer bestimmten Hardware. Dies geht auch einher mit der Frage nach einer voraussichtlichen Komplexität im Umgang mit zukünftigen Abhängigkeiten.

**6. Auswirkungen von Patenten**
Ausmaß der Beeinträchtigung durch Patente, die sich negativ auf die Fähigkeit von Archivierungseinrichtungen auswirken bestimmte Inhalte in einem Format aufrechtzuerhalten.

**7. Technische Schutzmechanismen**
Implementierung von Mechanismen wie Verschlüsselung, welche die Aufbewahrung von Inhalten durch ein vertrauenswürdiges Repository verhindern.

### Dateiformate
Die Wahl der Dateiformate für die Archivierung ist ein wesentlicher Faktor für den Erfolg (oder Misserfolg) einer digitalen Archivierung. Hier hat sich vor allem gezeigt, dass Eigenentwicklungen im Hinblick auf die Langzeitverfügbarkeit ein hohes Risiko des Scheiterns in sich bergen. Sinnvoller ist es dagegen, sich an bestehenden Standards zu orientieren. Ein Standard ist besser als kein Standard.

Gleichzeitig wird empfohlen, die Dateiformate und die damit verbundene Soft- und Hardware so offen wie möglich und so geschlossen wie nötig zu gestalten. Nicht-proprietäre Formate sind in der Regel durch den Open-Source-Gedanken langfristig erhalten. Und wo dies nicht gegeben ist, kann zumindest der Code, die Dokumentation etc. eingesehen und für das eigene technische Archivierungskonzept nutzbar gemacht werden.

Dennoch ist es sinnvoll, bei der Wahl der Dateiformate auch community-spezifische Aspekte des eigenen Wissenschaftsgebietes zu berücksichtigen. Der Umgang mit Dateiformaten kann daher nicht verallgemeinert werden. Es empfiehlt sich daher, die eigene Fachcommunity als Zielgruppe mitzudenken. Auch die technischen Gepflogenheiten eines Internetauftritts sollten berücksichtigt werden.

Auf der Suche nach konkreten Dateiformaten für die Archivierung sind zwei Anlaufstellen besonders zu empfehlen. Die Library of Congress in Washington bietet einen umfassenden Überblick über [langlebige Dateiformate](https://www.loc.gov/preservation/digital/formats/index.html). Besonders empfehlenswert ist dort der [Abschnitt zu qualitativen und funktionalen Faktoren bei der Archivierung von Webseiten](https://www.loc.gov/preservation/digital/formats/content/webarch_quality.shtml). Die Schweizerische Koordinationsstelle für die dauerhafte Archivierung elektronischer Unterlagen (KOST) bietet einen umfassenden [Katalog archivischer Dateiformate](https://kost-ceco.ch/cms/kad_main_de.html). Insbesondere die [Übersicht zu Standards und Richtlinien in der digitalen Archivierung](https://kost-ceco.ch/cms/standards_de.html) eignet sich für eine erste Orientierung in dieser Thematik.

> **Exkurs Archivformat**
> Neben den archivtauglichen Dateiformaten gibt es auch spezielle Dateiformate für die Archivierung von Webanwendungen. Ein Quasi-Standard für die Archivierung von Webseiten ist [Web ARChive (.warc file)](https://iipc.github.io/warc-specifications/specifications/warc-format/warc-1.1/).[^3] Das WARC-Format bietet eine standardisierte Möglichkeit, verschiedene Arten von Ressourcen, wie HTML, Bilder, Stylesheets und andere Dateien, mit speziellen Metadaten angereichert in einem einzigen Archiv zu speichern. Es ist das Standardformat vieler Archiv-Crawler und Archiv-Dienstleister.
### Datenmigration
Der Punkt der Datenübergabe ist einer der kritischen Momente bei der Archivierung von Webseiten. Er markiert den Übergang vom Arbeits- in den Archivmodus. Die Phase der inhaltlichen Bearbeitung ist damit abgeschlossen. Im Archivmodus findet praktisch keine inhaltliche Bearbeitung oder Überarbeitung mehr statt. Dieser Zeitpunkt der Datenmigration stellt in der Regel eher eine prozessuale als eine technische Herausforderung dar. Denn die Nutzer müssen sich davon verabschieden, dass die "eigene" Webseite nicht mehr unter ihrer (inhaltlichen) Kontrolle steht. Dem steht jedoch der Vorteil der Langzeitarchivierung und damit der Verfügbarkeit von Information und Form gegenüber.

Die Form der Datenmigration hängt stark von der Struktur und den technischen Gegebenheiten der Webseite ab. Für Internetauftritte, die beispielsweise viele PDF-Dateien enthalten, müssen andere Migrationsstrategien entwickelt werden als für Projektwebseiten, die überwiegend aus html-Elementen bestehen. Dies zeigt zugleich, dass archivfreundliche Plattformen als Basis langfristig einen Vorteil bieten. Weit verbreitete Content Management Systeme wie Wordpress bieten bereits Archivierungsfunktionen und umfangreiche Dokumentation. Open-Source-Systeme bieten hier zugleich den Vorteil, dass es meist Communities mit anderen gibt, die möglicherweise bereits Antworten auf solche Fragen gefunden haben oder gemeinsam danach suchen. Dies kann die Migration von Daten für die Archivierung von Webseiten deutlich vereinfachen.

## Graphische Darstellungen
Die Wiedergabe von grafischen Elementen einer Webseite im archivierten Zustand ist mit zahlreichen Herausforderungen verbunden. Die Probleme steigen in der Regel exponentiell mit der Komplexität der visuellen Elemente. Je einfacher die technischen Elemente einer Webseite sind, desto besser ist sie in Form und Inhalt zu archivieren.

### Wesentliche Fragen
> Werden externe Erweiterungen genutzt?
> Welche Bedeutung haben graphische Elemente für die Webseite?
> Welche Bedeutungsinformationen transportieren graphische Elemente? Und wie können sie langfristig bei geringer technischer Komplexität erhalten bleiben?

### Reduktion von externen Erweiterungen

Technische Elemente wie Erweiterungen, Plugins, externe Bibliotheken, Online-Datenbanken etc. erhöhen die Komplexität der Anwendung. Ihr Einsatz bedeutet für die Archivierung, dass eine reine Bitstream-Erhaltung in den meisten Fällen nicht ausreicht, um z.B. die grafischen Darstellungen interaktiver Karten zu erhalten. Das Zusammenspiel der technischen Systeme macht es notwendig, dass die Funktionalitäten der Schnittstellen erhalten bleiben.

Um solche Abhängigkeiten in der Pflege zu reduzieren, empfiehlt es sich, möglichst sparsam mit dynamischen und eingebetteten externen Elementen umzugehen. Durch den Verzicht auf Plugins und individuelle Erweiterungen werden Pfadabhängigkeiten vermieden, so dass die Archivierung weniger komplex und auch langfristig stabiler durchgeführt werden kann.

### Wiedergabe des visuellen Eindrucks

Die visuelle Darstellung von Webseiten ist in der Regel eine wesentliche Information, die es bei der Archivierung möglichst vollständig wiederzugeben gilt. Gleichzeitig werden Browser als interpretierende Software für Webseiten ständig weiterentwickelt. Dies führt langfristig zu Problemen bei der Darstellung von z.B. Bildern, grafischen Elementen wie Menübändern, die aber für den ursprünglichen Eindruck einer Webseite wesentlich sind.
Um den visuellen Eindruck von html-basierten Seiten zu erhalten, empfiehlt z.B. die KOST das Format [PDF/A-2 für Hypertext](https://kost-ceco.ch/cms/pdf-a-2-fuer-hypertext.html). Damit können html-Dateien und deren grafische Interpretation wiedergegeben werden. Bei der PDF-Darstellung bleibt die grafische Gestaltung zum Zeitpunkt der Archivierung erhalten. Angesichts der ständigen Weiterentwicklung der Browser-Technologien ist dies ein nicht zu unterschätzender Aspekt für die Langzeitarchivierung wissenschaftlicher Webseiten.


### Strategische Planungen zur "Look&Feel"
Bei der Planung der eigenen Webseite ist es daher besonders ratsam, sich über die Anforderungen und Wünsche an die graphische Darstellung im Klaren zu sein. Je komplexer die Gestaltung der Webseite, desto schwieriger gestaltet sich in der Regel die Archivierung der Webseite. Es ist sinnvoll, diesen Zielkonflikt frühzeitig zu thematisieren, um explizite Vorgaben und Maßnahmen zu etablieren. So können die eigenen Anforderungen und die technischen Möglichkeiten in Einklang gebracht werden.
Wird diese Entscheidung aufgeschoben und erst kurz vor der Archivierung getroffen, ist es in der Regel zu spät. Dies kann letztlich auch bedeuten, dass die Webseite doch nicht archiviert und damit unwiderruflich gelöscht wird.

## Maschinen-Lesbarkeit
Künstliche Intelligenz (KI oder auch AI) steht dank den beeindruckenden Fähigkeiten aktueller Sprachmodelle grell im Rampenlicht. Intelligente Chatbots verdeutlichen eindrucksvoll den aktuellen Stand von Forschung und Entwicklung im Bereich der Textanalyse und Textgenerierung. Der Erfolg von KI-Lösungen hängt jedoch nicht allein davon ab, geeignete Algorithmen für den jeweiligen Anwendungsbereich zu haben, sondern zum Training dieser Sprachmodelle werden wiederum möglichst gut aufbereitete Texte und Daten benötigt. Sollen für ein Forschungsprojekt Texte aus einem Korpus archivierter Webseiten extrahiert werden spielt die Gestaltung der Webseiten eine wichtige Rolle. Eine Webseite kann so aufgebaut sein, dass Textextraktion besonders effizient und genau erfolgen kann.

### Wesentliche Fragen
> Warum ist Maschinenlesbarkeit wichtig?
> Welche Aspekte sind beim Webdesign dazu zu berücksichtigen?

Die Umsetzung folgender Praktiken trägt dazu bei, dass Textextraktionstools und Suchmaschinen den Inhalt Ihrer Webseite besser erfassen und interpretieren können:

**1. Semantische HTML-Struktur**
Verwenden Sie eine klare, semantische HTML-Struktur. Das bedeutet, Verwendung von Überschriftentags (h1, h2, h3, usw.) für Überschriften, Absatztags (p) für Absätze und Listen für Listen. Dies erleichtert die Identifikation und Extraktion von Textelementen.

**2. Aussagekräftige Klassen und IDs**
Verwenden Sie CSS-Klassen und IDs, um Textelemente zu kennzeichnen, insbesondere wenn sie spezielle Bedeutung haben. Dies erleichtert das gezielte Extrahieren von Text aus bestimmten Abschnitten der Webseite.

**3. Vermeidung von komplexen Layouts**
Übermäßig komplexe Layouts, insbesondere solche, die hauptsächlich durch CSS und JavaScript generiert werden, können die Textextraktion erschweren. Bemühen Sie sich, ein einfaches und verständliches Layout zu verwenden.

**4. Strukturierte Metadaten**
Fügen Sie Metadaten wie Autoreninformationen, Erstellungs-, Veröffentlichungs- und Änderungsdaten, sowie Kategorien hinzu. Diese Informationen können bei der Extraktion und beim Verstehen des Kontexts hilfreich sein.

**5. Alternative Texte für Medien**
Wenn Sie Bilder oder andere Medien verwenden, versehen Sie sie mit alternativem Text (alt-Text), um deren Inhalt zu beschreiben. Dies ist wichtig, um den Textinhalt dieser Elemente zu verstehen.

**6. Klare Trennung von Inhalten**
Trennen Sie den Haupttextinhalt von Nebeninformationen wie Navigationselementen, Werbung und so weiter. Dies kann mithilfe von HTML-Tags und CSS erreicht werden.

**7. Nutzung von Microdata und Strukturierten Daten**
Verwenden Sie strukturierte Datenmarkierungen wie Schema.org, um wichtige Informationen auf der Webseite zu kennzeichnen. Suchmaschinen und Textextraktionswerkzeuge können diese Markierungen nutzen, um den Inhalt besser zu verstehen.

**8. Gültiges HTML und CSS** 
Stellen Sie sicher, dass Ihr HTML und CSS den Standards entsprechen. Fehler im Code können die Textextraktion beeinträchtigen.


## Webseiten-Archivierung in den Leitlinien zur guten wissenschaftlichen Praxis
Die langfristige Archivierung von Webseiten im wissenschaftlichen Kontext findet in unterschiedlichen normativen Rahmen statt.

### Wesentliche Frage
> Betreffen die Leitlinien im DFG-Kodex auch die eigene Projektwebseite?
> Gibt es eine institutionelle Regelung zur Archivierung von Projektwebseiten?
> Existieren community-spezifische Standards bei der Webseite-Archivierung?

### Webseiten-Archivierung im DFG-Kodex

Grundlegend im bundesdeutschen Zusammenhang sind hierfür zuerst die [DFG "Leitlinien zur Sicherung guter wissenschaftlicher Praxis"](https://www.dfg.de/download/pdf/foerderung/rechtliche_rahmenbedingungen/gute_wissenschaftliche_praxis/kodex_gwp.pdf). Laut dieser sind Wissenschaftler dazu verpflichtet die zugrunde liegenden, zentralen Materialien ihrer Forschung für einen angemessenen Zeitraum aufzubewahren.[^1] Hierunter können auch Projekt-Webseiten fallen. Üblicherweise bezieht sich der Zeitraum auf zehn Jahre nach Projektende. Je nach Fall und Relevanz kann diese Spanne aber auch (freiwillig) verlängert werden.

### Institutionelle Regelungen zur Webseiten-Archivierung

Parallel dazu besitzt jede bundesdeutsche Institution in der Wissenschaft eine eigenes Regelwerk zur guten wissenschaftlichen Praxis (GWP).[^2] In diesen internen Regelwerken kann ebenso die Verfügbarkeit von Forschungsergebnissen über das Projektende hinaus klarer geregelt sein.
Gleichzeitig gilt es bei Kooperationsprojekte zu beachten, dass die Partner gegebenenfalls unterschiedliche institutionellen Regelungen unterliegen. Solchen Problemen lässt sich durch eine frühzeitige Klärung, idealiter schon im Kooperationsvertrag bzw. gemeinsamen Drittmittelantrag, beheben.

### Fachspezifische Perspektive auf die Webseiten-Archivierung

Fachspezifische Regelungen können ebenso die Archivierung von forschungsgezogenen Webseiten betreffen. So können beispielsweise die [DFG-Fachkollegien fachspezifische Empfehlungen zum Umgang mit Forschungsdaten](https://www.dfg.de/foerderung/grundlagen_rahmenbedingungen/forschungsdaten/empfehlungen/index.html) veröffentlichen, welche auch Handlungsempfehlungen bei der Webseite-Archivierung formulieren. Es gilt daher bei der Archivierungsentscheidung auch immer der fachspezifische Kontext des Forschungsprojekts zu beachten. 

## Rechtliche Fragestellungen[^13]
Rechtliche Fragestellungen betreffen vielfach die Archivierung von forschungsbezogenen Webseiten. Ausgehend von der Fragestellung der Urheberschaft entwickeln sich die Handlungsoption für den Umgang mit der zu archivierenden Webseite. Dies können Entscheidungen wie etwa Lizenzierungen, Fristen oder Übertragung des Eigentumsrechts sein.

### Wesentliche Fragen
> Wie sind die Eigentumsverhältnis bei der Webseite?
> Wer besitzt die Veröffentlichungs- und Verwertungsrechte?
> Hat die Webseite eine Lizenz?
> Wie ist die Abgabe der Webseite an die archivierende Institution geregelt? Gibt es einen Depositalvertrag?

### Klärung des Eigentumsrechts
Eine der zentralen rechtlichen Fragen bei der Archivierung von Webseiten ist das Eigentumsrecht: Von welchen Person oder Personengruppe ist die Webseite das Eigentum? Besonders im wissenschaftlichen Kontext ist diese Frage häufig nicht pauschal zu beantworten. Denn auf der einen Seite wird eine Projektseite zumeist im Rahmen eines Dienstverhältnisses erstellt. Dem Dienstherrn stände aber Veröffentlichungs- und Verwertungsrechte zu. Auf der anderen Seite steht grundsätzlich dem Urheber das Recht zu einer Publikation zu. Ebenso besteht in der Bundesrepublik nach [GG Art. 5 Abs. 3](https://www.gesetze-im-internet.de/gg/art_5.html) die Freiheit der Forschung. Für die Klärung dieser Sachlage kommt es auf die Details des Beschäftigungsverhältnisses und die jeweiligen vertraglichen Vereinbarungen an.[^4] Beim Outsourcen von Webseiten muss selbstverständlich zusätzlich geklärt werden, wie die Arbeiten von Entwicklungsfirmen und Hosting-Dienstleister bei der Archivierung widergegeben werden. Auch für die Übergabe von Daten und Code von Dienstleister zur archivierenden Institution sollten dringend vorab schon (vertragliche) Vereinbarungen getroffen werden.

Parallel dazu muss entscheiden werden, wie die Webseite eingeordnet wird. Ist sie überwiegend textlicher Natur und kann somit als wissenschaftliche Publikation gewertet werden? Oder überwiegen Aspekte von Datenbanken samt Architekturen, Verschachtelungen und Verknüpfungen? In einem solchen Fall könnte die Webseite auch als Datenbankwerk nach [UrHrG § 4](https://www.gesetze-im-internet.de/urhg/__4.html) in Betracht kommen.[^5] Auch hier ist nur eine Entscheidung am konkreten Beispiel möglich. Bitte ziehen Sie im Zweifel Experten aus der eigenen Institution zu Rate.

### Lizenz und Lizenzierungsmöglichkeiten

Der Eigentümer kann die Webseite mit einer Lizenz versehen. Dies sollte nach Möglichkeit auch geschehen. Durch diesen Rechtsakt wird nämlich explizit gemacht, welche Nutzungsmöglichkeiten seitens Eigentümer eingeräumt werden. Wie bei Software generell gilt es auch im Fall von Webseiten, dass die Kompatibilität von Lizenzen, falls externe Objekte nachgenutzt werden, beachtet werden müssen. Je nach Kontext müssen Webseite-Inhalte und technische Plattform als unterschiedliche rechtliche Entitäten bei der Archivierung  behandelt werden. Im Zweifelfall können die Rechtsexperten der eigenen Institution hierbei beratend unterstützend.

Bei der Suche nach Lizenzen können gängige Adressen wie https://choosealicense.com, https://opensource.org/licenses/ etc. unterstützen. Für Code-Komponenten ist es auf jeden Fall empfehlenswert Software-spezifische Lizenzen auszuwählen. Sie enthalten nämlich einen Haftungsausschluss für fehlerhaften Code, was etwa datenspezifische oder CC-Lizenzen nicht aufweisen.

### Barrierefreiheit
Die Nutzung von Webseiten kann mit Hindernissen versehen werden. Gerade für Menschen mit einer Behinderung kann dies eine besondere Herausforderung darstellen. Aus diesem Grund muss eine Webseite barrierefrei konzipiert sein. Hergeleitet wird dies durch die EU-Richtlinie 2016/2102 über den barrierefreien Zugang zu Webseiten und mobilen Anwendungen öffentlicher Stellen.[^10] In nationales Recht überführt wurde dies 2019 in Verordnung BITV 2.0.[^11] Diese gilt auch für öffentliche Hochschulen und Forschungseinrichtungen. Bei der Konzeption einer Webseite ist dieses geltende Recht daher zu beachten.

Für die konkrete Umsetzung sind die [Web Content Accessibility Guidelines (WCAG 2)](https://www.w3.org/WAI/standards-guidelines/wcag/) des W3C ein sinnvoller Standard. Mit [WAI-ARIA](https://www.w3.org/TR/wai-aria/) existieren beispielsweise konkrete Spezifikationen, die für Webseiten und deren barrierefreie Anwendung relevant sind. Gleichzeitig existieren auch viele digitale Werkzeuge, welche unterstützen die Barrierefreiheit einer Webseite zu schätzen. Beispiele hierfür sind etwa der [WCAG Contrast Checker](https://contrastchecker.com/), das [Web Accessibility Evaluation Tool](https://wave.webaim.org/) oder allgemein auch [BITV-Test](https://www.bitvtest.de).

### Depositum der Webseite

Das Depositum (aus dem Lateinisch von "Hinterlegtem") einer wissenschaftliche Webseite sollte alle für den Erhalt notwendigen Dateien, Informationen etc. enthalten. Mit dem Akt der Übergabe einher geht, dass die Webseite seitens Eigentümer nicht mehr bearbeitet werden kann. Der Archivmodus ist "read only". Soweit möglich sollten auch die vollumfänglichen Nutzungsrechte an der Webseite auf die archivierende Institution übertragen werden.

Es ist hierzu in jedem Fall sinnvoll einen Depositalvertrag zwischen Webseiten-Eigentümer und archivierender Institution abzuschließen. Hierdurch wird eine Rechtssicherheit für beide Parteien hergestellt, die klare Rahmen für die Dienstleistung und Erwartungen an die Archivierungen setzen. Notwendig für einen solchen Vertrag ist aber die klare rechtliche Einordnung im Bezug auf das Eigentumsrecht. Denn nur hierdurch ist geklärt, wer den Depositalvertrag rechtsverbindlich schließen darf. Ein solcher Vertrag kann auch Einschränkungen der Benutzung bzw. benutzungsrechtliche Fragen beinhalten. Dies könnten beispielsweise Zugangsbeschränkungen oder Embargofristen sein. 

Für die Archivierung einer Webseite kann die Übertragung der Eigentumsrechte unter Umständen empfehlenswert sein. Hintergrund hierfür ist, dass die erhaltende Institution hierdurch auch kuratorische Maßnahmen wie beispielsweise Datenbankaktualisierungen, Behebung von Sicherheitslücken vornehmen können. Je nach vereinbartem Erhaltungsszenario und Relevanz kann ein solches Vorgehen sinnvoll sein.

Ein Archivierungsrecht seitens Bibliotheken, ausgelegt als Recht auf eine redundante Speicherung und gegebenenfalls eine Transformation in andere Dateiformate, kann unter Umständen auch durch [UrhG § 60e Abs. 1-3](https://www.gesetze-im-internet.de/urhg/__60e.html) gedeckt sein. Dieser Weg sollte gemeinsame diskutiert werden, ob ein solcher Weg zusätzliche Chancen bietet.

## Datenschutz
Aspekte des Datenschutzes können auch die Langzeitarchivierung von Webseiten betreffen. Es ist daher sinnvoll so früh wie möglich über Datenschutz nachdenken. Schon bei der Designentscheidung für eine Webseitenstruktur und ihrer technischen Lösung sollte der Datenschutz auch mit Blick auf eine langfristige Erhaltung mitgedacht werden.[^6]

### Wesentliche Fragen
> Wurden auf der Webseite personenbezogene oder sensible Daten veröffentlicht?
> Liegen Daten der Webseite-Nutzer vor?

### Datenschutz beim Archivieren von Webseiten

Der Datenschutz kann bei einer wissenschaftlichen Webseite in zwei Richtungen wirksam werden. Zum einen kann er sich auf den Inhalt der Projektseite beziehen. Bei Forschungsvorhaben mit personenbezogenen Daten kann dies etwa der Fall sein. Hierbei sollte die Seite vor der Archiv-Phase ebenfalls schon nicht oder nur eingeschränkt öffentlich verfügbar sein. Diesen Umstand muss auch die Archivlösung widerspiegeln.

Zum anderen sind auch die technisch-prozessualen Daten der Nutzenden im Bezug auf den Datenschutz zu bedenken. So können beispielsweise Nutzer-Accounts für das Veröffentlichen und Bearbeiten mit zusätzlichen, persönlichen Information oder sogar lokalen Passwörter vorhanden sein. Wenn diese Angaben für die Nutzung der archivierten Webseite nicht zwingend notwendig sind, sollte in Erwägung gezogen werden diese nicht in den archivierten Zustand mit zu überführen. Ein Möglichkeit könnte beispielsweise auch eine technische Trennung schon im Betrieb von Projektwebseite und Nutzenden-Informationen sein.

Im Zweifelsfall ist es sinnvoll die lokalen Datenschutzbeauftragten zu kontaktieren. Diese können bei den weiteren Maßnahmen und ihrer Wirksamkeit beratend zur Seite stehen.

## Use Cases
### Projektende
In vielen Bereichen kann die Konzeption und der Start von Projekten und zugehörigen Webseiten auf einen bewährten Werkzeugkasten zurückgreifen. Jedoch wird dabei nur selten darüber nachgedacht, wie ein Projekt beendet wird, wenn die Förderung ausläuft und was mit den dabei entstandenen Internetseiten passiert. Quellenangaben sind ein wesentlicher Bestandteil des wissenschaftlichen Diskurses und dieser ist darauf angewiesen, dass Informationen dauerhaft weiter zur Analyse, Replikation, Verifikation und Zitation zur Verfügung stehen.
Zu beachten ist hier vor allem, was primär erhalten bleiben soll: Der Webseiteninhalt, die möglicherweise getrennt gespeicherten Forschungsergebnisse oder die Benutzererfahrung? Können die einzelnen Präsentationsschichten gegebenenfalls getrennt archiviert und wieder sinnvoll zusammengesetzt werden? Außerdem ist vor einer Archivierung die Seite auf möglicherweise noch vorhandene persönliche Informationen zu überprüfen, die nicht archiviert werden sollen.

### Ruhestand
Einen etwas weiteren Zeithorizont als Projektwebseiten haben oft von einzelnen Wissenschaftlern über einen längeren Zeitraum hinweg aufgebaute Webseiten. Diese entwickeln sich über die Jahre zu wichtigen Anlaufstellen innerhalb der wissenschaftlichen Community. Wenn der Betreiber der Webseite in den Ruhestand eintritt soll die Seite aber weiterhin erhalten bleiben. Um dies zu ermöglichen, kommt oft die Übernahme des Hostings durch - idealerweise - einen institutionellen Betreiber in Frage. In einem Off-Boarding-Prozess sind dann die Modalitäten der Übergabe ("Transfer of Ownership") zu klären wie etwa die Übergabe von Passwörtern und Admin-Zugängen oder die Übertragung auf andere Server. Ebenfalls möglich ist die Einrichtung eines stillgelegten Mirrors und die möglicherweise nötige Einrichtung von Weiterleitungen, damit Zitationen und Verlinkungen weiterhin aufgelöst werden können. Je weniger komplex eine Seite aufgebaut ist, desto einfacher kann sie langfristig im Netz erhalten bleiben.

### Datenvisualisierung. Karten, Diagramme, interaktive Grafiken
Heute müssen Daten nicht nur erhoben, bearbeitet und analysiert, sondern auch angemessen visualisiert werden um Aussagen über sie treffen zu können. Dies führt oft zu sehr komplexen interaktiven Darstellungen, in denen unter Umständen Text und Visualisierung sich sogar dem Lesefortschritt anpassen. Datenvisualisierung sind also ein mächtiges Werkzeug um numerische Fakten darzustellen. Es ist jedoch zu beachten, dass komplexe interaktive Karten nur schwer langfristig erhalten werden können - je mehr unterschiedliche Softwarekomponenten zur Darstellung benötigt werden, desto unwahrscheinlicher. Wenn das Ergebnis einer Visualisierung eine Grafik ist, sollte diese in einem etablierten Format erstellt werden (s. [Dateiformat](#Dateiformate) und [Darstellungen](#Darstellungen))

## Beispiele

### MPDL: Zeitschrift für Naturforschung
nach eigener Service als Webseite wegen geringem Interesse eingestellt; Webseite wurde komplett offline genommen und die entsprechenden PDF-Dateien der Zeitschriften-Jahrgänge als Dataset veröffentlicht: https://doi.org/10.17617/3.GRUJYR. Die ehemalige Domain https://zfn.mpdl.mpg.de leitet nun direkt auf das Dataset weiter.
Die Lösung bei der Webseiten-Archivierung bestand somit darin, dass der Inhalt in anderer Format langfristig erhalten bleibt aber die ursprüngliche Webseite nicht mehr präsentiert wird. Der Inhalt in Format von PDF-Dateien ging dabei vor der Form.

## Checkliste für Webseiten-Konzipierung
- [ ] Definition der Vermittlungsziele
- [ ] Festlegung einzusetzender Informationsmodelle
- [ ] Konzeption des logischen Webseitenaufbaus
- [ ] Festlegung der eingesetzten Technik
Die Vielfalt muss langfristig beherrschbar bleiben
- [ ] Festlegung der eingesetzten Dateiformate
Möglichst offene und verbreitete Formate nutzen
- [ ] Webdesign-Richtlinien festlegen ("Look & Feel")
Designentscheidungen und graphische Elemente haben direkten Einfluss auf die langfristige Archivierbarkeit der Webseite
- [ ] Identifikation eines Webhostinganbieters
- [ ] Festlegung eines Datenmanagementplans (zumindest aber einer Backup-Routine)
- [ ] Konzeption eines Versionierungskonzepts
Garantiert wissenschaftliche Zitierbarkeit und beugt "Content Drift" vor
- [ ] Datenschutz: Technisches Konzept prüfen
- [ ] Datenschutz: Design-Konzept prüfen
## Checkliste für die Webseiten-Archivierung
- [ ] Identifikation eines geeigneten Webarchivs bzw. Infrastrukturanbieters
- [ ] Identifikation erhaltenswerter Eigenschaften einer Webseite 
Mögliche signifikante Eigenschaften: Inhalt (Datenbankinhalte, Text etc.), Darstellung (Grafiken, Kartendarstellungen etc.), Struktur (z.B. zeitliche Abfolge) oder Benutzererfahrung (Animationen, Design, Look & Feel)
- [ ] Einstufung: Welche Informationen müssen, sollen oder können erhalten bleiben
- [ ] Metadatenauszeichnung der Inhalte
Ein Suche steht einem Webarchiv möglicherweise nicht zur Verfügung
- [ ] Klärung von Eigentumsrechten
- [ ] Klärung von Urheberrechten
- [ ] Entfernung urheberrechtlich geschützter Inhalte
- [ ] Prüfung auf datenschutzrelevante Inhalte
- [ ] Einrichtung Zugriffskontrolle und/oder Entfernung datenschutzsensibler Inhalte
- [ ] End-of-project-Release der Webseite erstellen
- [ ] Unabhängige Archivierung von Datenbanken in Forschungsdatenrepositorien
- [ ] Depositum-Vertrag mit archivierender Institution
- [ ] Daten und Software an archivierende Institution transferieren
- [ ] Dokumentation von archivierten Inhalten
- [ ] Dokumentation der angewandten Methoden
- [ ] Bekanntmachung der Archivierung

## Weitere Hinweise
### Literatur
* Bundesministerium für Bildung und Forschung: „Urheberrecht in der Wissenschaft Ein Überblick für Forschung, Lehre und Bibliotheken“, 2023, 2. Auflage, https://www.bmbf.de/SharedDocs/Publikationen/de/bmbf/1/31518_Urheberrecht_in_der_Wissenschaft.pdf?__blob=publicationFile&v=6.
* Dave Bunten und Gregory P. Way: „Long-Term Software Gardening Strategies for Cultivating Scientific Development Ecosystems“, 17.08.2023, https://bssw.io/blog_posts/long-term-software-gardening-strategies-for-cultivating-scientific-development-ecosystems.
* Digital Preservation Coalition (2023): Digital Preservation Documentation: A Guide, http://doi.org/10.7207/documentation-23.
* Bastian Gillner, Martin Hoppenheit und Franziska Klein: „Webarchivierung im Landesarchiv NRW“, in: Archivpflege in Westfalen-Lippe 96 (2022), S. 47–51, https://www.lwl-archivamt.de/media/filer_public/5b/d9/5bd9b059-6a16-4b3f-a6d4-d589343b05ab/47-51_gillner_hoppenheit_klein.pdf.
* European Archives Group of the European Union (EAG): Archiving by Design Whitepaper, 25.05.2023, https://commission.europa.eu/system/files/2023-06/Whitepaper%20AbD_en.pdf
* Michelle Lindlar: „Bewertung & Priorisierung archivierungswürdiger digitaler Objekte in der Praxis“, nestor-Praktikertag 2020, https://www.langzeitarchivierung.de/Webs/nestor/SharedDocs/Downloads/DE/praesentationen/2020praktikertagLindlar.pdf?__blob=publicationFile&v=1.
* Mark C. Miller: „Discontinuing a Research Software Project“, 04.12.2023, https://bssw.io/items/discontinuing-a-research-software-project.
* Laura Niebling: Wissenschaftliche Webseiten -- Vergangenheit, Gegenwart und Zukunft von Wissenschaft im Internet, 2020, https://mediastudies.hypotheses.org/1363.
* Stapelfeldt, Kirsta u. a.: „Strategies for Preserving Digital Scholarship“, The Code4Lib Journal 53 (2022), https://journal.code4lib.org/articles/16370.
* Andreas Weber und Claudia Piesche: „Datenspeicherung, -kuration und Langzeitverfügbarkeit“, in: Markus Putnings, Heike Neuroth und Janna Neumann (Hrsg.): Praxishandbuch Forschungsdatenmanagement, 2021, https://doi.org/10.1515/9783110657807-019, S. 327–356.
* Konstanze Weimer und Astrid Schoger: „Das Dateiformat WARC für die Webarchivierung“, 2021, https://files.dnb.de/nestor/kurzartikel/thema_15-WARC.pdf.

### Links
* Deutsche Nationalbibliothek: https://www.dnb.de/DE/Professionell/Sammeln/Sammlung_Websites/sammlung_websites_node.html
* GitHub Web Archiving Community https://github.com/ArchiveBox/ArchiveBox/wiki/Web-Archiving-Community
* Nestor: https://www.langzeitarchivierung.de
* nestor-Wiki: Einführung in die LZA, https://wiki.dnb.de/x/ObmkBQ
* nestor-Wiki: Webarchivierung, https://wiki.dnb.de/x/-rSkBQ
* Library of Congress, Creating Preservable Websites, https://www.loc.gov/programs/web-archiving/for-site-owners/creating-preservable-websites/

## Endnoten
[^1]: DFG, Leitlinien zur Sicherung
guter wissenschaftlicher Praxis, 2019, Leitlinie 17, S. 22 bzw. https://wissenschaftliche-integritaet.de/kodex/archivierung/.
[^2]: Siehe beispielsweise die [Ludwig-Maximilians-Universität München](https://cms-cdn.lmu.de/media/lmu/downloads/die-lmu/beauftragte/richtlinien-der-lmu-muenchen-zur-selbstkontrolle-in-der-wissenschaft.pdf) und die [Max-Planck-Gesellschaft](https://www.mpg.de/197494/rulesScientificPractice.pdf).
[^3]: Andreas Weber und Claudia Piesche: „Datenspeicherung, -kuration und Langzeitverfügbarkeit“, in: Markus Putnings, Heike Neuroth und Janna Neumann (Hrsg.): Praxishandbuch Forschungsdatenmanagement, 2021, https://doi.org/10.1515/9783110657807-019, S. 349. Siehe auch https://kost-ceco.ch/cms/warc.html.
[^4]:BMBF: „Urheberrecht in der Wissenschaft Ein Überblick für Forschung, Lehre und Bibliotheken“, 2023, https://www.bmbf.de/SharedDocs/Publikationen/de/bmbf/1/31518_Urheberrecht_in_der_Wissenschaft.pdf?__blob=publicationFile&v=6, S.  43.
[^5]:BMBF: „Urheberrecht in der Wissenschaft Ein Überblick für Forschung, Lehre und Bibliotheken“, 2023, https://www.bmbf.de/SharedDocs/Publikationen/de/bmbf/1/31518_Urheberrecht_in_der_Wissenschaft.pdf?__blob=publicationFile&v=6, S. 33. Auch das Datenbankherrstellerrecht [UrhG § 87 Abs. 2](https://www.gesetze-im-internet.de/urhg/__87a.html) ist noch eine Option. Jedoch greift dieses Recht zum Schutz von Investitionen in Datenbank in wissenschaftlichen Kontexten wahrscheinlich selten.
[^6]:Matthias Bäcker und Sebastian Golla: Handreichung Datenschutz, hg. vom Rat für Sozial- und Wirtschaftsdaten, RatSWD Output 8 (6), 2. vollständig überarbeitete Auflage, Berlin 2020, https://doi.org/10.17620/02671.50, S. 31.
[^7]: https://www.loc.gov/preservation/digital/formats/intro/format_eval_rel.shtml#factors
[^8]:Donig, S., Eckl, M., Gassner, S., & Rehbein, M. (2023). Web archive analytics: Blind spots and silences in distant readings of the archived web. Digital Scholarship in the Humanities, 1-16. https://doi.org/10.1093/llc/fqad014.
[^9]:The American Historical Review, Volume 108, Issue 3, June 2003, Pages 735–762, https://doi.org/10.1086/ahr/108.3.735.
[^10]: Richtlinie 2016/2102 des Europäischen Parlaments und des Rates vom 26. Oktober 2016 über den barrierefreien Zugang zu den Websites und mobilen Anwendungen öffentlicher Stellen, https://eur-lex.europa.eu/legal-content/DE/TXT/PDF/?uri=CELEX:32016L2102.
[^11]: Verordnung zur Schaffung barrierefreier Informationstechnik nach dem Behindertengleichstellungsgesetz (Barrierefreie-Informationstechnik-Verordnung -- BITV 2.0), https://www.gesetze-im-internet.de/bitv_2_0/BJNR184300011.html. Die Verordnung BITV 2.0 enthält in § 2 (2.2) eine Ausnahmeregelung für "*Archive, die weder Inhalte enthalten, die für aktive Verwaltungsverfahren benötigt werden, noch nach dem 23. September 2019 aktualisiert oder überarbeitet wurden*".
[^12]: Ein anschauliches Beispiel für das Konzept einer Sitemap wird gegeben in dem Artikel Rockwell, G., Day, S., Yu, J., Engel, M.: Burying Dead Projects: Depositing the Globalization Compendium. In: Digital Humanities Quarterly, Vol. 8 Number 2, 2014, http://digitalhumanities.org
[^13]: Bitte beachten Sie, dass dieser Text keine rechtliche Beratung darstellt sondern nur über die Thematik informiert, ohne abschließende Gewissheit zu vermitteln. Für eine rechtliche Beratung wenden Sie sich bitte an Ihre jeweilige Rechtsabteilung.
