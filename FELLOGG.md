# Fellogg

En rad per fel. Skriv medan du minns hur du gjorde.

| Nr | Vad stod i loggen? | Lokalt eller på GitHub? | Hur tog du reda på orsaken? | Hur löste du det? |
|----|--------------------|-------------------------|-----------------------------|-------------------|
| 1  |           Det står att det är en felaktig yml-fil, att det finns ett yaml-syntaxfel på linje 11         |      På github                   |     Kollade i filen. Det ser ut som att en indentering under steps, i jobs, är fel.                        |   Tog bort ett mellanslag som inte skulle vara där.                |
| 2  |    Couldnt find lockfile.                |    Github                     |   borde ha kört en uv sync direkt när jag klonade                          |    körde uv sync               |
| 3  |    ruff går inte igenom                |    github                     |    importfel                         |   kör uv run ruff check --fix                |
| 4  |    ruff går inte igenom på formatnivå                |    github                     |                             |   kör uv run ruff format                |
| 5  |    pytests får en failure                |    lokalt (uv run pytest)                     |    logiskt fel, summan delas med window +1 i stället för antalet värden i fönstret                         |   ändrade nämnaren från window +1 till window så funktionen beräknar rätt medelvärde                |

Fortsätt tabellen med fler rader vid behov.
