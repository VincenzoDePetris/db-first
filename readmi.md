- CONSEGNA

Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.
potete usare una tabellina markdown o un semplice file di testo se vi riesce più comodo!

| COLONNA      | TIPO         | ATTRIBUTI                   |
| ------------ | ------------ | --------------------------- |
| id           | BIGINT       | PRIMARY KEY, AUTO INCREMENT |
| brand        | VARCHAR (20) | NOT NULL                    |
| model        | VARCHAR (50) | NOT NULL                    |
| tot_km       | MEDIUMINT    | UNSIGNED NOT NULL           |
| condition    | TINYINT      | UNSIGNED NOT NULL DEFAU(6)  |
| color        | VARCHAR (15) | NULL                        |
| engine_type  | CHAR(1)      | NOT NULL                    |
| engine_power | SMALLINT     | NULL                        |
| traction     | CHAR(3)      | NULL                        |
| owner_number | TINYINT      | DEFAULT(1) NULL             |
| price        | SMALLINT     | UNSIGNED NOT NULL           |
| plate_number | CHAR(7)      | NOT NULL, UNIQUE            |

- EXPLANATION
  - condition: integer rating from 1 to 10, 1=bad condition, 10=good condition
  - engine_type: refers to the first letter of engine type
    - E = electric
    - O = oil
    - M = mild Hybrid
    - H = Hybrid
    - D = diesel
    - G = gpl
  - traction: refers to the first letter of traction type
    - AWD = all-wheel-drive
    - FWD = front wheel drive
    - RWD = rear wheel drive
    - 4WD = 4 wheel drive
