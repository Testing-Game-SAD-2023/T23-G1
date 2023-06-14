<h1> Testing Game </h1>

<h2> Gruppo 1 </h2>
Iole Morabito M63001448 i.morabito@studenti.unina.it
Marika Sasso M63001438 marik.sasso@studenti.unina.it
Francesca Terracciano M63001550 francesca.terracciano@studenti.unina.it
Doriana Traetto M63001416 d.traetto@studenti.unina.it

<h2>  Task 2-3: Registrazione ed Autenticazione dei Giocatori </h2>

L'applicazione deve consentire agli studenti di registrarsi per poter conservare la storia delle attività svolte, oppure per accedere a requisiti di gioco più complessi. All'atto della registrazione, lo studente fornirà nome, cognome, un indirizzo e-mail valido ed una password, il sistema dopo aver controllato la validità dei dati forniti, aggiungerà il giocatore all'elenco dei giocatori registrati e gli assocerà un ID univoco. Sarebbe desiderabile raccogliere anche altre informazioni sugli studenti, come il corso di studi a cui sono iscritti (Bachelor, Master Degree, o altro).
All'atto della autenticazione, lo studente fornirà l'indirizzo e-mail fornito per la registrazione e la relativa password, il sistema dopo aver controllato la validità dei dati forniti, autenticherà il giocatore e gli fornirà una schermata per l'accesso alle funzionalità di gioco o di consultazione delle sessioni di gioco passate.

<h3> Deployment dell'applicazione </h3>

*Aprire Docker 
*Aprire un terminale da amministratore e posizionarsi sul percorso dove è contenuto il progetto
	-docker-compose up: viene utilizzato per avviare i servizi definiti in un file di configurazione "docker-compose.yml". Viene creata l’immagine del container e viene eseguito il running.
*Per effettuare le richieste, aprire da browser le pagine tramite i path in locale (http://localhost:8080/register, http://localhost:8080/login, ecc.)
*Per verificare la correttezza del popolamento delle tabelle del database, aprire un terminale ed eseguire i seguenti comandi:
	-docker exec –it g1-t2t3-app-1 bash: viene utilizzato per entrare all'interno di un container Docker in esecuzione e avviare una shell interattiva al suo interno.
	-mysql –u root –p STUDENTSREPO: viene utilizzato per accedere all'interfaccia della riga di comando di MySQL e connettersi al database "STUDENTSREPO" utilizzando l'utente "root" e richiedendo la password “password”.
*Utilizzare i comandi SQL per la gestione delle tabelle (SELECT, DROP, SHOW TABLES, ecc.)
