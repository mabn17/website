---
author: mos
revision:
    "2017-12-27": (PA1, mos) Arbete pågår.
...
Kmom01: Databas
====================================

[WARNING]
Kursutveckling pågår inför VT18.
[/WARNING]

Då dyker vi in i relationsdatabaser tillsammans med SQL och modellering av databaser.

I en relationsdatabas pratar vi SQL med databasen. Vi skriver SQL för att skapa tabeller och för att lägga till, uppdatera, visa och radera data från databasen.

Till databasen behövs klientprogram som kan användas för att prata med databasen.

Vi introduceras till databasen MySQL och dess olika klienter samt lär oss använda SQL tillsammans med MySQL. Du får jobba igenom en övning i SQL som introducerar dig i grundläggande konstruktioner för att skapa och uppdatera en databas.

Du får pröva att använda tre olika klienter till MySQL, alla tre har sin plats och användningsområde vid olika tillfällen.

<!--more-->

[FIGURE src=/image/snapshot/mamp-mysql-clu-test.jpg?w=w1&q=60 caption="SQL i en textbaserad klient."]

[FIGURE src=/image/snapshot/wamp-phpmyadmin.png?w=w1&sa=jpg&q=60 caption="SQL i en webbaserad klient."]

[FIGURE src=/image/snapshot/sql-ovning-alter-table.jpg?w=w1&q=60 caption="SQL som det ser ut i desktop-klienten MySQL WorkBench."]

<small><i>(Detta är instruktionen för kursmomentet och omfattar det som skall göras inom ramen för kursmomentet. Momentet omfattar cirka **20 studietimmar** inklusive läsning, arbete med övningar och uppgifter, felsökning, problemlösning, redovisning och eftertanke. Läs igenom hela kursmomentet innan du börjar jobba. Om möjligt -- planera och prioritera var du vill lägga tiden.)</i></small>



Labbmiljön  {#labbmiljo}
---------------------------------

*(ca: 2-4 studietimmar)*

Det finns en [längre beskrivning om kursens labbmiljö](./../installera-labbmiljo). Läs den om du är osäker på vad som skall göras, eller om detta är din första dbwebb-kurs.

Den korta varianten är att du behöver [installera labbmiljön](./../labbmiljo), uppdatera [dbwebb-cli](dbwebb-cli) samt klona och initiera kursrepot.

```text
# Gå till din katalog för dbwebb-kurser
dbwebb selfupdate
dbwebb clone databas
cd databas
dbwebb init
```



Läsanvisningar  {#lasanvisningar}
---------------------------------

*(ca: 8-10 studietimmar)*


###Kurslitteratur  {#kurslitteratur}

Läs följande:

1. [Databasteknik](kunskap/boken-databasteknik) om MySQL.
    * Kap 1: Databaser och databashanterare
    * Kap 7: Introduktion till frågespråket SQL
    * Kap 28: Introduktion till MySQL

Viss information finns i [bokens webbkurs](http://www.databasteknik.se/webbkursen/), del 1 och 3.



###Artiklar {#artiklar}

Kika igenom följande artiklar.

1. Kika igenom referensmanualen för MySQL, bara kort och översiktligt, men se till att du kan hitta till den delen som visar hur SQL skall skrivas i MySQL.
    * [SQL Statement Syntax](https://dev.mysql.com/doc/refman/5.7/en/sql-syntax.html)



Övningar & Uppgifter  {#ovningar_uppgifter}
-------------------------------------------

*(ca: 8-10 studietimmar)*



###Övningar {#ovningar}

Genomför följande övning för att förbereda inför uppgifterna.

1. Jobba igenom guiden "[Kom igång med databasen MySQL och dess klienter](kunskap/kom-igang-med-databasen-mysql-och-dess-klienter)". Som databasutvecklare är det bra att du ha koll på olika varianter av klienter, testa allihop och se till att din lokala utvecklingsmiljö fungerar.

1. Bekanta dig med "[BTH's labbmiljö för databasen MySQL](kunskap/bth-s-labbmiljo-for-databasen-mysql)". Se till att du kan använda BTH's databasserver för MySQL. Använd de olika klienterna för att koppla upp dig. Spara dina eventuella testfiler i `me/kmom01/mysql`.



###Uppgifter {#uppgifter}

Dessa uppgifter skall utföras och redovisas.

1. Gör uppgiften "[Skapa en me-sida för redovisning i dbwebb-kurs](uppgift/skapa-en-me-sida-for-redovisning-i-dbwebb-kurs)". Spara resultatet i `me/redovisa`.

1. Jobba igenom uppgiften "[Kom igång med SQL (del 1)](uppgift/kom-igang-med-sql)" genom att utföra den i MySQL Workbench. Spara all SQL-kod i `me/kmom01/skolan1/skolan.sql` och utför minst 2/3 av uppgifterna. Dokumentera vilka uppgifter du hoppar över. Jobba gärna i grupp och hjälp varandra, men se alltid till att skriva dina egna SQL-satser. Se till att du förstår begreppen HAVING, subqueries och OUTER JOIN. (inkl export, import)


1. Gör laborationen "[SQL lab, introduktion till SQL](uppgift/sql-lab-introduktion-till-sql-dbjs)" som låter dig träna på grunderna i SQL kommandon.



Resultat & Redovisning  {#resultat_redovisning}
-----------------------------------------------

*(ca: 1-2 studietimmar)*

Läs [instruktionen om hur du skall redovisa](./../redovisa).

Se till att följande frågor besvaras i redovisningstexten.

* Hur känns det att komma igång med MySQL och dess klienter?
* Har du jobbat med liknande tidigare?

TIL; är en akronym för "Today I Learned" vilket leksamt anspelar på att det finns alltid nya saker att lära sig, varje dag. Man brukar lyfta upp saker man lärt sig och där man kanske hajade till lite extra över dess nyttighet eller enkelhet, eller så var det bara en ny lärdom för dagen som man vill notera.

* Vilken är din TIL; för detta kmom?