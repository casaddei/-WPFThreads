# WPFThreads
programma che a partire dal click di un pulsante fa partire un contatore che va da 0 a 1000.
Il problema nasce dal fatto che il thread che aggiorna l'intrefaccia e il thread che fa funzionare il dodice sono gestiti entrambi dalla UI che però ne può gestire solamente uno. Inaftti una volta avviato il programma e premuto il pulsante, l'interfaccia si bloccherà completamente.
Le lambda expression permettono di scrivere funzioni in modo anonimo,infatti permettono di scrivere funzioni brevi e in linea anzinche definire una funzione completa con un nome. 
Il lock permette di eseguire in modo sicuro una parte di codice, infatti evita che più thread accedano contemporaneamente a una risorsa condivisa.Questo è un problema di atomicità. 
Per risolverlo usiamo il costrutto lock che ci permette di eseguire in modo sicuro una parte di codice, infatti evita che più thread accedeano contemporaneamente a una risorva condivisa. Viene definito con: lock(oggetto), in modo che un solo thread possa eseguire il blocco di codice. Il lock blocca gli altri thread fino a quando il lock non vine rilasciato quello che viene eseguito per primo. 

