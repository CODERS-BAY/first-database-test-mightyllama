# DB-Test
## Aufgabe 1
Stelle Entitäten mittels Chen-Notation und Min,Max Notation dar.
Wähle ein sinnvolles Beispiel!
  siehe Bild
## Aufgabe 2
Kann eine Beziehung Attribute haben?
Wenn ja, wie stelle ich es im ERD dar?
  Ja. (Raute→Oval)
## Aufgabe 3
Welche Codd'schen Anforderungen gibt es (Nenne mindestens 5)
  * Integration: einheitliche, nicht redundante Datenverwaltung
  *Operationen: Speichern, Suchen, Ändern, Einfügen,
  *Katalog: Zugriffe auf Datenbeschreibungen
  *Benutzersichten: Unterschiedliche Sichten für Benutzer
  *Integritätssicherung: Korrektheit des Datenbestandes
  *Zugriffskontrolle: Ausschluss von unberechtigtem Zugriff
  *Transaktionen: Mehrere Datenbank-Operationen als Funktionseinheit
  *Synchronisation: parallele Transaktionen mehrerer Benutzer koordinieren
  *Datensicherung: Wiederherstellung von Daten nach Sytemfehlern
## Aufgabe 4
Nenne den Unterschied zwischen Konzeptuellen und Logischem Schema
  Konzeptuelles Schema: Entwurf
  Logisches Schema: Konkrete Einbindung
## Aufgabe 5
Welche 3 Bestandteile gibt es im Entity Relationship Model
  *Entity(Objekt)
  *Relationship(Beziehung)
  *Attribute(Eigenschaft)
## Aufgabe 6
Welche Datentypen gibt es in MySQL? (Nenne mindestens 5)
  *Char
  *Int
  *Date
  *Double
  *Boolean
## Aufgabe 7
Welche Arten von Schlüsseln gibt es und welche Eigenschaften besitzen diese?
  *Primärschlüssel: eindeutige Identifikation eines Datensatzes
## Aufgabe 8
Welche Arten von Beziehungen gibt es? Zeichne für jede ein Beispiel auf
  siehe Bild
## Aufgabe 9
Was bedeutet der Begriff Kardinalität und welche Kardinalitäten gibt es?
  *Genauere Beschreibung der Beziehungen von Entitäten
  *Formen: 1:1, 1:N, N:1, N:M
## Aufgabe 10
Was bedeutet der Begriff Datenintegrität und worin unterscheidet sich Integrität und referentielle Integrität?
  ?
## Aufgabe 11
Erkläre die 3 Normalformen
   1.Normalform: erlaubt nur atomare Attribute in den Beziehungsschemata(Attributwerte sind Elemente von Standard-Datentypen wie int    oder string)
  2.Normalform: Partielle Abhängigkeit liegt vor, wenn ein Attribut nur von einem Teil des Schlüssels abhängt
  3.Normalform: Eliminiert zusätzliche Abhängigkeiten
## Aufgabe 12
Erkläre den Unterschied zwischen starken und Schwachen Entitäten und erstelle ein Beispiel.
  Eine schwache Entität ist von einer anderen abhängig(zb. Raum existiert nur in Gebäude). Eine starke Entität ist nicht an eine andere gebunden.
## Aufgabe 13
Welche Grundregeln gibt es im Relationenmodell? (Nenne mindestens 4)
  *Jede Zeile ist eindeutig und beschreibt ein Objekt/Entität der Realität
  *Die Ordnung der Zeilen ist ohne Bedeutung(Reihenfolge ist egal)
  *Die Ordnung der Spalten ist ohne Bedeutung(sie müssen einen eindeutigen Namen haben)
  *Jeder Datenwert innerhalb einer Relation ist ein atomares Daten-Element
  *Es existieren Primärschlüssel
## Aufgabe 14
Wie löst man eine M:N Beziehung auf? Erstelle ein Beispiel
  ?
## Aufgabe 15
Ein Handelsbetrieb verkauft ein Sortiment von Artikeln, die er von verschiedenen Herstellern bezieht. Der Handelsbetrieb hat einen bestimmten Kundenkreis, der regelmäßig Bestellungen aufgibt. Eine Bestellung kann mehrere Artikel umfassen. Ein Artikel kann von mehreren Lieferanten bezogen werden und ein Lieferant liefert natürlich meist mehr als einen Artikel. Erstelle ein ERD und ein Relationenmodell, welches der 3. Normalform entspricht.
## Aufgabe 16
Welche Anomalien kennst du und was beschreiben sie?
  *Änderungs-Anomalie: Beim Ändern eines Wertes müssen viele andere Tupels/Zeilen ebenfalls geändert werden
  *Einfüge-Anomalie: Beim Einfügen eines Tupels können bestimmte Werte noch nicht angegeben werden, da sie noch nicht bekannt sind. Wenn Schlüsselwerte fehlen, kann der Tupel nicht eingegeben werden
  *Löschanomalie: Beim Löschen gehen mehr Werte verloren als beabsichtigt
## Aufgabe 17
Modellieren Sie den angeführten Realitätsausschnitt einer Fluggesellschaft mit Hilfe eines Entity Relationship- Diagramms. Treffen Sie, falls notwendig, sinnvolle Annahmen und dokumentieren Sie diese nachvollziehbar in Ihrer Lösung. Der zu betrachtende Realitätsausschnitt der Fluggesellschaft umfasst folgenden
Sachverhalt:
Flughäfen haben ein Kürzel (= Schlüssel) und gehören zu einer Stadt (z.B. „FRA“ für Frankfurt, „FCO“ für Roma Fiumicino).
Flüge haben eine Flugnummer (z.B. „LH 306“), führen von einem Flughafen zu einem anderen, mit jeweils einer festen Abflugs- und Ankunftszeit (z.B. ab Frankfurt um 07:30 nach Roma Fiumicino mit Ankunft um 09:15).
Jeder Flugzeugtyp hat einen Namen (z.B. „747-400“) und eine Sitzanzahl (z.B. 430 Sitze).
Piloten haben einen Namen (z.B. „Meier“), ein Geburtsdatum (z.B. „1.1.1960“) und eine Berechtigung, bestimmte Flugzeugtypen zu fliegen (z.B. „747-400“ und „A310“).
Jedes einzelne Flugzeug ist von einem bestimmten Flugzeugtyp (z.B. „747-400“) und hat einen Namen (z.B. „Mozart“).
Bei einem Flug-Einsatz wird ein Flug (z.B. „LH 306“) an einem bestimmten Datum (z.B. „6.2.2011“) von einem bestimmten Piloten (z.B. „Meier“) mit einem bestimmten Flugzeug (z.B. „Mozart“) geflogen.
Bilden Sie das konzeptuelle Schema in ein relationales Schema ab. Das relationale Schema soll der 3. Normalform genügen
