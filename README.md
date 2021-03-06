# bechdelsdrama

Vorläufige Version 1:

                                              Dramatische Werke im Bechdel-Test.
                                Ein Ansatz für eine Methode der automatisierten Genderanalyse. 

1 Der Bechdel-Test

  1985 etabliert Alison Bechdel in der Comicserie „Dykes to watch out for“ einen Test, der über 30 Jahre später zum popkulturell-feministischen Phänomen für FilmkritikerInnen wurde. In seiner bestechlichen Einfachheit, gilt der Test als bestanden, wenn ein Film drei Fragen positiv beantwortet:
  •	Gibt es mindestens zwei Frauenrollen, die namentlich erwähnt werden?
  •	Sprechen diese miteinander?
  •	Reden die Frauen miteinander über etwas anderes als Männer?

Neben all der berechtigten, auf wissenschaftlich-qualitative Mängel bezogenen Kritik, gibt der Bechdel-Test trotzdem Aufschluss über ein Geschlechter-Missverhältnis, dessen Betrachtung auch für die Dramenanalyse interessant ist. Die Adaptierung des für Filme konzipierten Tests auf Dramen ist zulässig, da der Bechdel-Test auf etwas verweist, das bereits sehr früh im kreativen Prozess entsteht: die Handlung und die Figurenentwicklung.

Mithilfe von digitalen Methoden ist es möglich, große Datenmengen schnell und einfach zu verarbeiten. Dramen eignen sich in besonderer Weise dafür, da eine eindeutige Zuordnung von Redebeiträgen erfolgt. Der XML-basierte TEI-Standard ermöglicht es folgerichtig, Metainformationen und Tags in die Verarbeitung einzubinden.

Für die Dramenanalyse ergeben sich dadurch eine Vielzahl an Möglichkeiten. Mithilfe von einfachen Befehlen ist etwa die Ausweisung einzelner Figuren-Aktivitäten, wie die Anzahl der Verse und Wörter verfügbar. Entsprechend aufbereitete Daten geben Information preis, die ohne digitale Methoden nur sehr schwer herauszuarbeiten sind. Quantitative Analysen und Vergleiche werden dadurch in großem Umfang möglich.

Beim Gender-Aspekt betritt dieses Projekt überraschenderweise Neuland. Zwar lässt sich konstatieren, dass Tools der Digital Humanities für gender-bezogene Analysen sehr wohl zur Verfügung stehen, das aber eher der meist breiten Ausrichtung dieser Analyse-Tools geschuldet ist. Mit der Festlegung auf den Bechdel-Test als Ausgangspunkt der Analyse-Ambitionen ist dieses Projekt durchaus an die Grenzen der digitalen Möglichkeiten gekommen, da auf ein „close reading“ nicht verzichtet werden kann, wie die Dokumentation in Punkt 3 zeigt.


3.1. Festlegung der Forschungsparameter

3.1.1. Dramenauswahl

Um ein möglichst breit gefächertes Resultat zu erzielen, hat sich unser Projektteam darauf geeinigt, verschiedenste, willkürlich ausgewählte Dramen über die Epoche der Wiener Moderne hinaus zu untersuchen. Einzige Bedingung war das Vorhandensein weiblicher Figuren, um ein Scheitern des Testes bereits im Vorfeld ausschließen zu können.

3.1.2. Verwendete Programme und Ressourcen

[Screenshot SEQ ARABIC 1]

Verwendet werden im Folgenden die bereits digitalisierten Dramen aus dem Korpus von Gerdracor (der Kurzform für „German Drama Corpus“), welcher auf der Software-Entwicklungsplattform GitHub zur freien Verfügung bereitgestellt wird. Zur Nutzung Dramen haben wir im Rahmen unserer Forschung xPath-Suchen mithilfe des Oxygen-XML-Editors durchgeführt. 

  3.3. Dokumentation der Abfragen

Grabbe Napoleon:
Öffnen der xml-Datei des digitalisierten Dramas im Oxygen-XML-Editor, Doppelklick für Anzeige. Im Drama wurden bereits alle Rollennamen hinsichtlich ihres [sex] getagt.

[Screenshot SEQ ARABIC 2]

