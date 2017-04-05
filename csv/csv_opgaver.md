# Opgaver til CSV
Hver del indeholder nogle forskellige opgaver af cirka samme sværhedsgrad. Når man kommer til en ny del, vil sværhedsgraden oppes.

## Del 1
Denne del introducerer dig til hvordan man arbejder med CSV filer i Python.
### a)
Åben python skelettet udleveret, og i main funktionen, indlæs csv filen Dish.csv, og lav en læser.

*Vink:* Hvis du er i tvivl, kan du altid læse cheatsheetet igennem for hjælp

### b)
Print de fields der er i Dish.csv.

*Vink:* Man kan tilgå en liste over en readers fields med reader.fieldnames

### c)
Definér en funktion, kaldt getTimesAppeared(reader, amount), som returnerer i en liste alle rækker hvor retten har været i kogebøger præcist *amount* gange.

*Vink:* Kig tilbage i opgave 1.b) for et hint til hvilken field du skal analysere.

### d)
Definér en funktion, kaldt saveFile(row_data, headers, file_name), som gemmer dataen fra listen row_data i filen file_name med de headers givet som argmument.

## Del 2
Denne del viser hvordan man kan kombinere resultater til et resultat.
### a)
Definér en funktion, kaldt getDescriptionsByWord(reader, word), som returnerer alle rækker som indeholder ordet *word*.

*Vink:* Husk at fjerne specialkaraktererne i hvert ord.

### b)
Definér en funktion, kaldt getPriceChange(reader, change), som returnerer alle rækker med en prisstigning lig med eller større end change.

### c)
Definér en funktion, kaldt getExpensiveDishes(reader, change, word), som returnerer alle rækker som har i navnet *word* og et maksimal prisstigning lig med eller større end change.

*Vink 1:* Genbrug funktionerne defineret i 2.a og 2.
*Vink 2:* Man skal bruge en dobbel-løkke (en løkke i en løkke) til at løse opgaven.

## Del 3
Denne del viser hvordan man kan merge to filer til en. Hver række i de csv filer vi skal arbejde med indeholder et unikt id, som kendetegner en ret. I denne opgave vil vi merge nogle af filerne sammen via disse unikke id.
### a)
Udvid main() funktionen til at den også loader Menu.csv som en læser.

### b)
Definér en funktion, kaldt mergeByFields(reader1, reader2, fields), som tager to læsere og en liste af headers, og returnerer én række samlet via fælles id, som indeholder IDets navn, beskrivelse, event og sponsor.

### c)
Gem resultaterne fra 3.b) i en fil ved brug af en skriver.
