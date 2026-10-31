[README.md](https://github.com/user-attachments/files/34219241/README.md)
Memoria Digitale | L'Italia negli anni di piombo (1969-1980)

Progetto d'esame per il corso di Digital Humanities e Patrimonio Culturale della Prof.ssa Francesca Tomasi

Corso di Laurea Magistrale in Scienze Storiche e Orientalistiche presso l'Università di Bologna  

Autore: Lorenzo Brugnati  

Anno Accademico: 2025/2026  



In cosa consiste il progetto?

Memoria Digitale è un archivio storico e collezione digitale di fonti eterogenee, organizzate semanticamente e geolocalizzate, open access dedicato all'analisi e alla valorizzazione della memoria documentaria dell'Italia durante gli Anni di piombo (1969-1980).

Il progetto offre una fruizione digitale integrata delle fonti storiche (articoli di giornale, materiale d'archivio, testimonianze e filmati d'epoca) relative a 12 eventi simbolo del periodo, tra cui la Strage di Piazza Fontana, il Rapimento e l'Omicidio Moro, le stragi di Piazza della Loggia, dell'Italicus e della Stazione di Bologna.



Standard Metadati e Open Access

Dublin Core (DC): ciascun item del catalogo è corredato da metadati strutturati secondo lo schema Dublin Core (incorporati sia come meta-tag HTML nelle schede sia come file XML dedicati e validati).

Linked Open Data & Controllo d'Autorità: utilizzo di vocabolari controllati e URI standard internazionali, tra cui VIAF per i nomi di persona correlati (es. Giuseppe Pinelli, Aldo Moro, Carlo Maria Maggi) e GeoNames per la geolocalizzazione dei luoghi storici.

Tutela Legale: utilizzo del materiale documentario a scopi didattici e scientifici in conformità con la normativa sul diritto d'autore (Art. 70 L. 633/1941).



Quali sono i file principali?

Di seguito viene illustrata la struttura organizzativa della repository GitHub e il ruolo di ciascun file e cartella del progetto:

index.html---->Homepage e introduzione metodologica al progetto

catalogo.html---->Pagina principale del catalogo con la griglia dei 12 item

luoghi.html---->Sezione geografica con mappa interattiva Leaflet

date.html---->Sezione cronologica con la linea del tempo degli eventi

README.md---->Documentazione e guida al progetto (questo file)

css/style.css---->Foglio di stile personalizzato del sito web
    
js/main.js---->Logica in JavaScript vanilla (interazioni UI e mappa)

img/icona del sitoimmagini e anteprime generali

Item---->Repository locale di file multimediali

xml---->File di codifica e metadati XML/Dublin Core/TEI P5 per ogni Item analizzato

catalogoItem---->Sottocartella contenente le schede analitiche dei 12 singoli item


Le funzionalità principali

Il sito web integra componenti W3Schools e Bootstrap 5 avanzati per garantire accessibilità, responsività e un'esperienza utente immersiva:

1. Curtain Navigation Overlay (W3Schools/Bootstrap): menu a comparsa a schermo intero gestito in JavaScript, richiamabile dalla sticky header su tutte le pagine.

2. Griglia Dinamica di Card (Bootstrap 5 Grid System): visualizzazione responsive degli oggetti digitali in `catalogo.html` con anteprima, datazione, indicazione del luogo e bottone di reindirizzamento alla scheda di dettaglio.

3. Schede Descrittive e Metadati Strutturati: tabelle analitiche realizzate con classi Bootstrap (`table-striped`, `table-bordered`) che mostrano metadati DC, identificatori unici, collegamenti esterni VIAF e link georeferenziati.

4. Lettore Multimediale Integrato: utilizzo dei contenitori reattivi Bootstrap (`ratio ratio-16x9`) per la riproduzione fluida di video MP4 (teche Rai, interviste storiche, documentari) direttamente nella scheda dell'item.

5. Mappa Geografica Interattiva (Leaflet.js & Esri Topo): visualizzazione dei luoghi degli eventi storici in `luoghi.html` tramite marker geolocalizzati e popup informativi.

6. Cronologia Storica (Timeline): interfaccia grafica in `date.html` per l'esplorazione sequenziale degli avvenimenti dal 1969 al 1980.

7. Architettura a Percorsi Relativi Standardizzati: organizzazione modulare con gestione dei percorsi dei file tramite notazione relativa (`../`) per tutte le risorse allocate nella sottocartella `catalogoItem/`.
