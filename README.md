# PostureRecognition

**link datasets** 
https://physionet.org/content/pmd/1.0.0/


**Experiment_1 analysis**
1. Prendo 1 soggetto (Età, Peso, Altezza)
2. Lo facciamo stendere in una delle 17 possibili posizioni
3. Rileviamo la pressione esercitata sulla stuoia (Mat 32x64 e.g 0 dove non c'è pressione, valore alto dove ce nè tanta)
4. Dobbiamo riconoscere il soggetto in tale posizione

**Experiment_2 analysis**
1. Solo alcuni soggetti di Experiment_1 (Età, Peso, Altezza)
2. Lo facciamo dormire in un materasso ad aria o in uno normale in tre possibili posizioni (Supino, destra, sinistra)
3. Rileviamo la pressione esercitata sui materassi (Mat 27x64)
4. Dobbiamo riconoscere la posizione


**Idee**
1. Preprocessing: Padding, PCA, Clustering(K-means da decide numero di cluster e magnitude del cluster) 
2. Creare Dataset con intensità cluster + posizione, altezza e peso, postura e soggetto. 
3. Rete neurale, CNN per classificazione + eventuali stronzate di Rossi.
4. Demo