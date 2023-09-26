# la-mia-pizzeria-static

Ciao ragazzi oggi iniziamo a muovere i primi passi con questo fantastico Asp .Net Core MVC!  
Dobbiamo realizzare un’applicazione web che ci aiuti a gestire la nostra pizzeria.  
Abbiamo bisogno di creare la nostra prima pagina (index) per l'amministratore dove mostriamo tutte le pizze che il nostro locale gestisce.  
Una pizza avrà le seguenti informazioni :  
> - un nome  
> - una descrizione 
> - una foto (url) 
> - un prezzo
  
Modifichiamo quindi la view Index.cshtml generata in automatico da .Net Core scrivendo l’html che serve a noi per mostrare l’elenco delle pizze (possiamo creare una tabella con bootstrap o una qualche grafica a nostro piacimento che mostri l’elenco delle pizze... che sia funzionale e veloce per un amministratore!)  
Piccolo suggerimento : ricordatevi di inserire il seguente codice all’inizio della vostra view @ { Layout = null; }  
*BONUS:*   
Se vi avanza tempo, create anche una landing page per un cliente della vostra pizzeria che vuole vedere le vostre pizze. Chiamiamo questa pagina UserIndex.cshtml e creiamola nella cartella Home delle Views. A questo punto dovete creare all'interno di Controllers > HomeController.cs un metodo  
  
    public IActionResult UserIndex()  
    {  
	    return View();  
    }  
  
Con il quale ci andremo a far restituire la pagine UserIndex. Questa nuova pagina si troverà all'indirizzo /Home/UserIndex del vostro sito. Potete usare questo link per i vostri <a> tag.
