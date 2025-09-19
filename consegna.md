## App Frontend

L'applicazione deve rappresentare un dashboard (semplice) con all'inizio una pagina di log-in(fittizia, deve solo funzionare lato software senza auth provider), una volta loggato l'app deve contenere:

- una navbar laterale con due pulsanti o collegamenti ipertestuali che riportano a due pagine
- un pagina (collegata alla prima voce) che rappresenta una tabella con le persone segnate
- una pagina (collegata alla seconda voce) che contiene un form dove registrare l'accesso

lo stile (css) dell'applicazione è libero.

## App Backend

Fare una semplice rest API in golang DOCUMENTATA (openapi/swagger) che effettua query su mongodb necessarie alla visualizzazione dei dati nell'app frontend

endpoint operativi da sviluppare:

- "/api/v1/lista-accessi"
- "/api/v1/registra-accesso"
- "/api/v1/modifica-accesso"

endpoint di servizio da sviluppare:

- "/health" un semplice endpoint che deve tornare uno status 200 (importanza a livello infrastrutturale)

## Database MongoDB

Utilizzare il database NoSQL MongoDB per la persistenza dei dati
il database si chiamerà:

- **gpa-registro-accessi**

e per il momento una sola collection chiamata:

- **registro-accessi**