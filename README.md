# DB schema

Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario

## Nome tabella: AutoUsate (nome entità: VeicoloUsato)

colonne:

-id_auto INT
-marca VARCHAR(50)
-modello VARCHAR(50)
-carrozzeria VARCHAR(30)
-anno_immatricolazione YEAR
-colore VARCHAR(30)
-condizioni generali dell’auto TEXT
-chilometraggio INT
-alimentazione ENUM('benzina','diesel','elettrica','ibrida','gpl','metano')
-cilindrata INT
-potenza_cv INT
-prezzo DECIMAL(10,2)
-disponibilità ENUM('disponibile','venduta','prenotata')
-data_inserimento DATE
