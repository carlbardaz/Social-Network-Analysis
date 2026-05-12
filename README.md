# ✈️ Global Flight Network Analysis
### *Un'indagine sulla connettività, resilienza e diffusione nel trasporto aereo mondiale*

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg?logo=python&logoColor=white)](https://www.python.org/)
[![NetworkX](https://img.shields.io/badge/Library-NetworkX-orange.svg)]()
[![Analysis](https://img.shields.io/badge/Focus-Network%20Resilience-red.svg)]()

> [cite_start]**Progetto di Social Network Analysis** > Analisi approfondita del dataset OpenFlights per comprendere le dinamiche strutturali del traffico aereo globale, la sua vulnerabilità agli attacchi e i processi di diffusione epidemica. 

---

## 🧐 Panoramica del Progetto
[cite_start]Il progetto esplora la rete globale composta da **3.186 aeroporti** (nodi) e **17.297 rotte** (archi).  [cite_start]L'obiettivo è mappare l'infrastruttura del volo mondiale per identificare gli snodi critici e valutare come la rete reagisce a guasti o attacchi mirati. 

### 🔍 Aree di Analisi
1.  [cite_start]**Network Crawling & Topology:** Costruzione della rete e analisi delle proprietà strutturali (distribuzione dei gradi, diametro, coefficiente di clustering). [cite: 3, 5]
2.  [cite_start]**Community Detection:** Identificazione di gruppi di aeroporti densamente collegati per scoprire la struttura gerarchica del traffico. [cite: 3, 5]
3.  [cite_start]**Network Resilience:** Simulazione di attacchi ai nodi (casuali vs mirati) per misurare la robustezza della connettività globale. [cite: 3, 4]
4.  [cite_start]**Spreading Models:** Modellazione della diffusione (es. virus o informazioni) attraverso la rete utilizzando modelli SIR/SIS. [cite: 3, 6]

---

## 🛠️ Struttura del Repository
Il progetto è suddiviso in moduli focalizzati su aspetti specifici dell'analisi:

| File | Descrizione |
| :--- | :--- |
| `SNA Project - Parts 1, 2 and 4.ipynb` | [cite_start]Analisi topologica, centralità e rilevamento delle comunità. [cite: 5] |
| `Network Resilience.ipynb` | [cite_start]Studio della tolleranza ai guasti e robustezza della rete. [cite: 4] |
| `Spreading 2.ipynb` | [cite_start]Simulazioni di processi di diffusione e dinamiche di contagio. [cite: 6] |
| `airports.dat` / `routes.dat` | [cite_start]Dataset grezzi estratti da OpenFlights. [cite: 1, 2] |
| `SNA_Project_Report.pdf` | [cite_start]Report dettagliato con metodologia e conclusioni scientifiche.  |

---

## 🚀 Risultati Chiave

* [cite_start]**Topologia:** La rete dei voli segue una distribuzione "scale-free", dove pochi hub (come Francoforte, Pechino o Istanbul) detengono la maggior parte delle connessioni. 
* [cite_start]**Resilienza:** La rete è estremamente robusta contro i guasti casuali, ma altamente vulnerabile ad attacchi mirati sugli hub con il più alto grado di centralità. [cite: 3, 4]
* [cite_start]**Diffusione:** Grazie alla struttura "small-world", un processo di diffusione può raggiungere gran parte del mondo in pochissimi passaggi temporali. [cite: 3, 6]

---

## 🧰 Requisiti tecnici
Per eseguire i notebook è necessario l'ambiente Python con le seguenti librerie:
```python
pip install networkx numpy pandas matplotlib scipy