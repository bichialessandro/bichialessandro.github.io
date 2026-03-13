# Nuovo Sito Bichi Alessandro - Design Spec

## Obiettivo
Ricreare il sito www.bichialessandro.it come sito one-page moderno, responsivo e professionale con colore principale blu.

## Struttura
Sito single-page HTML/CSS/JS puro, nessun framework.

### Sezioni (scroll verticale)
1. **Navbar** - sticky, logo + menu links, hamburger su mobile
2. **Hero** - gradiente blu, badge "Dal 1995", titolo, sottotitolo, CTA "Richiedi Preventivo"
3. **Chi Siamo** - testo storia aziendale + foto + statistiche (30+ anni, 5 marchi, 1000+ clienti)
4. **Servizi** - 5 card con icone SVG: riavvolgimento motori, assistenza utensili, progettazione, pompe idrauliche, vendita utensili
5. **Marchi** - 5 card: Makita, Rupes, Pedrollo, Dreno, CML (con loghi esistenti)
6. **Gallery** - griglia foto 4 colonne (2 su mobile), placeholder Unsplash
7. **Contatti** - info contatto + form preventivo + Google Maps embed
8. **Footer** - copyright, P.IVA, indirizzo

### Palette
- Blu scuro: #1a3a6b (navbar, footer, hero)
- Blu primario: #2563eb (titoli, accenti, bottoni)
- Blu chiaro: #3b82f6 (hover, dettagli)
- Oro: #f59e0b (CTA, badge)
- Sfondo: #f8fafc (sezioni alternate con #f1f5f9)
- Testo: #1e293b

### Caratteristiche tecniche
- Responsive: mobile, tablet, desktop
- Scroll fluido tra sezioni
- Navbar sticky con evidenziazione sezione corrente
- Menu hamburger su mobile
- Animazioni fade-in al scroll (IntersectionObserver)
- Form preventivo (submit via mailto o action esterna)
- Google Maps embed nella sezione contatti
- Icone SVG inline (no dipendenze esterne)
- Foto placeholder da Unsplash (sostituibili)

### Dati aziendali
- Ragione sociale: Bichi Alessandro
- Attività: Utensili e Riparazioni
- Indirizzo: Via Aretina 150, 50061 Compiobbi (FI)
- Telefono/Fax: 055 6593423
- Email: info@bichialessandro.it
- P.IVA: 04688770488
- CF: BCHLSN73D01D612C
- Fondata: 1995

### Deploy
- File: index.html (sovrascrive il redirect attuale)
- Upload: Serverplan via FTP (`curl --netrc`) + push GitHub Pages
- Backup vecchio sito: rinominare file .html attuali in .old
