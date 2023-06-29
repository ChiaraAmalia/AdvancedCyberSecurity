# Analisi dataset CSE-CIC-IDS 2018 mediante tecniche di unsupervised learning
E' possibile scaricare il dataset al seguente [link](https://www.unb.ca/cic/datasets/ids-2018.html).

## Da cosa siamo partiti
Ad oggi, il rilevamento delle anomalie è al centro dell'attenzione ma la sua adozione richiede una quantità sostanziale di test ed una disponibilità del dataset estremamente rara. La soluzione è stata quindi quella di sviluppare un approccio sistematico per generare set di dati per il rilevamento delle intrusioni.

## Il Dataset
**CSE-CIC-IDS 2018** include sette diversi scenari di attacco:
+ Brute Force
+ HeartBleed
+ Botnet
+ DoS
+ DDoS
+ Web Attack
+ Infiltrazione rete dall'interno

L'infrastruttura di attacco comprende 50 macchine e l'organizzazione vittima ha 5 dipartimenti, comprendente 420 macchine e 30 server. Per la generazione di flussi di traffico di rete ed estrazione delle caratteristiche dei dati grezzi è stato utilizzato **CICFlowMeterV3**.

## PreProcessing dei dati
Al fine di poter effettuare una buona analisi del dataset sono stati rimossi alcuni valori fastidiosi ed effettuato operazioni di scaling sui dati

## Features Selection
È stata svolta un'operazione di features selection al fine di individuare solo le feature più importanti, utilizzando diversi algoritmi: 
+ **ANOVA**
+ **Random Forest**
+ **Support Vector Machine**
+ **Recursive Feature Eliminator**

## Clustering ed Esecuzione
Sono state svolte delle operazioni preliminari su ciascun file analizzato, effettuando se necessario una riduzione del dataset con conseguente bilanciamento delle classi. Sono stati poi applicati diversi algoritmi di clustering:
+ **K-Means**
+ **DBSCAN**
+ **Gerarchico Agglomerativo**
+ **Self-Organizing Map**
Sono stati valutati i pro e i contro di ciascun algoritmo con conseguente individuazione dei parametri ottimali.
Per quanto riguarda l'esecuzione degli algoritmi, dopo aver ottenuto i risultati è stata effettuata un'associazione del cluster alla classe. È stata poi applicata la PCA per poter effettuare un ulteriore confronto e calcolate quindi le metriche, tra cui:
+ **Accuracy**
+ **Precision**
+ **Recall**

Ulteriore documentazione ed i risultati ottenuti sono presenti nella seguente [relazione](https://github.com/ChiaraAmalia/AdvancedCyberSecurity/blob/main/Progetto_Advanced_Cybersecurity.pdf) 

## Autori
+ Chiara Amalia Caporusso
+ David Ceka
+ Melissa Proietti
+ Simone Scalella
+ Riccardo Schiavoni
