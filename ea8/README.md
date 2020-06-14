# ML Introduction Exercise

1. Read the Pedro Domingos article mentioned in the ML Introduction exercise at the end thoroughly and answer all the questions there.

## What is the meaning of generalization in the paper

Machine Learning kann der Problemlösung mehrerer Bereiche dienen (anders als Algorithmen, die sich um ein einzelnes kümmern).
Daher ist es sinnvoll und wichtig, dass Daten über einen Trainingssatz hinaus verallgemeinert – also generalisiert – werden. Anfänger testen laut Domingos
häufig die Trainingsdaten, was aber oft nicht besser als zufälliges Erraten sei. Es empfiehlt sich daher, einige Daten von Beginn an zu extrahieren und diese
erst am Ende an einem Classifier zu testen. Da sich die Menge der Trainigsdaten auf diese Weise reduziert, schlägt Domingos Kreuzvalidierungen vor.

Die Verallgemeinerung von Daten dient also letztendlich der Übertragbarkeit und sorgt dafür, dass Modelle auf verschiedene Probleme anwendbar sind.

## What are the many faces of overfitting

Overfitting entsteht, wenn zu wenig Daten für eine vollständige Bestimmung eines Classifiers zur Verfügung stehen. Dadurch
können Classifier zu sehr an Trainingsdaten gebunden werden, wodurch sie im Trainig zwar sehr gut abschneiden, aber in den Testdaten dann versagen.
Dies entsteht zum Beispiel, wenn Generalisierungsfehler in Verzerrung und Varianz vorliegen.

## Why do humans have problems in higher dimensions

Menschen haben im Allgemeinen ein gutes Verständnis von zwei und drei Dimensionen im Raum. Die Regeln, die dort gelten, können aber nicht immer auf
n-dimensionale Räume übertragen werden. In N Dimensionen zu Denken, fällt dem Menschen schwer, weil es an Vorstellungskraft und Verständnis mangelt.
Bei 100 Dimensionen und einem Trainingssatz von Billionen Beispielen würde letzteres zum Beispiel nur einen Bruchteil von etwa 10 bis 18 des Input Spaces abgedeckten werden.

## What is feature engineering

Beim Feature Engineering geht es darum herauszufinden, welche Subsets ein Classifier benötigt um die besten Resultate zu erzielen.

## Why does more data beats clever algorithms

Mit vielen Daten werden die Classifier genauer, da sich sowohl relevante als auch irrelavante Merkmale herauskristallisieren. Zudem ist es deutlich einfacher
mehr Daten zu erheben als einen Algorithmus zu verbessern.

## What is ensemble learning

Beim Ensemble Learning werden mehrere Lernalgorithmen zusammengeführt um bessere Resultate zu erzielen.

## What is accuracy in data science

Das ist die Wahrscheinlichkeit mit der ein Datenset richtig klassifiziert wird.
