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

## Librerie necessarie
Per il funzionamento del codice sono necessarie le seguenti librerie:
- *numpy*
- *pandas*
- *matplotlib*
- *scipy*
- *emcee*
- *pygtc*

Inoltre, il codice è stato sviluppato e commentato all'interno di un *Jupyter Notebook*, è dunque necessaria l'installazione dell'applicazione (oppure l'installazione dell'estensione per VS Code nel caso lo si utilizzi come editor).


## 1. Analisi del catalogo
### Lettura e selezione dati
Per il trattamento dei dati si è optato per l'utilizzo di dataframe pandas. In questo primo frammento si è generato un dataframe a partire dal file .csv contenente i dati della survey. Successivamente sono stati estratti i dati di interesse riguardanti le distanze normalizzate (BCG_offset_R500), le masse (logM500) e il redshift (BEST_Z) degli ammassi di galassie.

### Analisi della distribuzione delle distanze normalizzate
Sono state effettuate analisi preliminari sulla distribuzione delle distanze normalizzate, valutando anche come questa distribuzione varia in funzione della massa e del redshift degli ammassi.

## 2. Sviluppo dei modelli
### Modello S15
Il modello S15 è stato rappresentato al variare dei parametri per comprendere meglio il comportamento della distribuzione.

### Modello Z19
Analogamente, il modello Z19 è stato studiato al variare dei suoi parametri caratteristici.

## 3. Analisi Bayesiana
### Modello S15
Per il modello S15, i parametri sono stati stimati utilizzando l'algoritmo emcee. È stato effettuato un confronto tra i dati osservati e il modello per valutarne l'accuratezza e la capacità di riprodurre i dati osservati.

### Modello Z19
Anche per il modello Z19 si è proceduto con il fitting dei parametri tramite emcee, seguito da un confronto tra i dati e il modello per valutarne l'affidabilità.
