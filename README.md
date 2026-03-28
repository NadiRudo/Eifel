# Löschwasserversorgung bei Waldbränden – Eine GIS-gestützte Analyse der Löschwasserabdeckung in der Eifel

## Einleitung

Waldbrände stellen weltweit eine zunehmende Herausforderung für Ökosysteme, Infrastruktur und Katastrophenschutz dar. Während großflächige Vegetationsbrände lange Zeit vor allem mit Regionen wie Südeuropa, Australien oder Nordamerika in Verbindung gebracht wurden, zeigen Entwicklungen der letzten Jahrzehnte, dass auch Mitteleuropa stärker von dieser Problematik betroffen ist. Besonders Deutschland erlebt aufgrund klimatischer Veränderungen zunehmend längere Hitzeperioden und ausgeprägte Trockenphasen, die das Risiko von Wald- und Vegetationsbränden deutlich erhöhen (Marx et al. 2024).

Die Hitzewellen der Jahre 2003, 2018 und 2019 zählen zu den stärksten jemals in Mitteleuropa gemessenen Hitzeperioden (Gnilke et al. 2021). Diese extremen Wetterlagen führen dazu, dass Vegetation austrocknet und somit leichter entzündbar wird. Gleichzeitig kann sich Feuer unter diesen Bedingungen schneller und auf größeren Flächen ausbreiten.

Statistiken zeigen, dass Waldbrände auch in Deutschland ein relevantes Risiko darstellen. Zwischen 2020 und 2022 wurden deutschlandweit mehr als 22.000 Waldbrände registriert, die zusammen eine Fläche von über 15.000 Hektar zerstörten (Gnilke et al. 2024). Gleichzeitig hat sich laut Studien die Anzahl der Tage mit hoher Waldbrandgefahr seit 1990 im Vergleich zum langjährigen Mittel der Jahre 1961 bis 1990 etwa verdoppelt (ebd.).
Die Entstehung von Waldbränden wird grundsätzlich durch das Zusammenspiel von drei Faktoren bestimmt: verfügbares Brennmaterial, geeignete Wetterbedingungen und eine Zündquelle (Pyne et al. 1996). In Deutschland ist dabei menschliches Fehlverhalten die häufigste Ursache für Brände, beispielsweise durch unachtsam weggeworfene Zigaretten, offene Feuerstellen oder technische Defekte (Marx et al. 2024).

Vor diesem Hintergrund wird die effektive Brandbekämpfung in Waldgebieten immer wichtiger. Eine zentrale Voraussetzung dafür ist eine zuverlässige Versorgung mit Löschwasser.

## Herausforderungen der Löschwasserversorgung in Waldgebieten

Im Gegensatz zu urbanen Räumen verfügen Waldgebiete in der Regel über keine direkte Anbindung an ein flächendeckendes Hydrantennetz (Hoch, 2019). In Städten kann Löschwasser meist unmittelbar aus dem Trinkwassernetz entnommen werden. In abgelegenen Waldregionen ist dies jedoch nicht möglich.

Stattdessen müssen Feuerwehren häufig auf eine unabhängige Löschwasserversorgung zurückgreifen. Dazu zählen insbesondere Bäche, Flüsse, Seen und Teiche (Hoch, 2019). Diese offenen Gewässer dienen als Wasserentnahmestellen. Von dort aus wird Wasser mithilfe mobiler Pumpen, wie der Tragkraftspritze (siehe Abb. 1), über Schläuche (siehe Abb. 2) zur Brandstelle transportiert. Die Tragkraftspritze hat ein Gewicht von ca. 200 kg und kann daher nur von 4 Personen getragen werden. Auch die Uniform der Feuerwehr hat ein Gewicht, weshalb die Bewegungen und die Überwindung von Distanzen stark eingeschränlt sind.

