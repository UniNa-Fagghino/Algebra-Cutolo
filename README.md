# Algebra (Prof. Giovanni Cutolo) – Archivio e Guida all'Esame
**Corso di Laurea in Informatica – Università degli Studi di Napoli Federico II**

Raccolta strutturata, verificata e completa di materiali didattici, prove scritte d'esame, appunti manoscritti, dispense ufficiali e guide informative per la preparazione dell'esame di **Algebra** con il **Prof. Giovanni Cutolo**.

---

## 📌 Indice dei Contenuti

1. [Struttura del Repository](#-struttura-del-repository)
   * [Dispense_Algebra_Cutolo (Trattato Ufficiale in LaTeX)](#1-dispense_algebra_cutolo-trattato-ufficiale-in-latex)
   * [Materiale_Sito_Ufficiale_Cutolo](#2-materiale_sito_ufficiale_cutolo)
   * [Materiale_Prof_Cutolo](#3-materiale_prof_cutolo)
   * [Informazioni_Chat_Cutolo](#4-informazioni_chat_cutolo)
2. [Avvertenza su Fonti, Privacy e Riferimenti Personali](#-avvertenza-su-fonti-privacy-e-riferimenti-personali)
3. [Disclaimer sul Copyright e Proprietà Intellettuale](#-disclaimer-sul-copyright-e-proprietà-intellettuale)
4. [Istruzioni per la Clonazione (Git LFS)](#-istruzioni-per-la-clonazione-git-lfs)
5. [Autore & Contatti](#-autore--contatti)

---

## 📁 Struttura del Repository

### 1. `Dispense_Algebra_Cutolo/` (Trattato Ufficiale in LaTeX)
L'opera organica e modulare redatta in **LaTeX**, concepita come la dispensa definitiva per lo studio dell'intero programma d'esame. Include il codice sorgente suddiviso in 10 capitoli tematici, il preambolo stilistico con box decorati (`tcolorbox`), diagrammi vettoriali (`tikz`), tutte le dimostrazioni formali e una **GitHub Action** per la compilazione automatica del PDF ad ogni commit:

* [**`main.tex`**](Dispense_Algebra_Cutolo/main.tex): Documento principale, frontespizio e indice generale.
* [**`preamble.tex`**](Dispense_Algebra_Cutolo/preamble.tex): Pacchetti matematici, macro ufficiali di Cutolo ($\antivecf, \vecf, \P, \ds$), ambienti per teoremi, definizioni ed avvisi d'orale.
* **`capitoli/`**:
  * `00_prefazione.tex`: Metodologia di studio, convenzioni e criteri di valutazione.
  * `01_logica_e_fondamenti.tex`: Calcolo proposizionale, connettivi completi, tavole di verità, tautologie, calcolo dei predicati e quantificatori.
  * `02_insiemi_e_combinatoria.tex`: Teoria ingenua degli insiemi, buon ordinamento di $\N$, principio di induzione, calcolo combinatorio e binomio di Newton.
  * `03_relazioni_e_applicazioni.tex`: Relazioni d'equivalenza, partizioni, proiezioni canoniche, sezioni e retrazioni, Teorema di omomorfismo per insiemi e cardinalità (Cantor).
  * `04_relazioni_d_ordine_e_reticoli.tex`: Poset, diagrammi di Hasse, estremi, reticoli algebrici e d'ordine, criterio di Birkhoff ($N_5, M_3$), algebre di Boole e Teorema di Stone.
  * `05_aritmetica_modulare_e_diofantee.tex`: Divisione euclidea, algoritmo esteso di Bézout a tabella, congruenze in $\Z_m$, Teorema Cinese del Resto (CRT), funzione $\varphi$ di Eulero e teoremi di Eulero-Fermat.
  * `06_strutture_algebriche.tex`: Operazioni binarie, elementi neutri/simmetrici/cancellabili, semigruppi, monoidi, gruppi, Teorema di Lagrange, omomorfismi e anelli/campi.
  * `07_anelli_di_polinomi.tex`: Polinomi $K[x]$, divisione euclidea, Teorema di Ruffini, criteri di irriducibilità, ideali e campi quoziente $K[x]/(f(x))$.
  * `08_teoria_dei_grafi.tex`: Grafi non orientati, Handshaking Lemma, alberi e loro caratterizzazioni, grafi bipartiti (Kőnig), cammini euleriani (Eulero) e isomorfismi.
  * `09_guida_strategica_esame_e_orale.tex`: Le 10 domande "killer" di Cutolo all'orale, vademecum del rigore linguistico e gestione dei tempi dello scritto.
  * `10_raccolta_esercizi_svolti_tipo.tex`: Eserciziario risolto passo per passo con commento metodologico su tutti i tipi d'esame.
* [**`README.md`**](Dispense_Algebra_Cutolo/README.md): Guida alla consultazione e istruzioni per la compilazione (GitHub Actions, Overleaf o locale).

---

### 2. `Materiale_Sito_Ufficiale_Cutolo/`
Archivio integrale, speculare e verificato scaricato direttamente dal [sito ufficiale del docente](http://www.dma.unina.it/cutolo/didattica/AlgInfo/) (D.M.A. UniNa) per il corso di Algebra (LT Informatica - Canale 2 / U6282):

* **`01_Note_e_Dispense_Teoriche/`**: 19 monografie e note didattiche di teoria del docente (logica, calcolo combinatorio aggiornato 2026, partizioni ed equivalenze, algoritmo euclideo, polinomi ed esercizi svolti, strutture booleane, omomorfismi per insiemi, cancellabilità, ecc.).
* **`02_Esercizi_Ufficiali/`**: 5 fascicoli di esercizi tematici per l'esame (logica, insiemi e aritmetica modulare/diofantea, relazioni d'ordine e reticoli, teoria dei grafi, polinomi e strutture algebriche).
* **`03_Prove_Scritte_Esami/`**: Raccolta completa di 177 prove scritte ufficiali suddivisa in:
  * **`Recenti_2012_2026/`**: 114 tracce d'esame in PDF dal 2012 a settembre 2026.
  * **`Archivio_Storico_2001_2011/`**: 63 tracce d'esame storiche in PDF dal 2001 al 2011.
* **`04_Programmi_e_Registri/`**: Programmi ufficiali d'esame (recenti e storici) e il **registro integrale giorno per giorno delle lezioni ed esercizi** dell'anno accademico 2025/2026.

---

### 3. `Materiale_Prof_Cutolo/`
Raccoglie esclusivamente le risorse riferite al corso del Prof. Cutolo (filtrando i materiali di altri docenti come Celentani e Brescia):

* **`01_Appunti/`**: Appunti delle lezioni frontali in LaTeX (lezioni 2, 3, 4 e 5), appunti integrali del corso (raccolte A. Marasco, G. Fiorentino & G. Amato, appunti 2022/2025) e note aggiornate con prove svolte fino al 2025 (`unina_algebra_notes.pdf`).
* **`02_Dispense_e_Teoria/`**: Dispense generali del corso (versioni Settembre 2025, Febbraio 2025, Ottobre 2024), documenti ufficiali UNINA e la sottocartella **`Monografie_DMA_Cutolo/`** con i 32 fascicoli tematici del sito DMA (*algoritmo euclideo, aritmetica modulare, cancellabilità, combinatoria, connettivi, partizioni ed equivalenze, polinomi, reticoli e strutture booleane, principio di induzione*).
* **`03_Libri_Consigliati/`**: Testi di riferimento raccomandati dal docente (*A. Facchini – Algebra e Matematica Discreta*; *Leonesi, Toffalori – Un Invito all'Algebra*).
* **`04_Esami_e_Prove_Scritte/`**:
  * **`Archivio_Tracce_Scritte_Cutolo/`**: Tutte le tracce d'esame e prove intercorso dal 2012 al 2023, con la sottocartella `Tracce_Per_Data` per consultazione rapida per sessione.
  * **`Soluzioni_e_Compiti_Svolti/`**: Soluzioni ufficiali delle prove scritte, compiti d'esame svolti e commentati dagli studenti (2023 e 2025) e 32 svolgimenti in formato nativo Microsoft Journal (`.ink`) nella cartella `Prove_Svolte_Journal_Microsoft/`.

---

### 4. `Informazioni_Chat_Cutolo/`
Guide strategiche ricavate dall'analisi di oltre 4.400 messaggi ed esperienze dirette degli studenti della Federico II:

* [**`01_Modalita_Esame_e_Correzione.md`**](Informazioni_Chat_Cutolo/01_Modalita_Esame_e_Correzione.md): Ruolo di Cutolo come autore unico dello scritto per tutti i canali, regolamento Nuovo Ordinamento (2 ore, 2 esercizi in meno, alleggerimento su grafi e polinomi), correzione rapida (24-48 ore) e calendario orali.
* [**`02_Orale_Cutolo_Domande_Frequenti.md`**](Informazioni_Chat_Cutolo/02_Orale_Cutolo_Domande_Frequenti.md): Svolgimento dell'orale, importanza delle dimostrazioni formali, rigore terminologico e domande ricorrenti (reticoli distributivi, associatività di $\inf$, cancellabilità polinomi, Ruffini, convenzione $0 \in \mathbb{N}$).
* [**`03_Consigli_di_Studio_e_Preparazione.md`**](Informazioni_Chat_Cutolo/03_Consigli_di_Studio_e_Preparazione.md): Metodologia consigliata da ex studenti, fruizione delle videolezioni (prima mezz'ora di esercizi), ricevimenti e preparazione mirata scritto vs orale.
* [**`04_Link_e_Risorse_Ufficiali.md`**](Informazioni_Chat_Cutolo/04_Link_e_Risorse_Ufficiali.md): Pagine istituzionali DMA Cutolo (compiti, registro, tutorato), playlist YouTube ufficiali delle lezioni registrate e repository GitHub di supporto.
* [**`05_Dubbi_Ricorrenti_ed_Esercizi_Tipo.md`**](Informazioni_Chat_Cutolo/05_Dubbi_Ricorrenti_ed_Esercizi_Tipo.md): Risoluzione dei dubbi e degli errori più frequenti (corrispondenze vs applicazioni, controimmagini, elementi neutri unilaterali distinti, compatibilità relazioni d'equivalenza, congruenze con Bézout, reticoli e Hasse).

---

## ⚠️ Avvertenza su Fonti, Privacy e Riferimenti Personali

> [!IMPORTANT]
> I documenti, gli appunti, le tracce e le indicazioni presenti in questo repository derivano da una selezione e riorganizzazione delle risorse liberamente condivise tra studenti all'interno dei gruppi Telegram universitari (*Chat - Unina Files* e *Chat - Unina Help*).
> 
> Per questa ragione, **all'interno di alcuni file (ad esempio negli appunti manoscritti, nelle relazioni d'esame o nelle intestazioni di compiti svolti) potrebbero figurare riferimenti a persone fisiche, nomi, firme o crediti di studenti** che hanno originariamente predisposto e condiviso i propri appunti a beneficio della comunità accademica.
> 
> * L'intento della presente raccolta è **esclusivamente didattico, di studio collaborativo e di orientamento**, privo di qualunque finalità commerciale.
> * A tutela della riservatezza, le chat testuali complete e le conversazioni integrali **sono state escluse dal repository** e non vengono in alcun modo pubblicate.
> * **Qualora un autore, studente o interessato desideri la rettifica, l'anonimizzazione o la rimozione di un proprio appunto, elaborato o riferimento nominativo**, è invitato ad aprire una Issue su GitHub o a contattare il curatore del repository (**Fagghino**): la modifica o cancellazione richiesta verrà effettuata tempestivamente.

---

## ⚖️ Disclaimer sul Copyright e Proprietà Intellettuale

* I testi delle prove d'esame e le dispense didattiche ufficiali sono di proprietà del **Prof. Giovanni Cutolo** e del **Dipartimento di Matematica ed Applicazioni "R. Caccioppoli" dell'Università degli Studi di Napoli Federico II**.
* I libri di testo indicati rimangono di esclusiva proprietà dei rispettivi autori ed editori e sono menzionati a puro scopo bibliografico per i programmi d'esame dell'Ateneo.
* Gli appunti studenteschi appartengono ai rispettivi estensori e sono distribuiti a solo scopo di consultazione personale tra studenti.

---

## 🚀 Istruzioni per la Clonazione (Git LFS)

Poiché alcuni file di appunti manoscritti superano i 100 MB (limite massimo di GitHub per i singoli file), questo repository utilizza **Git Large File Storage (Git LFS)** per il tracciamento dei file binari e dei PDF di grandi dimensioni:

```bash
# 1. Assicurarsi di aver installato Git LFS (da eseguire una tantum)
git lfs install

# 2. Clonare il repository normalmente
git clone https://github.com/UniNa-Fagghino/Algebra-Cutolo.git
cd Algebra-Cutolo

# 3. Qualora i file di grandi dimensioni non venissero scaricati automaticamente:
git lfs pull
```

---

## 👤 Autore & Contatti

* **Curatore:** **Fagghino** ([@Fagghino](https://github.com/Fagghino))
* **Organizzazione:** [UniNa-Fagghino](https://github.com/UniNa-Fagghino)
