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
