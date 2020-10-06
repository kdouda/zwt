# Cvičení I.
* kniha Analýza dat z dotazníkových šetření
    * průběžný test 0-12 b
    * zpracování seminární práce 0-13 b
    * závěrečný test 0-75 b

## Klasifikace proměnných
* statistický znak - proměnná
    * kvantitativní
        * spojitá (plat, věk)
        * diskrétní (počet dětí)
    * kvalitativní
        * alternativní-dichotomická (pohlaví)
        * nominální (zaměření)
        * ordinální-pořadová (vzdělání)
    * kategoriální - málo hodnot
* škály měření
    * škála nominální - můžeme určit jestli jsou stejné nebo různé, ale nemůžeme stanovit jejich pořadí
    * škála ordinální - můžeme stanovit pořadí, nemůžeme však určit, o kolik je jedna hodnota větší či menší než druhá
    * škála intervalová - můžeme určit, o kolik je jedna hodnota větší či menší než druhá
    * škála poměrová - můžeme určit o kolik i kolikrát
* podle škály
    * nominální - typ absolvované střední školy, typ profese, druh výrobku
    * ordinální (stupeň znalosti, stupeň souhlasu s určitým výrokem)
    * kvantitativní (intervalové - např teplota, a poměrové - nula zde má význam!), v SPSS *scale* nebo *interval*
* dichotomické (alternativní) - pouze dvě kategorie
    * symetrické - kategorie mají obě stejnou důležitost
    * asymetrické - jedna kategorie je důležitější
    * binární - hodnoty 0 a 1 - u některých metod snižuje komplexitu
* rozdělení četností
    * absolutní
    * relativní
    * kumulativní relativní
    > $$P_i(x)$$
    * SPSS - platné hodnoty (chybějící údaje, když např. u dotazníku respondent neodpoví), v tabulce četností se odděluje

# Popisné charakteristiky
## Kategoriální proměnné
* míry polohy (C1 v SPSS)
    * modální kategorie - má nejvyšší četnost $x_{Mo}$
        * $n_{i}$ jsou absolutní 
* míra koncentrace
    * relativní četnost modální kategorie $p_{Mo}$
    * součet druhých mocnin relativních četností
        * $\sum_i{p_i^2}$
    * ilustrační příklad - všichni respondentni zvolili stejnou možnost, $p_{Mo} = 1$, nejvyšší koncentrace a nejnižší variabilita
    * rovnoměrně rozložené $p_{Mo} = 1/K$ - nejvyšší variabilita a nejnižší koncentrace
* míra variability
    * variační poměr $v = 1 - p_{Mo} = 1 - n_{Mo}/n$
    * nominální rozptyl (Giniho koeficient)
        *  $nomvar = 1 - \sum_{i=1}^K{p_i^2} = \sum_{i=1}^K{p_i (1 - p_i)}$ 
    * všichni zvolili jednu skupinu
        * $1 - p_{Mo} = 0$
    * rovnoměrně rozložené
        *  $v = (K - 1) / K$
    * entropie
        * nejnižší variabilita - H = 0
        * nejvyšší variabilita  $H = \ln{K}$
## Ordinální proměnné
* míry polohy
    * modální kategorie
    * mediánová kategorie
    * medián - vyžaduje číselné označení kategorií
* míra variability
    * ordinální rozptyl $dorvar = 2\sum_{i=1}^{K-1}(P_i(1-P_i))$
        * nejnižší variabilita (nejvyšší koncentrace) - 0
        * nejvyšší variabilita - když jsou krajní kategorie nejvíce četné $dorvar ∈ <0; (K-1)/2>$
## Kvantitativní
* modus
* medián
* aritmetický průměr
* kvantily
* míra variability
    * variační rozpětí
    * mezikvartilové rozpětí
    * rozptyl
    * směrodatná odchylka
    * variační koeficient
    * poměrový koeficient diferenciace
