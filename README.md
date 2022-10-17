Linux som utvecklingsmiljö 1

Uppgift 9 - Paket för distribution

A:
Modifiera electrotest så all nödvändig kod hamnar i en enda .c-fil electrotest-standalone.c

Skapa ett deb-paket, electrotest-standalone som installerar programmet i filsystemet

Avlusa paketet med lintian vid körning av debuild undantaget:
improbable-bug-number-in-closes
new-package-should-close-itp-bug

Extrahera information ur deb-paketet med dpkg-deb samt verifiera informationen med växlarna -c och -f