<p align="center">
  <img src="https://www.feuerwehr-pastetten.de/wp-content/uploads/2012/12/ts8.jpg" width="300"><br>
  <sub>Abbildung 1: Tragkraftspritze (Quelle: Freiwillige Feuerwehr Pastetten)</sub>
</p>

<p align="center">
  <img src="https://feuerwehrfischen.com/wp-content/uploads/2019/12/schlauch3.jpg?w=2048" width="300"><br>
  <sub>Abbildung 2: Aufbewahrung der Feuerwehrschläuche (Quelle: Freiwillige Feuerwehr Fischen im Allgäu)</sub>
</p>

In der Praxis bringt dieses Vorgehen mehrere Herausforderungen mit sich. Zum einen müssen geeignete Wasserentnahmestellen zunächst erreichbar sein. Feuerwehrkräfte müssen ihre Ausrüstung häufig über Waldwege transportieren und können sich nur begrenzt durch unwegsames Gelände bewegen. Zudem müssen Pumpen auf ausreichend stabilem Untergrund aufgebaut werden, damit sie zuverlässig arbeiten. Ein weiteres Problem ist der Druckverlust beim Transport von Wasser über längere Distanzen. In Feuerwehrschläuchen sinkt der Wasserdruck kontinuierlich mit zunehmender Entfernung. Wird eine bestimmte Distanz überschritten, reicht der Druck nicht mehr aus, um das Wasser effektiv zur Brandbekämpfung einzusetzen. In solchen Fällen müssen zusätzliche Pumpen eingesetzt werden.

## Wassertransport über lange Distanzen

Bei größeren Waldbränden wird häufig ein sogenannter Pumpenförderbetrieb eingerichtet. Dabei handelt es sich um ein System aus mehreren hintereinander geschalteten Pumpen.

Der Ablauf funktioniert vereinfacht folgendermaßen:
1.	Eine erste Pumpe entnimmt Wasser aus einem Gewässer.
2.	Das Wasser wird über eine bestimmte Strecke durch Schläuche transportiert.
3.	An einem geeigneten Punkt wird eine weitere Pumpe installiert.
4.	Diese erhöht erneut den Druck und pumpt das Wasser weiter in Richtung Brandstelle.

Dieses Verfahren kann theoretisch beliebig erweitert werden, indem weitere Zwischenpumpen aufgebaut werden. In der Praxis ist dies jedoch mit erheblichem personellen und logistischen Aufwand verbunden. Jede zusätzliche Pumpe benötigt Personal, Ausrüstung sowie Zeit für Aufbau und Inbetriebnahme.

## Zielsetzung der Untersuchung

Das Ziel des Projekts bestand darin, mithilfe von Geodaten zu analysieren, wie groß die potenziell erreichbare Fläche für Löschwasser in einem Waldgebiet der Eifel (siehe Abb. 3) ist.

<p align="center">
  <img src="Karten/Übersichtskarte.png" width="700"><br>
  <em>Abbildung 3: Standort Nationalpark Eifel (Quelle: Eigene Darstellung)</em>
</p>

Dabei standen zwei zentrale Fragen im Fokus:
1.	Welche Wasserentnahmestellen können erreicht werden und entsprechen aufgrund ihrer Neigung den Voraussetzungen, damit sie genutzt werden können?
2.	Wie weit kann Wasser von diesen Punkten aus transportiert werden, bevor der Druckverlust eine weitere Versorgung verhindert?

Die Analyse sollte außerdem untersuchen, wie sich der Einsatz zusätzlicher Pumpen auf die erreichbare Fläche auswirkt.

Als Untersuchungsgebiet wurde der Nationalpark Eifel gewählt. Die Region ist geprägt von ausgedehnten Waldflächen, teilweise steilem Gelände sowie zahlreichen kleineren Gewässern. Gleichzeitig existiert dort nur eine begrenzte Anzahl an fest installierten Löschwasserstellen.

## Datengrundlage und konzeptioneller Ansatz

