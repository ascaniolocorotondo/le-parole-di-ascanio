# Le Parole di Ascanio

Un gioco per indovinare parole italiane, da giocare sia sul computer che sul telefono.

👉 **Gioca qui: https://ascaniolocorotondo.github.io/le-parole-di-ascanio/**

## Come si gioca

1. Scegli quante lettere deve avere la parola (da 4 a 8) e la difficoltà.
2. Scrivi una parola italiana vera e premi **Invio**.
3. Le lettere si colorano:
   - 🟩 la lettera è giusta ed è al posto giusto
   - 🟨 la lettera c'è, ma in un altro posto
   - ⬜ la lettera non c'è
4. Indovina la parola prima di finire i tentativi.

Anche la tastiera si colora, così vedi subito quali lettere hai già escluso.

| Difficoltà | Aiuto | Tentativi |
|---|---|---|
| Facile | la prima lettera è già scritta | lettere + 2 |
| Media | nessuno | lettere + 1 |
| Difficile | nessuno | quanti sono le lettere |

## Com'è fatto

È un sito statico, senza server e senza installazioni:

- `index.html`: il gioco
- `style.css`: lo stile
- `parole.json`: le parole da indovinare (le 1000 più comuni) e il dizionario di circa 76.000 parole valide

Per provarlo sul computer basta servire la cartella, per esempio con:

```bash
python -m http.server
```

poi apri http://localhost:8000. Aprendo `index.html` con un doppio clic il dizionario non si carica, perché il browser blocca la lettura del file.

## Crediti

Le liste di parole vengono da [napolux/paroleitaliane](https://github.com/napolux/paroleitaliane), con licenza MIT. Il testo della licenza è in [LICENSE-dizionario.txt](LICENSE-dizionario.txt).
