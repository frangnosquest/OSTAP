# OSTAP

Planner statico per la generazione di turnazioni operative. Il progetto è pensato per GitHub Pages: non richiede backend e i file caricati vengono elaborati nel browser.

## Avvio

Aprire `index.html` in un browser oppure pubblicare la repository con GitHub Pages. La libreria SheetJS viene caricata da CDN per leggere e scrivere file Excel.

## Formato roster

Il primo foglio deve avere una riga di intestazione. Sono riconosciute automaticamente colonne chiamate, anche parzialmente, `Nome`, `Squadra` e `Qualifica` (sono sufficienti le prime due). Le colonne aggiuntive potranno ospitare in futuro disponibilità, abilitazioni, vincoli e storico.

Per una prova immediata è disponibile [roster-mock.xlsx](roster-mock.xlsx), con 18 persone distribuite nelle squadre A-D.

## Stato attuale

La versione iniziale include importazione, anteprima roster, calendario su intervallo di date, rotazione base di terzine, alternanza interna/esterna, rotazione weekend e export Excel. Le date di inizio e fine sono selezionabili dai calendari nativi del browser. Il generatore è volutamente una base parametrica: i vincoli di servizio, festività e uso dello storico devono essere formalizzati prima di rendere l'algoritmo vincolante.
