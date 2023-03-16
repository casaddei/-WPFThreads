# WPFThreads
programma che a partire dal click di un pulsante fa partire un contatore che va da 0 a 1000.
Il problema nasce dal fatto che il thread che aggiorna l'intrefaccia e il thread che fa funzionare il dodice sono gestiti entrambi dalla UI che però ne può gestire solamente uno. Inaftti una volta avviato il programma e premuto il pulsante, l'interfaccia si bloccherà completamente.
Per risolvere questo problema  abbiamo usato una lambda expression, il dispatcher che fa in modo che un thread non venga interrotto fino alla fine del suo lavoro. 
Per evitare che l'interfaccia si aggiornasse troppo velocemente abbiamo usato un il thread.sleep(500), un metodo che gestisce l'aggiornamento dell'interfaccia che avviene ogni 500 millisecondi. 
Esempio di lambda expression: 


  Dispatcher.Invoke(
                    () =>
                    {
                        txtCounter1.Text = _counter.ToString();
                    }
                );


Una lambda expression viene definita tramite 
(
()=> 
{//istruzioni da eseguire}
);
