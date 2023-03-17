# WPFThreads
programma che a partire dal click di un pulsante fa partire un contatore che va da 0 a 1000.
Il problema nasce dal fatto che il thread che aggiorna l'intrefaccia e il thread che fa funzionare il dodice sono gestiti entrambi dalla UI che però ne può gestire solamente uno. Inaftti una volta avviato il programma e premuto il pulsante, l'interfaccia si bloccherà completamente.
Per risolvere questo problema  abbiamo usato una lambda expression, il costrutto lock.
Il lock permette di eseguire in modo sicuro una parte di codice, infatti evita che più thread accedano contemporaneamente a una risorsa condivisa. 
Il lock si dichiara tramite la parola chiave lock e una parentesi in cui è contenuto l'oggetto di blocco. 

