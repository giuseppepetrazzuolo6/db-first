# DB schema

Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario

## Nome tabella: AutoUsate (nome entità: VeicoloUsato)

colonne:

-id_auto INT - NOT NULL
-marca VARCHAR(50) - NOT NULL
-modello VARCHAR(50) - NOT NULL
-carrozzeria VARCHAR(30) - NULL
-anno_immatricolazione YEAR - NOT NULL
-colore VARCHAR(30) - NULL
-condizioni_generali TEXT - NULL
-chilometraggio INT - NOT NULL
-alimentazione ENUM('benzina','diesel','elettrica','ibrida','gpl','metano') - NOT NULL
-cilindrata INT - NULL
-potenza_cv INT - NULL
-prezzo DECIMAL(10,2) - NOT NULL
-disponibilità ENUM('disponibile','venduta','prenotata') - NOT NULL DEFAULT('disponibile')
-data_inserimento DATE - NOT NULL DEFAULT(now())
