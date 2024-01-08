To display the given text as editable code in Markdown for GitHub, we should use code blocks. In Markdown, code blocks are created using triple backticks (` ``` `) before and after the code. Here's how your text would be converted into Markdown format with code blocks:


## Spaß mit Datenbanken
### SQL
### Structured Query Language

#### Entwicklung
The paper, “A Relational Model of Data for large Shared Data Banks,” by Dr. E. F.
Codd, was published in June 1970 in the Association of Computer Machinery (ACM) journal.
Codd’s model is now accepted as the definitive model for relational database management
systems (RDBMS).

ca. 1975 - SEQUEL = **S**tructured English **Q**uery **L**anguage, Vorläufer von SQL wird für
das Projekt System R von IBM 

1979 - **SQL** gelangt mit **Oracle V2** erstmals durch **Relational Software Inc**.
auf den Markt.

1986 - **SQL1** wird von ANSI als Standard verabschiedet.

1987 - **SQL1** wird  auch von ISO als Standard verabschiedet und 1989
nochmals überarbeitet.

1992 - Der Standard **SQL2** bzw. **SQL-92** wird von der ISO verabschiedet. 

1999 - **SQL3** bzw. **SQL:1999** wird verabschiedet. 

2003 - **SQL:2003** wird von der ISO als Nachfolger des SQL:1999
Standards verabschiedet. 

2006 - SQL:2006 ISO/IEC 9075-14:2006 legt fest, wie SQL in Zusammenhang mit
XML verwendet werden kann. 

2008 - SQL:2008 ISO/IEC 9075

2011 - SQL:2011 ISO/IEC 9075:2011 ist die aktuelle Revision des SQL
Standards

#### Benefits of SQL
The strengths of SQL benefit all ranges of users including application programmers, database administrators, management and end users.

SQL is a non–procedural language because it:
* processes sets of records rather than just one at a time
* provides automatic navigation to the data

SQL provides commands for a variety of tasks including:
* querying data
* inserting, updating, and deleting rows in a table
* creating, replacing, altering, and dropping objects
* controlling access to the database and its objects
* guaranteeing database consistency and integrity

SQL unifies all of the above tasks in one consistent language

#### SQL Generation 4
Gesucht ist der Vorname und der Familienname aller Kunden, die in '4040' wohnen.


3.Generation                      4. Generation
Öffne die Kundendatei             SELECT VORNAME, ZUNAME
Lies den ersten Satz              FROM KUNDE
Solange die Datei nicht leer      WHERE PLZ = '4040'
mache folgendes
  wenn plz = '4040'
    gib Vorname und Zuname aus
  lies den nächsten Satz
Schliesse die Kundendatei


#### Subsprache

##### Data Definition Language  (DDL)
dient zur Implementierung des relationalen Modells  in einer Datenbank. Definition von Tabellen, deren Attribute, Typen und Wertebereiche
Beispiel Pseudocode:


erstelle Tabelle kunde mit den Feldern 
kundennummer ganzzahlig, 
vorname zeichenkette


* CREATE - definieren
* ALTER  - ändern
* DROP - löschen

##### Data Manipulation Language (DML)
dient zur Manipulation von Daten:
Abfrage, Ändern, Einfügen, Löschen.

* SELECT - auswählen
* UPDATE - aktualisieren
* INSERT - einfügen
* DELETE - löschen

##### Data Control Language (DCL)
regelt den Zugriff und die Berechtigungen insbesondere in Mehrbenutzersystemen.

* GRANT  - Berechtigungsvergabe
* REVOKE - Berechtigungsentzug
* COMMIT - fixieren von Veränderungen
* ROLLBACK - Zurücksetzen
* LOCK   - sperren 

#### Relationale Algebra

Die Grundlagen der Relationalen Datenbanken liegen in den Arbeiten von Edgar F. Codd aus den 60er und 70er Jahren. 

Er entwickelte ein algebraisches Modell (eine Algebra befasst sich mit den Eigenschaften von Rechenoperationen), das sich damit befasst, wie Daten gespeichert, abgefragt und manipuliert werden können.

Die Operationen basieren auf Relationen, den
