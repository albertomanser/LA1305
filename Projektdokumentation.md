![image](https://github.com/albertomanser/LA1305/assets/110892537/05989ad3-9edb-4208-8cfd-091c9e484ecf)# LA1305
# Projekt-Dokumentation

Alberto Manser

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
| 17.5.2024| 0.0.1   | Erstellung der Userstories und Testfälle, Abschluss von I,P,E|
| 24.5.2024| 0.0.2   | Erstellung des Projektes und der Erkunden Funktion           |
| 31.5.2024| 0.0.3   | Erstellung des Ladens und der Statusfunktion Abschluss von R |
| 7.6.2024| 1.0.0   | Durchführung Tests, Abschluss dokumentation Abschluss K, A   |

## 1 Informieren

### 1.1 Ihr Projekt

Ein Abenteuer Spiel in c#

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1    | muss              | Funktional     | Als User möchte ich erkunden können |
| 2  |  muss               | Funktional     | Als User möchte ich Gegner begegnen können                                   |
| 3    | muss | Funktional |Als User möchte ich Gold sammeln können |
| 4 | kann  | Funktional  | Als User möchte ich Ausrüstung kaufen können |
| 5 | muss | Funktional | Als User möchte ich mich heilen können |
| 6 | muss | Funktional | Als User möchte ich sterben können |
| 7 | kann | Qualität | Als User möchte ich ein stabiles Game spielen |
| 8 | kann | Qualität | Als User möchte ich beim erkunden nichts finden können |



### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  | Programm offen             | 1.        | Sie sind erkunden gegangen, sie haben ... gefunden!|
| 2.1  | Programm offen             | 1.        | Sie sind einem Gegner begegnet: Gegner Leben: 30 Deine Leben: 100                  |
| 3.1  | Im Kampf gegen Gegner  | Abschluss kampf | Sie haben den Gegner getötet, sie haben 20 Gold erhalten. |
| 3.2  | Programm offen | 1. |Sie haben ... gefunden und 15 Gold erhalten! |
| 3.3  | Erkunden | 1. | Sie haben ... gefunden und 15 Gold erhalten! Sie haben nun 30 Gold |
| 4.1  | Laden offen, 50 Gold | 1 | Sie haben eine Waffe für 50 Gold gekauft, ihr schaden beträgt nun 20 |
| 4.2  | Laden offen, 40 Gold | 1 | Sie haben nicht genug Gold für dies. |
| 5.1 | Laden offen, 20 Gold, 50/100 Leben | 4 | Sie haben sich geheilt, ihre Gesundheit beträgt wieder 100, sie haben noch 0 Gold. |
| 5.2 | Laden offen, 10 Gold, 50/100 Leben| 4 | Sie haben nicht genug Gold dafür |
| 5.3 | Laden offen, 20 Gold, 100 Leben | 4 | Sie haben schon volle Lebenspunkte. |
| 6.1 | Kampf Leben noch 8 | Angriff | Gegner hat dir 8 Schaden zugefügt, sie sind gestorben Spiel vorüber|
| 7.1 | Spiel offen | a | ungültiger Input, versuchen sie es nochmal |
| 7.2 | Spiel offen | 7 | ungültiger Input, versuchen sie es nochmal |
| 8.1 | Spiel offen | 1 | sie haben erkundet und nichts gefunden. |


### 1.4 Diagramme


## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  | 24.5.2024      | Manser Alberto           | Erkundungfunktion              | 2*45              |
| 2.A  | 24.5.2024      | Manser Alberto           | Gegner begegnungen sowie Kampf              | 3*45              |
| 3.A |  24.5.2024      | Manser Alberto | Gold bei erkunden und beendung Kampf | 45 |
| 4.A | 31.5.2024 | Manser Alberto | Laden sowie die Ausrüstungen im Laden | 2*45 |
| 5.A | 31.5.2024 | Manser Alberto | Heilung im Laden einbauen | 30 |
| 6.A | 31.5.2024 | Manser Alberto | sterbefunktion bei 0 Leben | 30 |
| 7.A | 31.5.2024 | Manser Alberto | Failsafes und catch schlaufen | 45 |
| 8.A | 31.5.2024 | Manser Alberto | Fehlschlag funktion bei Erkunden | 30 |


Total: 11*45


## 3 Entscheiden


## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A | 24.5.2024| Manser Alberto|2*45|2*45                   |
| 2.A | 24.5.2024| Manser Alberto| 3*45|2*45                  |
| 3.A | 24.5.2024| Manser Alberto| 45 | 60|
| 4.A | 31.5.2024| Manser Alberto| 2*45| 2*45|
| 5.A | 31.5.2024| Manser Alberto| 30 | 30|
| 6.A | 31.5.2024| Manser Alberto| 30 | 20|
| 7.A | 31.5.2024| Manser Alberto| 45 | 2*45|
| 8.A | 24.5.2024| Manser Alberto| 30 | 30 |


## 5 Kontrollieren
### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  | 7.6.2024|Funktioniert|Manser Alberto|
| 2.1  | 7.6.2024|Funktioniert|Manser Alberto|
| 3.1  | 7.6.2024|Funktioniert|Manser Alberto|
| 3.2  | 7.6.2024|Funktioniert|Manser Alberto|
| 3.3  | 7.6.2024|Funktioniert|Manser Alberto|
| 4.1  | 7.6.2024|Funktioniert|Manser Alberto|
| 4.2  | 7.6.2024|Funktioniert|Manser Alberto|
| 5.1  | 7.6.2024|Funktioniert|Manser Alberto|
| 5.2  | 7.6.2024|Funktioniert|Manser Alberto|
| 5.3  | 7.6.2024|Funktioniert|Manser Alberto|
| 6.1  | 7.6.2024|Funktioniert|Manser Alberto|
| 7.1  | 7.6.2024|Funktioniert|Manser Alberto|
| 7.2  | 7.6.2024|Funktioniert|Manser Alberto|
| 8.1  | 7.6.2024|Funktioniert|Manser Alberto|


Fazit:
Das Programm funktioniert einwandfrei, alle Userstories wurden erfüllt und die Testfälle haben alle funktioniert.

