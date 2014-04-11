# Esercizio

Scopo dell'esercizio e' ottenere l'aspetto grafico che si vede nell'immagine output-stiloso.png.  NON TOCCARE IL FILE HTML, tutto quello che devi fare e' modificare il file style.css.


Esegui l'esercizio secondo i passi che seguono.  Devi modificare solo il file style.css, non il file html.  **Importante**: dopo ogni minima modifica al CSS, ricarica la pagina nel browser per osservare l'effetto.

0. Copia in una directory il file index.html.  Crea un file vuoto &ldquo;style.css&rdquo;.

1. Metti una prima sezione nel file style.css copiando il frammento che segue.  Apri index.html nel browser e osserva gli sfondi colorati.  Questi serviranno per aiutarci a visualizzare questi due elementi nel corso dello sviluppo.  Quando avremo ottenuto il risultato desiderato, la sezione Debug la commenteremo.

<pre>
/* Debug */
aside {
	background-color: rgb(85%, 85%, 100%);
}
article {
	background-color: rgb(85%, 100%, 85%)
}
</pre>


3. Apri una nuova sezione nel file CSS, intitolata `/* Typography and colors */` Scegli uno stile tipografico.  Applica le seguenti proprietà:

    * Per tutto il documento: font-family: Tahoma, Arial, sans-serif;
    * Dimensioni: altezza del font 12px, altezza della riga 18px
    * Per l'*aside*: corsivo (italic) e font più piccolo (smaller)
    * Per l'*h3*: font più grande del 50%

1. Scegli i colori
    * Per il body, background-color: white; color: #706C6E
    * Per i link (elemento `a`): color: #A1805C
    * Per lo aside: background-color: rgb(85%, 85%, 100%)
    * Per l'article: background-color: rgb(85%, 100%, 85%)

2. Apri una nuova sezione nel file CSS, `/* Page layout */` Scegli le dimensioni.
    * La div che ha classe "content" deve essere larga 240px
    * La larghezza di article e aside deve essere di 120px
    * Applica float: left sia ad article che ad aside.

3. Applichiamo una cornice a tutto il div che ha class="content"
    * border: 2px dashed rgb(224, 226, 230);
    * Oooops! il div .content ha altezza nulla, perché i float che contiene strabordano! Per correggere il problema, mettiamo float="left" anche al .content!

5. Diamo un po' di respiro:
    * Diamo ad article e aside 12px di margine
        * PERÒ il margine destro di article deve essere 6
        * e il margine sinistro di aside deve essere 6
    * Di conseguenza il width di article e aside deve essere ridotto di 18px (12+6), altrimenti non possono restare affiancati

7. Stilizziamo il menu.  Apri una nuova sezione `/* Navigation menu */`
    * Lo sfondo del menu deve essere grigio rgb(224, 226, 230)
    * I link (elementi `a`) devono essere in grassetto (font-weight: bold)
    * I link non devono essere sottolineati (text-decoration: none).  Ma attenzione: solo i link dentro al menu di navigazione devono perdere la sottolineanura! Gli altri link devono conservarla.  Usa i contextual selectors.
    * Quando passo con il puntatore sopra le voci di menu, devono evidenziarsi in reverse: scambiare il background-color con il color.  Per ottenere questo effetto, occorre sfruttare la pseudo-classe `a:hover`


8. Il menu deve essere **orizzontale**.  Per ottenere questo effetto occorre applicare diverse proprietà
    * Applicare a li la proprietà display: block (spariscono i pallini)
    * Applicare a ul la proprietà padding: 0
    * Applicare a li le proprietà
        * display: block
        * float: left;
        * width: 80px (cioè 240 / 3)
        * text-align: left
    * Per fare in modo che l'elemento ul contenga tutti i suoi li, dobbiamo applicare anche a lui la proprietà display: block.

9. A questo punto, se allarghiamo la finestra, possiamo vedere che il .content si allinea a destra del menu!  E' perché sia il menu che il .content sono fluttuati a sinistra.  Per evitare questo effetto applichiamo la proprietà clear: left a .content
