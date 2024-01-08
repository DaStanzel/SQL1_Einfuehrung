{\\rtf1\\ansi\\ansicpg1252\\cocoartf2759
\\cocoatextscaling0\\cocoaplatform0{\\fonttbl\\f0\\fswiss\\fcharset0
Helvetica;} {\\colortbl;\\red255\\green255\\blue255;}
{\\\*\\expandedcolortbl;;}
\\paperw11900\\paperh16840\\margl1440\\margr1440\\vieww11520\\viewh8400\\viewkind0
\\pard\\tx720\\tx1440\\tx2160\\tx2880\\tx3600\\tx4320\\tx5040\\tx5760\\tx6480\\tx7200\\tx7920\\tx8640\\pardirnatural\\partightenfactor0

\\f0\\fs24 \\cf0 == Spa\\'df mit Datenbanken ==\\

### SQL

\\

### Structured Query Language

\\ \\

#### Entwicklung

\\ The paper, \\'93A Relational Model of Data for large Shared Data
Banks,\\'94 by Dr. E. F.\\ Codd, was published in June 1970 in the
Association of Computer Machinery (ACM) journal.\\ Codd\\'92s model is
now accepted as the definitive model for relational database
management\\ systems (RDBMS).\\ \\ ca. 1975 - SEQUEL = **S**tructured
English **Q**uery **L**anguage, Vorl\\'e4ufer von SQL wird f\\'fcr\\ das
Projekt System R von IBM \\ \\ 1979 - **SQL** gelangt mit **Oracle V2**
erstmals durch **Relational Software Inc**.\\ auf den Markt.\\ \\ 1986 -
**SQL1** wird von ANSI als Standard verabschiedet.\\ \\ 1987 - **SQL1**
wird auch von ISO als Standard verabschiedet und 1989\\ nochmals
\\'fcberarbeitet.\\ \\ 1992 - Der Standard **SQL2** bzw. **SQL-92** wird
von der ISO verabschiedet. \\ \\ 1999 - **SQL3** bzw. **SQL:1999** wird
verabschiedet. \\ \\ 2003 - **SQL:2003** wird von der ISO als Nachfolger
des SQL:1999\\ Standards verabschiedet. \\ \\ 2006 - SQL:2006 ISO/IEC
9075-14:2006 legt fest, wie SQL in Zusammenhang mit\\ XML verwendet
werden kann. \\ \\ 2008 - SQL:2008 ISO/IEC 9075\\ \\ 2011 - SQL:2011
ISO/IEC 9075:2011 ist die aktuelle Revision des SQL\\ Standards\\ \\

#### Benefits of SQL

\\ The strengths of SQL benefit all ranges of users including
application programmers, database administrators, management and end
users.\\ \\ SQL is a non\\'96procedural language because it:\\

-   processes sets of records rather than just one at a time\\
-   provides automatic navigation to the data\\

\\ SQL provides commands for a variety of tasks including:\\

-   querying data\\
-   inserting, updating, and deleting rows in a table\\
-   creating, replacing, altering, and dropping objects\\
-   controlling access to the database and its objects\\
-   guaranteeing database consistency and integrity\\

\\ SQL unifies all of the above tasks in one consistent language\\ \\

#### SQL Generation 4

\\ Gesucht ist der Vorname und der Familienname aller Kunden, die in
'4040' wohnen.\\ \\ \\{\| class="wikitable" \\ \|-\\ ! 3.Generation\\ !
4. Generation\\ \|-\\ \|  
`\'d6ffne die Kundendatei`  
`Lies den ersten Satz`  
`Solange die Datei nicht leer mache folgendes`  
`wenn plz = '4040'`  
`gib Vorname und Zuname aus`  
`lies den n\'e4chsten Satz`  
`Schliesse die Kundendatei`  
\\ \|  
`SELECT VORNAME, ZUNAME`  
`FROM KUNDE`  
`WHERE PLZ = '4040'`  
\\ \|\\}\\ \\

#### Subsprache

\\ \\

##### Data Definition Language (DDL)

\\ dient zur Implementierung des relationalen Modells in einer
Datenbank. Definition von Tabellen, deren Attribute, Typen und
Wertebereiche\\ Beispiel Pseudocode:\\ `\`
`erstelle Tabelle kunde mit den Feldern \` `kundennummer ganzzahlig, \`
`vorname zeichenkette\`\\

-   CREATE - definieren\\
-   ALTER - \\'e4ndern\\
-   DROP - l\\'f6schen\\

\\

##### Data Manipulation Language (DML)

\\ dient zur Manipulation von Daten:\\ Abfrage, \\'c4ndern,
Einf\\'fcgen, L\\'f6schen.\\ \\

-   SELECT - ausw\\'e4hlen\\
-   UPDATE - aktualisieren\\
-   INSERT - einf\\'fcgen\\
-   DELETE - l\\'f6schen\\

\\

##### Data Control Language (DCL)

\\ regelt den Zugriff und die Berechtigungen insbesondere in
Mehrbenutzersystemen.\\ \\

-   GRANT - Berechtigungsvergabe\\
-   REVOKE - Berechtigungsentzug\\
-   COMMIT - fixieren von Ver\\'e4nderungen\\
-   ROLLBACK - Zur\\'fccksetzen\\
-   LOCK - sperren \\

\\

#### Relationale Algebra

\\ \\ Die Grundlagen der Relationalen Datenbanken liegen in den Arbeiten
von Edgar F. Codd aus den 60er und 70er Jahren. \\ \\ Er entwickelte ein
algebraisches Modell (eine Algebra befasst sich mit den Eigenschaften
von Rechenoperationen), das sich damit befasst, wie Daten gespeichert,
abgefragt und manipuliert werden k\\'f6nnen.\\ \\ Die Operationen
basieren auf Relationen, den Tabellen.\\ \\

#### Konzepte relationaler Datenbanken

\\

##### Theorie

\\ Alle zu speichernden Informationen, also auch die Beschreibung der
Datenbank selbst, werden in Form von Tabellen durchgef\\'fchrt. \\ \\
Mathematische Beschreibung der Relation:\\ Eine Relation `R` zwischen
den Mengen `A` und `B` kann durch die Elementpaare `(a, b)`
ausgedr\\'fcckt werden, f\\'fcr die `aRb` gilt. Eine Relation ist eine
Teilmenge des kartesischen Produkts `A x B`.\\ \\

##### Beispiel

\\ `S` sei die Menge aller \\'f6sterreichischen St\\'e4dte (Dom\\'e4ne
`S`) (Wien, Linz, Eisenstadt, Bregenz, \\'85)\\ \\ `F` sei die Menge
aller \\'f6sterreichischen Fl\\'fcsse (Dom\\'e4ne `F`) (Mur, Donau, Inn,
\\'85)\\ \\ `R` sei die Relation `liegt am / liegt an der`\\ \\ Eine
Relation \\'fcber den beiden Dom\\'e4nen ist definiert als eine
Teilmenge des kartesischen Produktes:\\ `s liegt am / an der f`\\ \\

#### Relation und Tupel

\\ Ein Tupel (Zeile) ist ein Element einer Relation\\ \\ Ein Telefonbuch
ist Beispiel f\\'fcr eine Relation. Ein Tupel besteht aus den
Komponenten (Attributen) `Name, Stra\'dfe und Telefonnummer`.\\ \\ Das
Tupel f\\'fcr die `CODERS.BAY` hat die Attributsauspr\\'e4gungen
`Peter Behrens Platz 6 und 073269227070`\\ \\

#### Operationen der relationalen Algebra

\\

-   Projektion\\
-   Selektion\\
-   Kartesisches Produkt\\
-   Umbenennung\\
-   Vereinigung\\
-   Differenz\\

\\

#### Beispieltabellen

\\

##### DEPT

\\ \\{\| class="wikitable" \\ \|- style="font-weight:bold;"\\ ! DEPTNO\\
! DNAME\\ ! LOC\\ \|-\\ \| 10\\ \| ACCOUNTING\\ \| NEW YORK\\ \|-\\ \|
20\\ \| RESEARCH\\ \| DALLAS\\ \|-\\ \| 30\\ \| SALES\\ \| CHICAGO\\
\|-\\ \| 40\\ \| OPERATIONS\\ \| BOSTON\\ \|\\}\\ \\

##### EMP

\\ \\{\| class="wikitable" \\ \|- style="font-weight:bold;"\\ ! EMPNO\\
! ENAME\\ ! JOB\\ ! MGR\\ ! HIREDATE\\ ! SAL\\ ! COMM\\ ! DEPTNO\\ \|-\\
\| 7369\\ \| SMITH\\ \| CLERK\\ \| 7902\\ \| 17-DEC-80\\ \| 800\\ \| \\
\| 20\\ \|-\\ \| 7499\\ \| ALLEN\\ \| SALESMAN\\ \| 7698\\ \|
20-FEB-81\\ \| 1600\\ \| 300\\ \| 30\\ \|-\\ \| 7521\\ \| WARD\\ \|
SALESMAN\\ \| 7698\\ \| 22-FEB-81\\ \| 1250\\ \| 500\\ \| 30\\ \|-\\ \|
7566\\ \| JONES\\ \| MANAGER\\ \| 7839\\ \| 02-APR-81\\ \| 2975\\ \| \\
\| 20\\ \|-\\ \| 7654\\ \| MARTIN\\ \| SALESMAN\\ \| 7698\\ \|
01-MAY-81\\ \| 1250\\ \| 1400\\ \| 30\\ \|-\\ \| 7698\\ \| BLAKE\\ \|
MANAGER\\ \| 7839\\ \| 09-JUN-81\\ \| 2850\\ \| \\ \| 30\\ \|-\\ \|
7782\\ \| CLARK\\ \| MANAGER\\ \| 7839\\ \| 09-DEC-82\\ \| 2450\\ \| \\
\| 10\\ \|-\\ \| 7788\\ \| SCOTT\\ \| ANALYST\\ \| 7566\\ \| 17-NOV-81\\
\| 3000\\ \| \\ \| 20\\ \|-\\ \| 7839\\ \| KING\\ \| PRESIDENT\\ \| \\
\| 08-SEP-81\\ \| 5000\\ \| \\ \| 10\\ \|-\\ \| 7844\\ \| TURNER\\ \|
SALESMAN\\ \| 7698\\ \| 12-JAN-83\\ \| 1500\\ \| \\ \| 30\\ \|-\\ \|
7876\\ \| ADAMS\\ \| CLERK\\ \| 7788\\ \| 03-DEC-81\\ \| 1100\\ \| \\ \|
20\\ \|-\\ \| 7900\\ \| JAMES\\ \| CLERK\\ \| 7698\\ \| 03-DEC-81\\ \|
950\\ \| \\ \| 30\\ \|-\\ \| 7902\\ \| FORD\\ \| ANALYST\\ \| 7566\\ \|
22-SEP-81\\ \| 3000\\ \| \\ \| 20\\ \|-\\ \| 7934\\ \| MILLER\\ \|
CLERK\\ \| 7782\\ \| 23-JAN-82\\ \| 1300\\ \| \\ \| 10\\ \|\\}\\ \\

#### Tabellen anlegen

\\

-   Der Name der Tabelle\\
-   Der Name jeder Spalte\\
-   Der Typ der Daten, die in jeder Spalte gespeichert werden\\
-   Die L\\'e4nge jeder Spalte\\
-   Weitere optionale Informationen\\

\\

##### DEPT

\\ \\{\| class="wikitable" \\ \|- style="font-weight:bold;"\\ ! DEPTNO\\
! DNAME\\ ! LOC\\ \|-\\ \| 10\\ \| ACCOUNTING\\ \| NEW YORK\\ \|-\\ \|
20\\ \| RESEARCH\\ \| DALLAS\\ \|-\\ \| 30\\ \| SALES\\ \| CHICAGO\\
\|-\\ \| 40\\ \| OPERATIONS\\ \| BOSTON\\ \|\\}\\ \\

    \
    CREATE TABLE DEPT (\
     DEPTNO              NUMBER(2) NOT NULL,\
     DNAME               CHAR(14),\
     LOC                 CHAR(13),\
     CONSTRAINT DEPT_PRIMARY_KEY PRIMARY KEY (DEPTNO));\

\\ \\

#### Einf\\'fcgen von Tupel

\\

    \
    INSERT INTO Tabelle\
    VALUES (Liste von Datenwerten);\

\\ Beim `INSERT` Kommando m\\'fcssen die einzelnen Werte durch Komma
getrennt werden. Character- und Datumswerte m\\'fcssen unter einfache
Hochkomma gestellt werden. Die Werte m\\'fcssen in der gleichen
Reihenfolge angegeben werden, in der die Spalten angegeben worden sind
als die Tabelle erzeugt wurde. \\ \\

##### Beispiel

\\

    INSERT INTO EMP VALUES (7954,'CARTER','CLERK',7698,'7-APR-84',1000,NULL,30);

\\ \\

-   Einf\\'fcgen von Null-Werten:\\

\\

    INSERT INTO EMP (EMPNO,ENAME,HIREDATE,DEPTNO,SAL) VALUES (7955,'WILSON','22-APR-84',30,1500);

\\ \\

-   Einf\\'fcgen von Datumswerten:\\

\\

    INSERT INTO EMP \
    VALUES (7657,'MASON','ANALYST',7566,\
    TO_DATE(\'924/24/84','MM/DD/YY'), 3400, NULL, 20);\

\\ \\

#### \\'c4ndern und L\\'f6schen

\\

##### \\'c4ndern

\\

    \
    UPDATE EMP\
    SET JOB = 'SALESMAN' \
    WHERE ENAME = 'WILSON\'92;\

\\ \\

##### L\\'f6schen

\\

    \
    DELETE FROM BONUS\
    WHERE ENAME = 'WARD';\

\\ \\

#### Daten auslesen (SELECT)

\\

    \
    SELECT DNAME, DEPTNO\
    FROM DEPT;\
    \
    SELECT *\
    FROM EMP \
    \
    SELECT DISTINCT JOB\
    FROM EMP;\
    \
    SELECT (DISTINCT) DNAME \
    FROM DEPT\

\\ }
