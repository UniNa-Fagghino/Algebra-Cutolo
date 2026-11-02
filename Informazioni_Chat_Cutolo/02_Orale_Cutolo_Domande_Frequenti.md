# Orale con il Prof. Cutolo: Modalità e Domande Frequenti
**Corso di Algebra – Corso di Laurea in Informatica – Università degli Studi di Napoli Federico II**

---

## 1. Come si Svolge l'Orale con Cutolo: Atmosfera e Stile

Dalle testimonianze dirette degli studenti nelle chat emergono indicazioni chiare sullo stile d'esame del docente:
* **Massimo rigore formale:** Il Prof. Cutolo esige precisione assoluta sul piano linguistico e notazionale. Formulare una definizione "a parole proprie" in modo impreciso è uno dei motivi principali di bocciatura.
* **Dimostrazioni richieste:** A differenza di altri docenti che talvolta si limitano agli enunciati, Cutolo **chiede esplicitamente le dimostrazioni dei teoremi** presenti nelle dispense e spiegati a lezione.
* **Attenzione ai dettagli:** Gli studenti sottolineano che domande apparentemente marginali (es. una proprietà specifica di un'operazione o un lemma citato a lezione) possono essere determinanti per il superamento dell'orale.
* **Correttezza dello scritto:** Durante l'orale il professore può chiedere di discutere o giustificare passaggi svolti durante la prova scritta.

---

## 2. Domande Specifiche Registrate dalle Chat per l'Orale di Cutolo

Ecco le domande e i temi specifici segnalati direttamente dagli studenti dopo aver sostenuto l'orale con Cutolo:

### A. Reticoli e Insiemi Parzialmente Ordinati
1. **Reticoli distributivi:** Definizione formale, condizioni equivalenti di distributività e controesempi classici (reticolo pentagonale $N_5$ e reticolo a diamante $M_3$).
2. **Proprietà di estremo inferiore ($\inf$) ed estremo superiore ($\sup$):**
   * Definizione formale con quantificatori logici.
   * **Dimostrazione dell'associatività di $\inf$:** Dimostrare che in un reticolo $(L, \le)$ si ha $a \wedge (b \wedge c) = (a \wedge b) \wedge c$.
3. **Complementi nei reticoli:** Definizione di elemento complementato e unicità del complemento nei reticoli distributivi.

### B. Polinomi e Anelli
1. **Regola di addizione dei gradi:**
   * Enunciato formale: $\deg(fg) = \deg(f) + \deg(g)$.
   * Condizioni affinché valga (anello commutativo unitario integro vs presenza di divisori dello zero).
2. **Cancellabilità nei polinomi:**
   * Teorema: Se il coefficiente direttore di $f$ è cancellabile in $R$, allora $f$ è un elemento cancellabile in $R[x]$. Dimostrazione completa.
3. **Teorema di Ruffini:**
   * Attenzione: Cutolo richiede l'enunciato esatto dato a lezione, distinguendo nettamente il teorema vero e proprio dai suoi corollari sul numero massimo di radici di un polinomio.

### C. Strutture Algebriche e Monoidi
1. **Elementi neutri unilaterali:**
   * È possibile avere due elementi neutri a sinistra distinti in un magma/semigruppo? **Sì**, purché non esista un elemento neutro a destra.
   * Dimostrazione: Se una struttura possiede un elemento neutro a sinistra $e_s$ e un elemento neutro a destra $e_d$, allora necessariamente $e_s = e_d$, e tale elemento neutro globale è unico.
2. **Definizione di Monoide:** Condizioni necessarie (associatività + esistenza dell'elemento neutro bilaterale).

### D. Insiemi, Applicazioni e Relazioni
1. **Convenzione fondamentale su $\mathbb{N}$:**
   * Nelle lezioni e nelle dispense di Cutolo, **lo zero è incluso nei numeri naturali:** $0 \in \mathbb{N}$. Considerarlo escluso negli esercizi o nelle definizioni formali viene considerato errore.
2. **Sottrazione indotta e riduzioni:**
   * Perché non esiste la sottrazione indotta in $\mathbb{N}$? Spiegazione tramite la restrizione/riduzione di un'applicazione: $\mathbb{N} \times \mathbb{N}$ non è stabile rispetto alla sottrazione di $\mathbb{Z}$.
3. **Partizioni e Relazioni d'Equivalenza:**
   * Teorema fondamentale delle relazioni di equivalenza: corrispondenza biunivoca tra le partizioni di un insieme $A$ e le relazioni di equivalenza su $A$.
   * Costruzione rigorosa dell'insieme quoziente $A/\rho$ e proprietà della proiezione canonica $\pi: A \to A/\rho$.
4. **Principio di Induzione Matematica:**
   * Prima forma del principio di induzione, seconda forma (induzione forte o completa).
   * Equivalenza con il Principio del Buon Ordinamento di $\mathbb{N}$.

---

## 3. Riepilogo per Superare l'Orale
* Conoscere a memoria e con padronanza formale tutte le **definizioni matematiche** (con quantificatori $\forall, \exists$).
* Preparare le dimostrazioni chiave presenti nei file della cartella `02_Dispense_e_Teoria\Monografie_DMA_Cutolo` (associatività $\inf/\sup$, cancellabilità polinomi, Bézout, induzione).
* Studiare rigorosamente dalle **dispense e note di Cutolo** (cartella `02_Dispense_e_Teoria`), in quanto riflettono la sua terminologia e le sue predilezioni metodologiche.

