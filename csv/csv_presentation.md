# Ting der skal gennemgås til oplæg om csv
* Hvordan en CSV fil ser ud
  * Header
  * Data
* Loading en CSV fil
  * ````python
    with filename as file
    ````
  * ````python
    reader = csv.DictReader(file)
    ````
* Databehandling
  * Søgning af data via headers
  * Iterering af data
  * Skrubning/matching af data
    * Upper/lowercase
      * .lower()
    * Specielkarakterer (, . ? ')
      * Filtrering af alphanumericals via regex (hjælpefunktion)
  * Evt. casting (string -> float/int)
* Escaping karakterer?
  * \\\\
  * \\'
  * \\"