Für die Analyse wurden verschiedene Geodaten kombiniert. Ausgangsdaten waren ein digitales Geländemodel mit einer Auflösung von 1 m vom Geoportal.NRW, sowie Straßen, Wanderwege und Gewässerdaten aus dem QuickOSM Plugin von QGIS. Die Software QGIS Version 3.36.3 wurde für den Großteil der Analyse genutzt, für einzelne Schritte wurde auf GRASS GIS Version 8.4.1 zurückgegriffen. 

Zunächst wurden potenzielle Wasserentnahmestellen entlang der vorhandenen Gewässer identifiziert. Da Feuerwehrkräfte ihre Ausrüstung in der Regel nicht weit durch dichtes Gelände tragen können, wurden nur Gewässer berücksichtigt, die sich in einer Entfernung von 100 m zu den Wegen befinden. Gleichzeitig wurde eine weitere Einschränkung berücksichtigt, denn die Tragkraftspritze, welche für die Analyse beispielhaft als Pumpe der Feuerwehr ausgewählt wurde, kann nur bis zu einer Hangneigung von 15° zuverlässig arbeiten. Identifizierte Wasserentnahmestellen an steileren Hängen als 15° wurden ausgeschlossen.

Anschließend wurde untersucht, wie weit das Wasser von diesen Punkten aus transportiert werden kann. Als Ausgangsdruck der Pumpe wurden 10 bar angenommen. Durch den Transport durch Feuerwehrschläuche geht kontinuierlich Druck verloren. Für die Schläuche wurden C-Schläuche der Feuerwehr angenommen, die einen Druckverlust von 0,013 bar pro Meter haben. Zudem verliert der Wasserdruck durch den Transport 0,1 bar pro Höhenmeter. Die Berechnungen des Wasserdrucks wurde in einem Kostenraster dargestellt, welches pro m² die „Kosten“ des Druckverlusts beinhaltet. Da die Tragkraftspritze einen begrenzten Ausgangsdruck von 10 bar erzeugen kann und am Ende eine Mindestmenge von 5 bar benötigt wird, ergibt sich eine maximale Distanz für den Wassertransport (siehe Abb. 1). Mit dem Kostenraster wurde anschließend von den Wasserentnahmestellen eine Pfadanalyse mit dem Tool r.cost der GRASS GIS Toolbox durchgeführt. Damit wird die Fläche ausgegeben, die von den Wasserentnahmestellen aus, ins Gelände mit Berücksichtigung der Neigung und den Kostenobergrenze, erreicht werden kann.

Nach dieser ersten Analyse wurde ein zweites Szenario betrachtet, bei dem eine zusätzliche Zwischenpumpe eingesetzt wird. Dadurch kann Wasser über eine größere Entfernung weitergeleitet werden, bevor der Druck erneut zu stark abfällt. Hier wurde eine weitere Restriktion berücksichtigt. Die Feuerwehr kann eine Neigung über 40° nicht überwinden und daher auch nicht die Schläuche oder die zweiten Pumpe bei dieser starken Neigung installieren. Darüber hinaus ist der Druckverlust durch die Höhenmeter zu groß. Daher wurde ein zweites Kostenraster erstellt. Es beinhaltet dieselbe Berechnung wie das erste Kostenraster und enthält außerdem die Restriktion, dass alle m² ausgeschlossen werden, die eine stärkere Neigung als 40° aufweisen, da diese Flächen nicht erreichbar und für die Löschaktion nutzbar sind. Für den Standort der zweiten Pumpe wurde der Rand der Fläche, die mit der ersten Pumpe erreicht werden kann, genutzt (siehe Abb. 3). 

<p align="center">
  <img src="Karten/Nahansicht%20der%20FLächenabdeckung%20und%20Pumpstandorte.png" width="700"><br>
  <em>Abbildung 4: Erreichbarkeiten nach Wasserdruck bei 10 bar Ausgangsdruck nach den Wasserentnahmestellen und der zweiten Pumpe (Quelle: Eigene Darstellung)</em>
