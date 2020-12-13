# Přednáška I.
* zpracování textů
    * s ohledem na obsah
* informatika
    * definice
        * věda o cílevědomém zpracování informací prostřednictvm automaticky pracujících strojů
    * informace
        * více pohledů
        * proces informování - někdo něcomu něco sděluje (předává znalost)
        * technický pohled - přenos zprávy (komunikačním kanálem), záznam zprávy (na nějakém médiu)
        * matematický pohled - informace = míra snížení neurčitosti
        * čím pravděpodobnější je výskyt určité zprávy, tím méně informace taková zpráva nese
    * z pohledu informatiky
        * informace = interpretace dat
* zpracování textů
    * vytváření, šíření, shromažďování, pořádání, vyhledávání, zpřístupňování

* informační věk
    * informační exploze
        * roční produkce informací se znásobuje
    * informační zahlcení
        * výsledek informační exploze, přitom klesá podíl nových informací
    * informační bariéry
        * potřeba efektivního výběru informací, jazykové bariéry, ekonomické bariéry
    * rozptyl informací
        * Bradfordův experiment, seřadil časopisy podle počtu článků na dané téma, rozdělil je na zóny s přibližně stejným celkovým počtem článků ($k_1 = n$, $k_2 = n^2$, $k_3 = n^3$ přičemž $k_1 = k_2 = k_3$)
    * stárnutí informací
        * vzali vzorek publikací z nějakého oboru, počítali citované zdroje staré 1 rok, 2 roky a dále
        * 75 % citovaných zdrojů je z posledních 10 let, 88 % z posledních 20 let (pro vybraný obor, který studovali)
        * poločas stárnutí - časový interval, do kterého se vejde polovina citovaných zdrojů

# Přednáška II.
* přirozený jazyk
* interpretace - na více úrovních, nutno provádět zdola nahoru
    * hlásková, znaková rovina -> morfologicko-lexikální rovina -> syntaktická rovina
* každá rovina jazyka má vlastní pravidla (gramatiku) - hlavní roviny gramatiky - syntaxe, morfologie, fonologie (fonotaxe), pravopis
* do úrovně morfologicko-lexikální vstupuje slovník (slovník - seznam posloupnosti hlásek, které lze v daném jazyce použít k pojmenování nějaké skutečnosti nebo představy)
* sémantika - nad gramatikou a slovníkem, lexikální sémantika = významy slov, sémantina nad gramatikou = vztah forem a funkcí mezi jednotlivými rovinami gramatiky
* synonymie, homonymie
* jazyk funguje pragmaticky

# Přednáška III.
* informační proces v užším pojetí
* akvizice (předpoklád - sledování produkce)
    * získávání zdarma, získávání nákupem
* pořádání
    * informační analýza, obsahová
    * identifikační - bibliografický záznam, katalogizační záznam, bibliografická citace
        * co identifikuje dokument - kdo, co, kde, kdy
        * stránkový rozsah, systémový identifikátor
        * obsahová - redukované sekundární dokumenty referát, anotace
        * indexování
        * selekční jazyky - na bázi přirozeného jazyka, umělé
            * přirozený jazyk
                * problémy - synonomie, homonymie
            * tezaurus - deskriptory, nedeskriptory
            * ekvivalence, hierarchie, asociovanost
        * umělé - DDC, MPT

# Přednáška IV.
* internet jako zdroj informací
* rozdíly v obsahu, rozsahu, faktické dostupnosti dokumentu
* volně přístupné vs placené zdroje
* ne vše je vyhledatelné
* pokrytí webu je pravděpodobně dost nízké
* předmětové katalogy
    * závislost na předem daných tématických strukturách
* portály
* přesnost vyhledávání - precision, úplnost - recall
* kvalita obsahu - aktuálnost, autorizovanost, adresa, objektivita, chyby

# Přednáška V.
* text je v přirozeném jazyce, rozdělený na slova
* cílem indexování je přiřadit dokumentu selekční obraz
* cílem indexování je zjistit slova která nejlépe charakterizují jeho obsah
* základní problémy
    * různá míra významnosti jednotlivých výrazů v textu
        * vlastní obsažnost/významnost výrazu, selektivní síla výrazu i v bázi dokumentů b, schopnost výrazu i charakterizovat text T lépe než jiné výrazy - frekvence
        * tf-idf - term frequency - inverse document frequency
    * morfologická variabilita výrazů v textu
        * problém s koncovkami
    * překrývání významu výrazů
    * homonymie výrazů
* základní nástroje
    * derivátor
        * slovník všech slov nebo pravidla která vycházejí z toho, jak slovo vypadá
    * lematizátor

