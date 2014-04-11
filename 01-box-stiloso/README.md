# Esercizio

Scopo dell'esercizio e' ottenere l'aspetto grafico che si vede nell'immagine output-stiloso.png.  NON TOCCARE IL FILE HTML, tutto quello che devi fare e' modificare il file style.css.


0. Scegliere uno stile tipografico
  * Fonts: Tahoma, Arial, sans-serif;
  * Dimensioni: altezza del font 12px, altezza della riga 18px
  * Per l'*aside*: corsivo (italic) e font più piccolo (smaller)
  * Per l'*h3*: font più grande del 50%


1. Scegliere i colori
  * Per il body, background-color: white; color: #706C6E
  * Per i link: (elemento a) color: #A1805C
  * Per lo aside: background-color: rgb(85%, 85%, 100%)
  * Per l'article: background-color: rgb(85%, 100%, 85%)

2. Scegliere le dimensioni
  * La div che ha classe "content" deve essere larga 240px

3. Posizionare l'aside a destra e l'article a sinistra
  * Applicare float: left a entrambi
  * La larghezza di article e aside deve essere di 120px





4. Applichiamo una cornice a tutto il div class="content"
  * border: 2px dashed rgb(224, 226, 230);
  * Oooops! il float "esce" dal suo contenitore! Per correggere il problema, mettiamo float="left" anche al content!


5. Diamo un po' di respiro:
  * Diamo ad article e aside 12px di margine
    * PERÒ il margine destro di article deve essere 6
    * e il margine sinistro di aside deve essere 6
  * Di conseguenza al width di article e aside diventa 120-12-6 (e' semplice aritmetica... calcola che la div che contiene article e aside e' larga 240.  Abbiamo inserito due margini di 12px e due di 6px.  Fai il conto di quanti pixel restano per article e aside.)

7. Stilizziamo il menu.
  * Lo sfondo del menu deve essere grigio rgb(224, 226, 230)
  * I link devono essere in grassetto (font-weight: bold)
  * I link del menu non devono essere sottolineati (text-decoration: none).  Nota che **i link dentro al testo** devono restare sottolineati.
  * I link devono essere in reverse quando ci passa sopra il puntatore.  In reverse significa che il colore dello sfondo diventa il colore del testo, e viceversa.

8. Il menu deve essere **orizzontale**.  Qui bisogna usare un po' di trucchetti, di cui il piu' importante e' dare agli elementi li la proprieta' display: inline-block.  Poi bisogna togliere il "pallino" con la proprieta' list-item.

Per imparare il "trucco" del CSS occorre fare un po' di esperimenti.  Alcune cose non sono ovvie, ma si capiscono facendo un po' di esperimenti.  Per le informazioni che non ho dato, utilizza internet.

