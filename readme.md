# CALCOLO BIGLIETTO DEL PREZZO DEL TRENO

## TRACCIA

```plaintext
cartella/repo js-biglietto-treno

Il programma dovrà chiedere all'utente il numero di chilometri che vuole percorrere e l'età del passeggero.
Sulla base di queste informazioni dovrà calcolare il prezzo totale del viaggio, secondo queste regole:
- il prezzo del biglietto è definito in base ai km (0.21 € al km)
- va applicato uno sconto del 20% per i minorenni
- va applicato uno sconto del 40% per gli over 65
L'output del prezzo finale va messo fuori in forma umana (con massimo due decimali, per indicare centesimi sul prezzo).
```

## SVOLGIMENTO

- Inizializzo una costante per il prezzo unitario di 1 km, due costanti per la percentuale di sconto
- Dichiaro una variabile prezzo che andrò man mano a "modellare"
- Inizializzo la costante per il numero di km che si vogliono percorrere con un prompt
- Inizializzo la costante per l' età del passeggero con un prompt
- Controllo se i valori inseriti dall' utente sono accettabile, solo se corretti procedo
- Calcolo il prezzo del biglietto moltiplicando i km desiderati per la tariffa al km e lo applico alla variabile prezzo (qui lordo, senza sconto)
- Gestisco la scontistica da applicare in base all'età modificando sempre la stessa variabile del prezzo (rendendolo netto)
- Arrotondo e rendo visibile la parte decimale che mi interessa (Decimi e Centesimi)
- Stampo il prezzo finale, al netto di eventuale sconto, con l'elemento id nell'HTML
