# IMMIGRAZIONE TRA DATI E CRONACA
**Autrici**: Dania Chiari, Claudia Cocci, Sara De Simone

**Corso**: Introduzione alla programmazione

**Università**: Dati, metodi e modelli per le scienze linguistiche (Unibo)

## Panoramica
Questo progetto nasce come lavoro di gruppo nell'ambito del corso universitario di Introduzione alla Programmazione (**python**). La versione pubblicata in questo repository include modifiche e correzioni apportate autonomamente dalla sottoscritta in un secondo momento, dopo la conclusione dell'esame.
Di seguito, vengono illustrati gli obiettivi del lavoro:
1.  **Analisi statistico-distribuzionale**: indagare la presenza e l'evoluzione demografica di sei comunità target sul territorio italiano dal 2013-2019, prestando attenzione anche alla distribuzione geografica nelle diverse ripartizioni territoriali (Nord, Centro, Sud, Isole).
2.  **Analisi comparativa**: verificare se la rappresentazione mediatica di tali comunità, nel corpus di articoli de *La Repubblica*, sia coerente rispetto all'effettiva presenza sul territorio. L'analisi si articola in tre confronti:
3.  **Analisi terminologica**: intercettare l'esistenza di **associazioni terminologiche** tra comunità straniere e parole con differenti connotazioni (positive, negative o neutre), rintracciate negli articoli incentrati sull'immigrazione.

-  I testi degli articoli sono stati tokenizzati con una funzione di tokenizzazione basata su regex (`\w+`), previa normalizzazione in minuscolo.
-  È stata sviluppata un'euristica basata su criteri posizionali, al fine di conteggiare con maggiore precisione le occorrenze relative alle nazionalità target.
-  Per l'analisi terminologica è stato creato un codice che crea, per ogni articolo, un set di indici di contesto, ovvero gli indici delle parole che si trovano intorno all'occorrenza della nazionalità entro una finestra predefinita.

## Struttura
```
PROGETTO/
├── dati/
│   ├── change-it/
│   │   └── repubblica.csv      (da scaricare, vedi sotto)
│   └── istat/
│       └── Dati_RCS/
├── progetto_github.ipynb
└── README.md
```

## Dati 
### Dati Istat
I dati relativi alle cittadinanze straniere sono forniti dall'Istat e inclusi in questo repository, nella cartella `dati/istat/Dati_RCS/`.
### repubblica.csv
Il file `repubblica.csv` (63.702 articoli de *La Repubblica*, 2013-2019) non è incluso in questo repository per motivi di dimensione.
**Scaricalo da [qui](https://drive.google.com/file/d/1bE36jHuy_xLcyuZc2VY1J5YhDyA09_tC/view?usp=sharing)** e posizionalo in `dati/change-it/repubblica.csv` prima di eseguire il notebook.
Il file deriva dal dataset [ChangeIT](https://github.com/LanD-FBK/ChangeIT) (progetto EVALITA), ma è stato preventivamente filtrato/ripulito dal docente del corso; non corrisponde quindi esattamente alla versione pubblica originale del dataset.

## Come eseguire il notebook
1. Clonare il repository
2. Scaricare `repubblica.csv` dal link sopra e posizionalo in `dati/change-it/repubblica.csv`
3. Installare le dipendenze: `pandas`, `numpy`, `matplotlib`, `seaborn` (oltre a `re` e `os`, già inclusi in Python)
4. Eseguire `progetto_github.ipynb` in ordine, dall'alto verso il basso
