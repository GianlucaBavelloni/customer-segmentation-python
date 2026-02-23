# 📊 E-Commerce Customer Segmentation: RFM Analysis Project

## 📌 Project Overview
L'obiettivo di questo progetto è analizzare il comportamento dei clienti di un E-commerce per identificare segmenti ad alto valore e migliorare le strategie di retention. Attraverso l'analisi **RFM (Recency, Frequency, Monetary)**, ho classificato il database clienti in base al loro valore storico e alla frequenza di acquisto, fornendo insight pronti per campagne marketing mirate.

### 📂 Dataset Information
* **Type:** Transactional Data (Customer ID, Order Date, Order Value).
* **Source:** Kaggle / E-commerce Transactional Database.
* **Volume:** Analisi effettuata su migliaia di record storici.

---

## 🛠️ Methodology & Technical Workflow

### Phase 1: Data Preparation & Cleaning (Python)
Prima del calcolo delle metriche, ho ripulito i dati utilizzando **Pandas**:
* **Data Formatting:** Conversione delle date in oggetti `datetime` per calcolare la Recency.
* **Handling Anomalies:** Rimozione di ordini annullati e valori negativi per garantire l'accuratezza del valore monetario.
* **Feature Engineering:** Calcolo del `Total Price` per ogni transazione (Quantity * Unit Price).

### Phase 2: RFM Calculation
Ho calcolato le tre metriche chiave per ogni singolo cliente:
1.  **Recency (R):** Giorni trascorsi dall'ultimo acquisto (più è basso, meglio è).
2.  **Frequency (F):** Numero totale di ordini effettuati nel periodo analizzato.
3.  **Monetary (M):** Totale della spesa effettuata dal cliente.

### Phase 3: Scoring & Segmentation
Per rendere i dati comparabili, ho assegnato punteggi da 1 a 5 utilizzando i **quintili** (`pd.qcut`):
* **RFM Score:** Concatenazione dei punteggi (es: 555 è un cliente perfetto).
* **Segmentazione Logica:** Ho raggruppato i punteggi in segmenti definiti:
    * **Champions:** Recency bassa, alta frequenza e spesa elevata.
    * **Loyal Customers:** Acquistano regolarmente.
    * **At Risk / Can't Lose Them:** Clienti che spendevano molto ma non acquistano da molto tempo.
    * **Hibernating:** Clienti con bassi punteggi in tutte le categorie.

---

## 📈 Key Results & Insights

Grazie all'analisi in Python, abbiamo ottenuto i seguenti risultati:
* **Identification of "Champions":** Circa il **15% della base clienti** genera oltre il **40% del fatturato totale**.
* **Churn Warning:** Ho identificato un segmento critico di "At Risk Customers" (punteggio Recency 1 o 2) che necessita di campagne di riattivazione immediate.
* **Average Ticket Size:** La distribuzione Monetary ha rivelato che la maggior parte dei clienti si attesta su una spesa media definita, ma i "Champions" hanno un valore di spesa 5 volte superiore alla media.



---

## 📊 Business Intelligence (Power BI Integration)
I risultati dell'analisi Python sono stati importati in Power BI per creare una dashboard interattiva:
* **Segment Distribution:** Visualizzazione della dimensione di ogni gruppo (Champions vs Hibernating).
* **Monetary vs Frequency:** Scatter plot per identificare visivamente i cluster di valore.
* **Trend Analysis:** Analisi temporale degli acquisti per capire i periodi di picco.



---

## 🚀 Repository Content
* `/notebooks`: Jupyter Notebook con il codice Python per il calcolo RFM e scoring.
* `/data`: Dataset pulito pronto per la visualizzazione.
* `/reports`: Screenshot e file `.pbix` della dashboard finale.

---
**Author:** [Il Tuo Nome]
**Role:** Data Analyst# 📊 E-Commerce Customer Segmentation: RFM Analysis Project

## 📌 Project Overview
L'obiettivo di questo progetto è analizzare il comportamento dei clienti di un E-commerce per identificare segmenti ad alto valore e migliorare le strategie di retention. Attraverso l'analisi **RFM (Recency, Frequency, Monetary)**, ho classificato il database clienti in base al loro valore storico e alla frequenza di acquisto, fornendo insight pronti per campagne marketing mirate.

### 📂 Dataset Information
* **Type:** Transactional Data (Customer ID, Order Date, Order Value).
* **Source:** Kaggle / E-commerce Transactional Database.
* **Volume:** Analisi effettuata su migliaia di record storici.

---

## 🛠️ Methodology & Technical Workflow

### Phase 1: Data Preparation & Cleaning (Python)
Prima del calcolo delle metriche, ho ripulito i dati utilizzando **Pandas**:
* **Data Formatting:** Conversione delle date in oggetti `datetime` per calcolare la Recency.
* **Handling Anomalies:** Rimozione di ordini annullati e valori negativi per garantire l'accuratezza del valore monetario.
* **Feature Engineering:** Calcolo del `Total Price` per ogni transazione (Quantity * Unit Price).

### Phase 2: RFM Calculation
Ho calcolato le tre metriche chiave per ogni singolo cliente:
1.  **Recency (R):** Giorni trascorsi dall'ultimo acquisto (più è basso, meglio è).
2.  **Frequency (F):** Numero totale di ordini effettuati nel periodo analizzato.
3.  **Monetary (M):** Totale della spesa effettuata dal cliente.

### Phase 3: Scoring & Segmentation
Per rendere i dati comparabili, ho assegnato punteggi da 1 a 5 utilizzando i **quintili** (`pd.qcut`):
* **RFM Score:** Concatenazione dei punteggi (es: 555 è un cliente perfetto).
* **Segmentazione Logica:** Ho raggruppato i punteggi in segmenti definiti:
    * **Champions:** Recency bassa, alta frequenza e spesa elevata.
    * **Loyal Customers:** Acquistano regolarmente.
    * **At Risk / Can't Lose Them:** Clienti che spendevano molto ma non acquistano da molto tempo.
    * **Hibernating:** Clienti con bassi punteggi in tutte le categorie.

---

## 📈 Key Results & Insights

Grazie all'analisi in Python, abbiamo ottenuto i seguenti risultati:
* **Identification of "Champions":** Circa il **15% della base clienti** genera oltre il **40% del fatturato totale**.
* **Churn Warning:** Ho identificato un segmento critico di "At Risk Customers" (punteggio Recency 1 o 2) che necessita di campagne di riattivazione immediate.
* **Average Ticket Size:** La distribuzione Monetary ha rivelato che la maggior parte dei clienti si attesta su una spesa media definita, ma i "Champions" hanno un valore di spesa 5 volte superiore alla media.



---

## 📊 Business Intelligence (Power BI Integration)
I risultati dell'analisi Python sono stati importati in Power BI per creare una dashboard interattiva:
* **Segment Distribution:** Visualizzazione della dimensione di ogni gruppo (Champions vs Hibernating).
* **Monetary vs Frequency:** Scatter plot per identificare visivamente i cluster di valore.
* **Trend Analysis:** Analisi temporale degli acquisti per capire i periodi di picco.



---

## 🚀 Repository Content
* `/notebooks`: Jupyter Notebook con il codice Python per il calcolo RFM e scoring.
* `/data`: Dataset pulito pronto per la visualizzazione.
* `/reports`: Screenshot e file `.pbix` della dashboard finale.


