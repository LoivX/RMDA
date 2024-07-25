# eROSITA Miscentering Distribution Analisis
All'interno di questo breve elaborato si analizzeranno i dati ottenuti dalla survey di eROSITA con lo scopo principale di studiare la miscentering distribution degli ammassi di galassie. 
Con questo obiettivo è stato sviluppato un breve script in python che consente di elaborare i dati della survey basandosi su librerie atte all'analisi e alla rappresentazione dei dati.

Il codice è stato suddiviso per facilitare la lettura nelle seguenti macroaree:
1. **Analisi del catalogo**: estrazione, selezione e prima analisi dati
    - Lettura e selezione dati
    - Analisi della distribuzione delle distanze normalizzate
        - Distribuzione dei dati
        - Variazione distribuzione in funzione di massa e redsift
2. **Sviluppo dei modelli**: studio dei modelli descrittivi della distribuzione
    - Rappresentazione del modello *S15* al variare dei parametri
    - Rappresentazione del modello *Z19* al variare dei parametri
3. **Analisi Bayesiana**: verifica dell'accuratezza dei modelli per la rappresentazione dei dati
    - Modello *S15*
        - Fitting dei parametri con algoritmo emcee
        - Confronto dati - modello
        - Valutazione della riproducibilità dei dati mediante il modello
    - Modello *Z19*
        - Fitting dei parametri con algoritmo emcee
        - Confronto dati - modello
        - Valutazione della riproducibilità dei dati mediante il modello
