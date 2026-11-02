# Istituzioni di Algebra – Trattato e Dispense Ufficiali in LaTeX
**Corso di Laurea Triennale in Informatica – Università degli Studi di Napoli Federico II**  
**Docente:** Prof. Giovanni Cutolo (Dipartimento di Matematica e Applicazioni "Renato Caccioppoli")  
**A cura di:** Fagghino ([UniNa-Fagghino](https://github.com/UniNa-Fagghino))  
**Anno Accademico:** 2025/2026  

---

## 📖 Panoramica del Progetto

Questo progetto raccoglie e unifica in un'unica opera organica, rigorosa e completa in **LaTeX** l'intero patrimonio didattico necessario per preparare con il massimo dei voti l'esame di **Algebra** (Canale 2 / U6282).

L'opera è stata redatta sintetizzando e integrando:
1. Le **19 monografie ufficiali del DMA** redatte dal Prof. Cutolo.
2. I **registri giorno per giorno delle lezioni** con tutti gli argomenti ed esercizi spiegati in aula.
3. Le **prove d'esame ufficiali** (2001--2026) e le soluzioni commentate.
4. Il **censimento integrale delle domande d'orale** e dei tranelli logici più frequenti.

---

## 📁 Struttura Modulare dei File

```text
Dispense_Algebra_Cutolo/
├── main.tex                               (File principale di inclusione e frontespizio)
├── preamble.tex                           (Configurazione pacchetti, colori, tcolorbox, macro)
│
├── capitoli/
│   ├── 00_prefazione.tex                  (Metodologia, convenzioni e guida all'esame)
│   ├── 01_logica_e_fondamenti.tex         (Calcolo proposizionale, predicati, quantificatori)
│   ├── 02_insiemi_e_combinatoria.tex      (Insiemi, buon ordinamento, induzione, combinatoria)
│   ├── 03_relazioni_e_applicazioni.tex    (Equivalenze, partizioni, sezioni/retrazioni, omomorfismo)
│   ├── 04_relazioni_d_ordine_e_reticoli.tex (Poset, Hasse, reticoli, Birkhoff, strutture booleane)
│   ├── 05_aritmetica_modulare_e_diofantee.tex (Divisione euclidea, Bézout, congruenze, CRT, Eulero)
│   ├── 06_strutture_algebriche.tex        (Semigruppi, monoidi, gruppi, Lagrange, anelli, campi)
│   ├── 07_anelli_di_polinomi.tex          (K[x], divisione, Ruffini, irriducibilità, quozienti)
│   ├── 08_teoria_dei_grafi.tex            (Handshaking, alberi, bipartiti, euleriani, isomorfismi)
│   ├── 09_guida_strategica_esame_e_orale.tex (Le 10 domande killer di Cutolo, vademecum)
│   └── 10_raccolta_esercizi_svolti_tipo.tex (Eserciziario risolto passo-passo tipo-esame)
│
└── README.md                              (Questa guida)
```

---

## 🛠️ Come Compilare il Documento in PDF

### 1. Compilazione Automatica su GitHub (Consigliata)
Il repository include una **GitHub Action** (`.github/workflows/compile-latex.yml`):
- A ogni `git push` sul branch `main`, GitHub avvia una macchina virtuale Ubuntu con TeX Live completo.
- Il file `main.tex` viene compilato automaticamente in `Istituzioni_di_Algebra_Cutolo_UniNa.pdf`.
- Il PDF generato è scaricabile direttamente dalla sezione **Actions** (sotto gli *Artifacts*) di GitHub.

### 2. Compilazione su Overleaf
1. Scaricare o clonare la cartella `Dispense_Algebra_Cutolo/`.
2. Caricare i file su [Overleaf](https://www.overleaf.com/) creando un nuovo progetto.
3. Selezionare come file principale `main.tex` e compilare con motore **pdfLaTeX** standard.

### 3. Compilazione Locale (TeX Live / MiKTeX)
Se disponi di una distribuzione TeX locale sul tuo computer:
```bash
cd Dispense_Algebra_Cutolo
pdflatex main.tex
pdflatex main.tex  # Seconda passata per indice e collegamenti ipertestuali
```
