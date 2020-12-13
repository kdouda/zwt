* nominální vysvětlovaná, vystvětlující kvantitativní - diskriminační analýza

# Klasifikační stromy
* odhaduje výslednou kategoriální proměnnou
* vstup mohou být nominální, ordinální i kvantitativní proměnné
* klasifikační strom vybírá takovou proměnnou která má nejvyšší vliv na rozlišení hodnot vysvětlované proměnné
* vybere proměnnou a zkouší různé možnosti překódování
* zkouší různé možnosti překódování
    * kvantaitativní vytváří intervaly
    * ordinální spojuje pouze za sebou
    * kategoriální může sjednocovat

* logres - vysvětlující jak kvantitativní tak kategoriální, převádí se na kvantitativní
* diskriminační analýza - vysvětlující pouze kvantitativní
* klasifikační stromy - jak kategoriální tak kvantitativní spojité proměnné, ale interně si vše převádí na kategoriální

* postup výběru proměnných
    * vyberou se dvě proměnné a udělá se chí-kvadrát s využitím Pearson. testem nebo věrohodnostního testu
    * nejnižší p-hodnota -> ta proměnná se vybere jako vysvětlující
    * p-hodnoty se upravují Bonferohi metodou
    * ze souboru vzniknou tři podsoubory
    * v podsouborech se hledá opět znovu, pokud nebude statisticky významná závislost tak se nevybere žádná
    * pravidla pro ukončení větvení stromu - počet objektů v uzlech, nebo když není významná proměnná, mohou být i jiná kritéria

* zjistíme variabilitu po oddělení do skupin (vnitroskupinovou)
    * snažíme se aby vnitroskupinová variabilita byla co nejnižší (nejvyšší meziskupinová)

* využívají se i jiné míry např, gini

* data lze vyjádřit jako shluky
    * giniho míra (nomvar)

* shluková analýza

* podíly skupin z celkového počtu

* shluková analýza
    * jaké skupiny existují, kolik jich je...
    * metody rozkladu (kolik skupin má být)
    * zkusit rozložit objekty do podskupin
    * shlukování - pevné nebo fuzzy (pravděpodobnost příslušnosti)
    * centroid (průměry, mediány, nestanovuje se,)
    * vzdálenosti - objektů od centroidů, vzdálenosti mezi objekty z různých shluků
    * tři skupiny
        * pevný rozklad
        * fuzzy rozklad
        * hierarchické metody


* 