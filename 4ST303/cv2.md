# Cvičení II.

* bodový odhad relativní četnosti v základním souboru $p_i = n_i/n$
* intervalový odhad

## Binomický test
* **součástí testů**
* pouze dvě kategorie (případně na dvě kategorie převedeme)
* nulová hypotéza - relativní četnost se rovná konkrétní četnosti
* alternativní - že se nerovná konkrétnímu číslu
* proměnné značíme $\pi_1, \pi_2$
* binomické rozdělení s parametery n, $\pi_{1,0}$
* lze využít exaktní test (použijeme Binomické rozdělení)
    * dostaneme přímo P hodnotu jako distribuční funkci
* případně aproximace normálním rozdělením (když n1 + n2 > 25)
* musíme nastavit správně sloupeček na scale v SPSS, jako kategorii nominal
* Analyze -> One-Sample Nonparametric Text (weight je ten sloupec který testujeme?)
* u výsledku může být komentář a. The alternative... - pouze pro levostrannou alternativní hypotézu (tedy < co testujeme), pravostranná to nemá, oboustranná ne
* data -> weight cases

## Chí-kvadrát
* analysis -> non-parametric -> one-sample -> customize tests -> square

## Kontingenční tabulky
* kontingence - závislost nominálních proměnných
* kontingenční tabulka (i pro jiné typy kategoriálních proměnných)
* nulová hypotéza o nezávislosti

test: chí-kvadrát, binomický test
tabulka četností
zaškrtávací test