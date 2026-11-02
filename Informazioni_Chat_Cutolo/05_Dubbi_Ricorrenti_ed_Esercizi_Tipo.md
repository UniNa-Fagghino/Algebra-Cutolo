# Dubbi Ricorrenti ed Esercizi-Tipo Estratti dalle Chat
**Corso di Algebra – Corso di Laurea in Informatica – Università degli Studi di Napoli Federico II**

---

Dall'analisi delle oltre 4.000 interazioni e richieste di chiarimento nel topic di supporto, sono stati isolati i dubbi teorici e pratici più frequenti che gli studenti incontrano nello svolgimento delle tracce e nella preparazione dell'esame.

---

## 1. Applicazioni, Corrispondenze e Cardinalità

### Calcolo del numero di corrispondenze e applicazioni
* **Formula per le corrispondenze:** Una corrispondenza tra due insiemi finiti $A$ e $B$ è un qualsiasi sottoinsieme del prodotto cartesiano $A \times B$. Il numero totale di corrispondenze è quindi:
  $$\text{Numero corrispondenze} = |\mathcal{P}(A \times B)| = 2^{|A| \cdot |B|}$$
* **Formula per le applicazioni (funzioni):** Un'applicazione assegna a ciascun elemento di $A$ esattamente un elemento di $B$:
  $$\text{Numero applicazioni} = |B|^{|A|}$$

### Immagine diretta e Controimmagine (Anti-immagine)
* Uno dei dubbi più dibattuti riguarda il calcolo dell'anti-immagine $f^{-1}(Y)$:
  * Non confondere la controimmagine $f^{-1}(Y)$ (che esiste **sempre** per qualsiasi funzione, associando ad un sottoinsieme del codominio gli elementi del dominio che vi mappano) con l'applicazione inversa $f^{-1}$ (che esiste **solo se $f$ è biettiva**).
* Errore comune: testare l'iniettività ponendo $f(x_1) = f(x_2) \implies x_1 = x_2$ senza verificare attentamente le condizioni di dominio (ad esempio su domini a tratti o con funzioni a valori modulo $n$).

---

## 2. Operazioni Binarie e Tavole di Cayley

### Elementi neutri a sinistra e a destra (Quesito Cutolo)
* **Dubbio emerso in chat:** *"Perché Cutolo dice che possono esistere due elementi neutri a sinistra distinti?"*
* **Chiarimento teorico:** In un magma o semigruppo $(S, *)$, un elemento $e_1$ è neutro a sinistra se $\forall x \in S, \; e_1 * x = x$.
  * È perfettamente possibile avere **più elementi neutri a sinistra distinti**, purché **non esista alcun elemento neutro a destra**.
  * Esempio classico: l'operazione proiettiva a destra definita da $x * y = y$. In questa struttura, **ogni elemento** è neutro a sinistra!
  * **Teorema fondamentale:** Se in una struttura esiste **almeno un neutro a sinistra $e_s$** e **almeno un neutro a destra $e_d$**, allora:
    $$e_s = e_s * e_d = e_d$$
    Quindi coincidono necessariamente ed esiste un unico elemento neutro bilaterale.

### Tavole di Cayley su Insieme delle Parti
* Quando l'operazione è definita su $\mathcal{P}(A)$ (es. unione, intersezione o differenza simmetrica), la tavola di Cayley richiede di elencare tutti i $2^{|A|}$ sottoinsiemi come righe e colonne.

---

## 3. Relazioni di Equivalenza e Insiemi Quoziente

* **Definizione di partizione:** Una famiglia di sottoinsiemi non vuoti, a due a due disgiunti, la cui unione coincide con l'intero insieme.
* **Proiezione canonica $\pi: A \to A/\rho$:**
  * È sempre un'applicazione **suriettiva**.
  * È iniettiva se e solo se la relazione di equivalenza è la relazione diagonale (identità).
* **Compatibilità di un'operazione con una relazione di equivalenza:**
  * Affinché un'operazione $*$ su $A$ sia ben definita sull'insieme quoziente $A/\rho$ ponendo $[a] \star [b] = [a * b]$, l'operazione deve essere compatibile con $\rho$:
    $$\forall a, a', b, b' \in A: \quad a \mathrel{\rho} a' \land b \mathrel{\rho} b' \implies (a * b) \mathrel{\rho} (a' * b')$$

---

## 4. Aritmetica Modulare e Teorema Cinese del Resto

### Risoluzione delle equazioni congruenziali lineari
Data l'equazione $ax \equiv b \pmod m$:
1. Si calcola $d = \operatorname{MCD}(a, m)$ tramite l'algoritmo euclideo.
2. **Criterio di esistenza:** La congruenza ha soluzioni se e solo se $d$ divide $b$ ($d \mid b$).
3. Se $d \mid b$, l'equazione ammette **esattamente $d$ soluzioni distinte modulo $m$**.
4. Si determina una soluzione particolare $x_0$ tramite i coefficienti di Bézout $as + mt = d$.
5. Le $d$ soluzioni non congruenti tra loro sono date da:
   $$x_k = x_0 + k \cdot \frac{m}{d}, \quad \text{per } k = 0, 1, \dots, d-1$$

---

## 5. Teoria dei Reticoli e Diagrammi di Hasse

### Come verificare se un insieme ordinato è un reticolo
1. Disegnare correttamente il **Diagramma di Hasse**, verificando la transitività e la proprietà antisimmetrica.
2. Un insieme parzialmente ordinato è un reticolo se **ogni coppia di elementi** ammette sia l'estremo inferiore ($a \wedge b = \inf\{a, b\}$) che l'estremo superiore ($a \vee b = \sup\{a, b\}$).
3. **Controllo di distributività:**
   * Un reticolo non è distributivo se e solo se contiene un sottoreticolo isomorfo al reticolo pentagonale $N_5$ o al reticolo a diamante $M_3$.
4. **Elementi complementati:**
   * Un elemento $b$ è complemento di $a$ se $a \wedge b = 0$ (minimo) e $a \vee b = 1$ (massimo).
   * In un reticolo distributivo, il complemento (se esiste) è **unico**.