</p>

Es ist zu erwähnen, dass die Methodik eine Limitation beinhaltet. Von den identifizierten Wasserentnahmestellen wurden die Erreichbarkeitsanalyse begonnen, jedoch wurde die Richtung nicht angegeben, sodass auch auf der anderen Seite des Gewässers, eine Fläche als „abgedeckt“ angezeigt wird. Diese Vorgehensweise ist in der Praxis nicht immer anwendbar, da tiefere und größere Gewässer nicht gekreuzt werden können und somit die Fläche am anderen Ufer nicht erreichbar ist. Dies muss bei der Betrachtung der nachfolgenden Ergebnisse beachtet werden. 

## Ergebnisse

Die Analyse zeigt deutlich, dass die Löschwasserversorgung in großen Waldgebieten stark eingeschränkt sein kann (siehe Abb. 4).

<p align="center">
  <img src="Karten/Löschabdeckung.png" width="700"><br>
  <em>Abbildung 4: Abbildung 5: Erreichbare Fläche nach den Wasserenahmestellen und der zweiten Pumpe (Quelle: Eigene Darstellung)</em>
</p>

Im untersuchten Gebiet ergeben sich folgende Ergebnisse:
- Mit dem Einsatz von zwei Pumpen (einer Wasserentnahme und einer Zwischenpumpe) kann eine Fläche von etwa 3,58 km² erreicht werden.
- Die erste Pumpe kann eine Fläche von 1,71 km² erreichen.
- Daran anschließend kann mit der zweiten Pumpe eine Fläche von 1,87 km² abgedeckt werden.

Die Gesamtfläche des untersuchten Nationalparks beträgt 10,87 km². Damit können mit diesem Aufbau nur etwa 32 Prozent der gesamten Fläche direkt mit Löschwasser versorgt werden.

Große Teile des Parks liegen also außerhalb der Reichweite dieses Systems. Diese Bereiche befinden sich entweder zu weit von geeigneten Gewässern entfernt oder sind aufgrund der Geländestruktur schwer zugänglich. Dennoch kann die Untersuchung, wie oben erwähnt, weitergeführt werden und weitere Zwischenpumpen eingesetzt werden, um die erreichbare Fläche zu erweitern.

## Diskussion

Die Ergebnisse verdeutlichen, wie stark die Effektivität der Brandbekämpfung in Waldgebieten von natürlichen Gegebenheiten abhängig ist. Dabei beeinflussen mehrere Faktoren, wie die Entfernung zur Wasserquelle, die Geländestruktur, die Zugänglichkeit über Wege und das Equipment der Feuerwehr die erreichbare Fläche.

Insbesondere in großen, zusammenhängenden Waldgebieten kann die Wasserversorgung daher schnell zu einem limitierenden Faktor werden. In solchen Fällen müssen alternative Strategien eingesetzt werden, etwa der Transport von Wasser durch Tanklöschfahrzeuge oder der Einsatz von Löschhubschraubern. Gleichzeitig zeigen die Ergebnisse, dass eine gezielte Planung von Wasserentnahmestellen eine wichtige Rolle spielen kann. Zusätzliche Löschwasserteiche oder zugängliche Gewässerstellen könnten die Reichweite der Brandbekämpfung deutlich erhöhen.

Ein weiteres Problem besteht darin, dass Informationen über erreichbare Wasserquellen häufig nicht aktuell sind. Veränderungen in der Landschaft, versperrte Wege oder ausgetrocknete Gewässer können dazu führen, dass zuvor nutzbare Wasserentnahmestellen im Ernstfall nicht mehr verfügbar sind. Hier bieten Geoinformationssysteme ein großes Potenzial. Sie ermöglichen es, räumliche Daten zu analysieren, potenzielle Versorgungslücken zu identifizieren und Planungen zu unterstützen.

