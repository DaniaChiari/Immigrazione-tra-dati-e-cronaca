# IMMIGRAZIONE TRA DATI E CRONACA
**Autrici**: Dania Chiari, Claudia Cocci, Sara De Simone

**Corso**: Introduzione alla programmazione

**Università**: Dati, metodi e modelli per le scienze linguistiche (Unibo)

## Panoramica
Questo progetto nasce come lavoro di gruppo nell'ambito del corso universitario di Introduzione alla Programmazione. La versione pubblicata in questo repository include modifiche e correzioni apportate autonomamente dalla sottoscritta in un secondo momento, successivamente alla conclusione dell'esame.

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