Frage 1:
Mit dem Befehl count(//person[@sex="FEMALE"]) Suche nach der Anzahl der weiblichen Figuren, das Ergebnis lautet 23, womit die erste Frage des Tests bereits positiv beantwortet ist. Die 23 weiblichen Rollennamen sind "die_stuhlvermieterin", "eine_alte_putzhaendlerin", "madame_de_serre", "die_amme", "herzogin_von_angouleme", "die_nichte", "die_damen_der_halle", "eine_dame_der_halle_2-1", "eine_andere_dame_der_halle_2-1", "louise", "graefin_von_choisy", "frau_des_schneidermeisters", "eine_dame_der_halle_3-1a", "eine_dame_der_halle_3-1b", "ein_aeltliches_frauenzimmer", "weiber", "goettin_der_vernunft", "frau_des_kraemers", "hortense", "eine_dame", "marketenderin", "adeline" und "herzogin_von_chimay".

Frage 2:

[Screenshot SEQ ARABIC 3]

Der Befehl //sp[@who="#Rollenname"] dient zur Filterung der Dialogszenen, um hintereinander sprechende weibliche Figuren ausfindig zu machen, unter der Annahme, dass dies ein Gespräch zwischen den Beiden bedeutet.
Treffer, da "madame_de_serre" und "die_amme" hintereinander Dialog besitzen und somit ein Gespräch miteinander führen. Die zweite Frage des Tests ist damit bestanden. 

[Screenshot SWQ ARABIC 4]

Frage 3: 
Das Nachlesen der gefunden Szene ergibt, dass es in allen Gesprächen der "madame_de_serre" um einen Mann geht, womit die dritte Frage mit Nein beantwortet werden muss.

3.4. Ergebnisse 

[Tabelle]

3.5. Voyant Tool 
Um die ermittelten Szenen, in welchen sich zwei Frauen unterhalten, auch graphisch darzustellen, um diese dann zu vergleichen, kann man das Voyant Tool verwenden. Die Homepage ermöglicht es Szenen in einer Wortwolke darzustellen. Es werden nach Eingabe der Szene die darin vorkommenden Wörter graphisch dargestellt. Die Wörter, welche am häufigsten fallen, werden groß hervorgehoben, wohingegen die weniger verwendeten Wörter klein ausfallen.
Für unsere Arbeit ist dies eine interessante Möglichkeit um die Fragen zwei und drei zu analysieren, da man in einem Bild die zentralen Themen des Gesprächs erkennen kann. 
Im folgenden Beispiel haben wir jeweils eine Szene der Werke Dantons Tod und Frühlings Erwachen gewählt in welcher sich zwei Frauen unterhalten.

In Dantons Tod wurde die Szene eingegeben, in welcher sich Camille und Lucile miteinander unterhalten und das Gesprächsthema sich über Danton handelt. 
Im Gegensatz zu dieser Szene wählten wir bei Frühlings Erwachen eine Szene, in welcher sich Wendla und Frau Bergmann nicht über Männer unterhalten. 
Die visuelle Darstellung der Szenen sieht wie folgt aus:

[WORDCLOUD 1]
[WORDCLOUD 2]

Wie man nun an der grafischen Darstellung sehen kann, erscheint bei der Szene aus Dantons Tod das Wort „scheiden“ sehr groß, was bedeutet, dass es häufig vorkommt. Da die Scheidung, in der Zeit der Entstehung des Werkes, immer einen Mann und eine Frau betraf, kann man bei der Betrachtung der Wortwolke schon erahnen, dass sich das Gespräch um einen Mann dreht. 
Wedekinds Frühlings Erwachen   hingegen beinhaltet keine Wörter, die beim ersten Betrachten darauf schließen lassen, dass das Gespräch von einem Mann handelt. Wörter wie „Mutter“ oder „Prinzeßkleidchen“ sind eindeutig nicht mit Männern in Verbindung zu setzen.
Eindeutige Ergebnisse liefert diese Tool zwar nicht, jedoch kann es für einen ersten Interpretationsanatz beziehungsweise zum visuellen Vergleichen der ausgewählten Szenen hilfreich sein.  