## Fazit

Die zunehmende Waldbrandgefahr in Deutschland macht eine effektive Planung der Löschwasserversorgung immer wichtiger. Besonders in abgelegenen Waldregionen stellt die Verfügbarkeit von Wasser eine zentrale Herausforderung für Feuerwehren dar.

Die vorliegende Analyse zeigt, dass selbst mit dem Einsatz mehrerer Pumpen nur ein begrenzter Teil eines großen Waldgebiets effektiv erreicht werden kann. Im untersuchten Gebiet der Eifel konnten mit zwei Pumpen lediglich etwa ein Drittel der Gesamtfläche potenziell mit Löschwasser versorgt werden. Diese Ergebnisse verdeutlichen die Bedeutung einer strategischen Planung von Wasserentnahmestellen sowie einer kontinuierlichen Aktualisierung entsprechender Geodaten. GIS-basierte Analysen können dabei helfen, kritische Bereiche zu identifizieren und die Einsatzplanung von Feuerwehren zu verbessern.

Angesichts zunehmender Trockenperioden und steigender Temperaturen wird die Bedeutung solcher Analysen in Zukunft weiter zunehmen. Eine frühzeitige räumliche Planung kann einen wichtigen Beitrag leisten, um Waldbrände effektiver zu bekämpfen und Schäden an Ökosystemen und Infrastruktur zu minimieren.

## Quellen

- Gnilke, A., & Sanders, T. (2021). Waldbrandhistorie in Deutschland (2001-2020). Project brief, 32.
- Gnilke, A., & Sanders, T. G. M. (2024). Waldbrände in Deutschland und die besondere Gefahrenlage in Brandenburg. In J. L. Lozán, H. Graßl, D. Kasang, M. Quante, & J. Sillmann (eds.), Warnsignal Klima: Herausforderung Wetterextreme: Ursachen - Auswirkungen - Handlungsoptionen (pp. 218–223). Wissenschaftliche Auswertungen. https://doi.org/10.25592/warnsignal.klima.wetterextreme.37.
- Hoch, W. (2019). Löschwasserversorgung. In: Mutschmann/Stimmelmayr Taschenbuch der Wasserversorgung. Springer Vieweg, Wiesbaden. https://doi.org/10.1007/978-3-658-23222-1_9
- Marx, A., Blauhut, V., Boeing, F., Forkel, M., Hagenlocher, M., Herbst, M., Hoffmann, P., Kuhlicke, C., Kumar, R., Madruga de Brito, M., Samaniego, L., Thonicke, K. & Ziese, M. (2023). Dürren und Waldbrände unter Klimawandel. Klimawandel in Deutschland, 131.
- Pyne SJ, Andrews PL, Laven RD (1996) Introduction to wildland fire, 2. Aufl. Wiley, New York, S. 769.

## Abbildungen

- Abbildung 1: Freiwillige Feuerwehr Pastetten (o.J.). Tragkraftspritze URL: https://www.feuerwehr-pastetten.de/tragkraftspritze/
- Abbildung 2: Freiwillige Feuerwehr Frischen im Allgäu (o.J.). Aufbewahrung der Feuerwehrschläuche URL: https://feuerwehrfischen.com/478-2/ueber-uns/unser-geratehaus/
- Abbildung 3: Rudolph, N. u. Schmitz, A. (2026). Standort Nationalpark Eifel (Quelle: Eigene Darstellung)
- Abbildung 3: Rudolph, N. u. Schmitz, A. (2026). Erreichbarkeiten nach Wasserdruck bei 10 bar Ausgangsdruck nach den Wasserentnahmestellen und der zweiten Pumpe
- Abbildung 4: Rudolph, N. u. Schmitz, A. (2026). Erreichbare Fläche nach den Wasserenahmestellen und der zweiten Pumpe 



Autoren: Alexandra Schmitz und Nadine Rudolph
