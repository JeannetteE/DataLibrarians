# Introduktion til python opgaver:
Her er de opgaver vi har lavet for at give jer en ide om hvad python kan. Opgavesættet består af 2 dele.
* __Del 1__: Består af _python_ opgaver hvor i får prøvet kræfter med de dele af sproget der er præsenteret i hjælpearket. Det er en god ide at læse det igennem og have ved siden af som reference.
* __Del 2__: Består af mere frie og "løse" opgaver, hvor i også selv skal finde på de algoritmer i skal bruger for at løse opgaverne.



## Del 1 - Sig goddag til python
* __Task 1__: _Variabler_ -  Her skal vi lave nogle variabler og printe deres indhold til skærmen. Vi starter med at printe navnet på den opgave vi er igang med.
    ```Python
    print("Task1:")
    ...
    ```
    Erstat `...` med 6 linjer kode hvor 3 af dem laver variabler, en af hver type (tal, bogstaver, sandhedsværdi) og de sidste 3 linjer printer dem.


* __Task 2__: _Matematik_ - Start igen med at printe opgavenummeret altså `Task2`. Nu vil vi så prøve at bruge _python_ som lommeregner. Lav to variabler med tal og to variabler med bogstaver. Prøv så en linje af gange at printe deres resultat. Altså
    ```Python
        print(a + b)
    ```
    For dine to tal gør dette med gange, plus, minus, division (*, +, -, /).
    Var svarene det du forventede?

    For dine to variabler med bogstaver prøv at printe resultatet af at plusse dem sammen, og prøv at print `'Hej' * 2`. Hvad forventer du det giver?


* __Task 3__: - Lister og dictionaries.
Start med at lave en liste af tal og en liste af bogstaver. Når det er gjort så prøv at print det første og sidste element i begge lister.

    Nu skal vi så prøve at lave en dictionary, lav en med 3 "nøgler" hvor du selv vælger hvad de skal hede og deres værdi. Print derefter den midterste værdi ud.


* __Task 4__: Indbygget funktioner - Start med at lave en variabel der er lig med en liste af tal der indeholder 5 elementer. Vi ønsker nu at skrive et lille program der regner gennemsnittet af de tal i listen ud.

    Det betyder at vi skal lægge alle tallene sammen og dividere med længden af listen.
    I python kan man skrive `sum(listeNavn)` for at få summen af en liste og
    `len(listeNavn)` for at få længden.


* __Task 5__: Sandhedsværdier - Her skal vi prøve at lege med sandhedsværdier. Start med at lave den her kode
    ```python
    value1 = True
    value2 = False
    value3 = 10 < 15
    value4 = "Hej" == "Hej"
    ```
    Print 4 resultatet af at bruge disse fire udtryk
    ```python
    a == b
    a and b
    a or b
    not a
    ```
    Hvor du erstatter `a` og `b` med en `value` gør det på en måde hvor udtrykket altid bliver sandt. Til sidst så prøve om du kan regne ud om det her bliver sandt eller falsk før du kører det.
    ```python
    print(value1 and not(value2) or value3  and not value4)
    ```


* __Task 5__: Løkker - Lav en for løkke der printer tallene mellem 1 og 20. Husk på at en for løkke starter med `for i in range(10):` hvor $i$ så går igennem alle tallene i det interval.

    Lav en variabel der er lig med en liste der har 5
    korte sætninger. F.eks
    ```Python
        sentences = [
            'hej med dig',
            'Vi koder i python',
            'DTU har gode lokaler',
        ]
    ```
    Prøv så at lav en for løkke der printer disse sætninger, denne gang på den anden måde hvor løkken starter med `for i in sentences:`


* __Task 6:__ Betingelser - Brug `input()` funktionen til at spørge brugeren om at tal og gem det i en variabel. Hvis tallet er større end $100$ så print en ting, hvis det er mindre end $100$ så print noget andet.


* __Task 7:__ Egne funktioner - Vi vil gerne prøve at lave vores egen funktion. Vi vil gerne lave en funktion der givet et negativt tal returnerer det samme tal bare positivt, og givet et positivt tal returnerer det samme tal bare negativt.

* __Task 8:__ Egne funktioner 2 - Lav en funktion der givet en liste af ord som f.eks `['hej', 'med', 'dig']` aflevere dem som en sammenhængende tekst altså `'Hej med dig'`. Husk at du også kan bruge $+$ ved tekst.


# Del 2
Som sagt er de her opgaver mere løst stillet, det er for at træne jer i hvordan man finder på en algoritme og derefter "forklarer" den til computeren. Husk på de $3$ spørgsmål man kan stille sig selv
1. Hvad er det helt præcist du vil?
2. Kan det deles op i mindre problemer?
3. Hvordan sættes python kommandoer sammen til det?



* __Task 1:__ Lav en funktion der givet et beløb regner ud hvor mange drikkepenge man skal give. F.eks hvis du synes at man altid skal give $10\%$ så skal funktionen ved input $150$ returnere $15$.
__Ekstra point:__ Gør sådan at funktionen både tager beløb og hvor mange procent man vil give


* __Task 2:__ Lav en funktion der givet en liste og et tal fortæller om tallet er i listen. F.eks hvis du kalder din funktion `isIn` så skal den fungere på følgende måde
    ```python
    numbers = [1,3,5,7,9,11,13]
    print(isIn(numbers, 5)) # Skal printe True
    print(isIn(numbers, 10)) # Skal printe False
    ```

* __Task 3:__ Prøv at lav et sten-saks-papir spil.
    En god ide er at sige at f.eks $1$ betyder saks, $2$ betyder sten og $3$ betyder papir. Så kan du bruge `input()` til at spørge brugeren om hvad de vil vælge.
    Hvis du tilføjer `import random` i toppen af koden så kan du sige til computeren at den skal vælge ved at sige `comChoice = random.randint(1,3)` som betyder at den vælger et tilfældigt tal mellem $1$ og $3$.


* __Task 4:__ Find summen af alle lige tal mellem $1$ og $1000$.
    __Hint:__ (I det her udtryk `value = x % 2 == 0` så er `value` lig med `True` hvis det er et lige tal og `False` hvis det er ulige )


* __Task 5:__ Fibonacci tal: Der er en bestemt tal sekvens der hedder fibonacci tal, de første tal ser sådan her ud: $1, 1, 2, 3, 5, 8, 13$.
Hvert tal er lig med de to forgående lagt sammen. Skriv en funktion hvor man kan sige `print(fib(10))´ og den så printer de $10$ første Fibonacci tal.
