🇮🇹 Italiano:
Nel mio progetto Laravel ho sviluppato un sistema completo per la gestione dei giocatori. Ho creato le rotte necessarie per consentire l'inserimento, la memorizzazione nel database e la visualizzazione dei giocatori registrati.

In particolare, ho definito una rotta GET per la pagina di creazione (/player/create) e una rotta POST per la sottomissione del form (/player/submit), utilizzando un controller dedicato (PlayerController). All’interno di questo controller, ho gestito i dati provenienti dal form attraverso una classe di validazione personalizzata (PlayerRequest) per garantire la correttezza dei dati immessi.

Per quanto riguarda il salvataggio, ho implementato un controllo sull'upload delle immagini e ho previsto un comportamento sicuro nel caso in cui l’utente non carichi alcun file. I dati vengono poi salvati nel database utilizzando il Mass Assignment, dopo aver impostato correttamente il campo fillable nel modello Player.

Infine, ho creato anche una rotta per la visualizzazione dell'elenco dei giocatori salvati nel database (/player/index), mostrando le informazioni tramite una view dedicata.


--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


🇬🇧 English:
In my Laravel project, I developed a complete system for managing players. I created the necessary routes to allow users to add new players, store them in the database, and view the list of registered players.

Specifically, I defined a GET route for the creation page (/player/create) and a POST route for the form submission (/player/submit), using a dedicated controller (PlayerController). Within the controller, I handled the incoming form data through a custom validation class (PlayerRequest) to ensure input correctness.

Regarding storage, I implemented a check for image upload and provided a safe fallback in case no file is submitted. The data is stored in the database using Mass Assignment, after correctly setting the fillable property in the Player model.

Lastly, I added a route to display the list of saved players (/player/index), presenting the information through a dedicated view.
