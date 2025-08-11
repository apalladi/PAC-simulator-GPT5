# Simulatore Monte Carlo di un PAC

## Descrizione

Questa applicazione a pagina singola simula l’andamento di un Piano di Accumulo Capitale (PAC) tramite simulazioni Monte Carlo basate su log-rendimenti gaussiani (modello geometric Brownian mensile).

L’app mostra graficamente e testualmente l’evoluzione del capitale investito, la distribuzione finale del capitale, i massimi drawdown e altre statistiche rilevanti per aiutare a valutare i rischi e i potenziali risultati dell’investimento.

---

## Parametri di Input

L’utente può personalizzare i seguenti parametri:

- **Versamento iniziale (€)**: capitale versato una tantum all’inizio  
- **Versamento mensile (€)**: quota versata ogni mese  
- **Durata (anni)**: periodo totale dell’investimento  
- **Rendimento medio atteso annuo (%)**: rendimento medio previsto ogni anno  
- **Deviazione standard annua (%)**: volatilità attesa dei rendimenti  
- **Tassazione sui guadagni**: scelta tra 0%, 12.5% e 26%  
- **Numero di simulazioni Monte Carlo**: da 100 in su, più è alto più l’analisi è precisa ma richiede tempo  
- **Adeguamento mensile all’inflazione**: attivabile per far crescere i versamenti in linea con l’inflazione attesa  

---

## Output e Risultati

L’app produce sia output grafici che testuali:

- **Grafici**:  
  - Evoluzione del capitale nel tempo per ciascuna simulazione  
  - Distribuzione del capitale finale al termine del periodo  
  - Distribuzione dei massimi drawdown raggiunti in ogni simulazione  

- **Valori numerici**:  
  - Capitale complessivamente versato  
  - Valore mediano finale del capitale  
  - Intervallo di confidenza al 95% del capitale finale  
  - Valore mediano del massimo drawdown  
  - Intervallo di confidenza al 95% del drawdown  
  - Probabilità che il capitale finale sia inferiore al capitale versato (rischio di perdita reale)  

---

## Metodo di simulazione

La simulazione è basata su una distribuzione gaussiana dei **log-rendimenti mensili**, assumendo che il capitale segua un processo di tipo geometric Brownian motion mensile. La tassazione viene applicata al guadagno finale. Il modello permette di generare molteplici scenari futuri per analizzare la variabilità e il rischio.

---

## Collaborazione

Questa applicazione è stata realizzata da Andrea Palladino in collaborazione con **ChatGPT 5 Pro**, che ha supportato la progettazione e lo sviluppo del codice sulla base di un prompt dettagliato.

---

## Come usare l’app

1. Aprire il file HTML in un browser moderno (funziona offline).  
2. Inserire i parametri personalizzati nella sezione “Parametri del PAC” e “Parametri mercato”.  
3. Cliccare su **Esegui simulazione** e attendere il completamento (il tempo dipende dal numero di simulazioni).  
4. Esplorare i risultati grafici e testuali nella sezione di output.  
5. Per effettuare una nuova simulazione, cliccare su **Ripristina**.

---

## Crediti

**Credit:** Dr. Andrea Palladino e ChatGPT 5 Pro.

---

> **Nota:** Questo simulatore fornisce stime statistiche basate su un modello semplificato e non rappresenta una previsione certa o una consulenza finanziaria.
