do odevzdávárny excel

příklady nebudou jasně zadané - prostě bude příklad a pak musíme vybrat správné řešení
chí kvadrát (očekávané četnosti...), poměry šancí, McNemarův test

# Volné poznámky
* Vše je na výběrový soubor, vše jsou výběrové charakteristiky!
* 0,028 < 0,05 zamítáme nulovou hypotézu jsou závislé 
* 0,028 > 0,01 nezamítáme nulovou hypotézu jsou nezávislé
* 0,054 > 0,05 zamítáme nulovou hypotézu jsou závislé 

# Typy proměnných
* klasifikace proměnných
    * kvantitativní
        * spojitá
        * diskrétní
    * (kvalitatitvní)
        * alternativní-dichotomická
        * nominální
        * ordinální
    * kategoriální
* škály měření
    * nominální - různé, nelze odlišit pořadí
    * ordinální - stanovit poořadí, ne o kolik je vtší
    * intervalová - můžeme určit o kolik je jedna hodnota větší či menší než druhá
    * poměrová - o kolik i kolikrát je hodnota větší než druhá
* klasifikace proměnných podle typů škály
    * nominální - např. typ profese
    * ordinální - např. stupěn znalosti
    * kvantitativní - intervalové (počet stupňů), poměrové - počet členů domácnosti
* z hlediska statistické analýzy
    * kvantitativní spojité (z libovolného intervalu)
    * kategoriální - nominální, ordinální nebo kvantitativní
        * obor hodnot jsou kategorie, malý počet obvykle
    * kvalitatitivní - nominální a ordinální
    * kvantitativní diskrétní a ordinální s větším počtem hodnot
    * kvantitativní spojité
* proměnné
    * dichotomické (alternativní)
    * symetrické - obě kategorie mají stejnou dlůežitost
    * asymetrické - jedna kategorie je důležitější
    * binární - hodnoty 0 a 1

# Popisné charakteristiky

* popisné charakteristiky
    * nominální proměnná
        * míry polohy - úrovně (počet, procenta)
            * modální kategorie - kategorie s největší četností
                * pokud p_mo > 0,5 tak můžeme označit modální kat. jako majoritní
        * míra variability
            * vyjádření koncentrace
            * mírou může být relativní četnost modální kategorie nebo součet druhých mocnin relativních četností
            * variační poměr
            * nominální rozptyl (Giniho koeficient)
            * entropie
    * ordinální proměnmná
        * míry polohy
            * modální kategorie, medianová kategorie
            * medián (číselné označení aktegorií)
        * míry variability
            * ordinální rozptyl
    * kvantitativní proměnná
        * míry polohy
            * modus
            * medián
            * aritmetický průměr
        * kvantily
            * kategorie dolního kvartilu (0,25), kategorie horního kvartilu (0,75)
            * dolníé kvartil, horní kvartil
            * prostřední kvartil = medián
        * variabilita
            * variační rozpětí
            * mezikvartilové rozpětí
            * rozptyl
            * směrodatná odchylka
            * variační koeficient
            * poměrový koeficient diferenciace
            

# Míry

# Odhad relativní četností
* bodový odhad + směrodatná odchylka

# Hypotézy a testování
## Binomický test
* testuje se četnost 1 konkrétní kategorie, u dichotomické proměnné, buď shoda četností nebo jednostranná H1

* $H_0 = \pi_k = \pi_{k,0}$
* $H_0 = \pi_1 = \pi_2$ (tohle je později v prezentaci a dává to víc smysl)
* $H_1 = \pi_k \neq \pi_{k,0}$

* k-tá kategorie, nulová hypotéza k-té kategorie se rovná určité četnosti
    * alternativní hypotéza bývá že se nerovná této četnosti
* proměnná dichotomická, nebo na dvě kategorie převedeme
* exaktní test - dostaneme přímo p-hodnotu jako distribuční funkci která je rovná té menší z těch četností
* aproximace normálním rozdělením
* když testujeme na 0,5 tak je oboustranná
    * dvojnásobek distribuční funkce?
* weight cases 
* SPSS - nonparametric
* one-sample nonparametric tests -> settings -> choose tests -> binomial test
* pokud nás zajímá jiný sig. level tak v settings -> test options
* pokud nás zajímá $\pi_1 = 0,6$ tak hypothesized proportion v settings -> 0,6
* pro 0,6 -> pí_1 <= 0,6 - hláška se zobrazuje jen pro levostranné
* testujeme 0,4 (binom_other), alternativní hypotéza pí_1 < 0,4
* když pod tabulkou není nic tak je pravostranná pí_1 > 0,1
* SPSS - CDF.BINOM(1,5,0.4)
* kalkulátor na levostrannou nebo pravostrannou - http://statkat.com/online-calculators/p-value-binomial-test-single-proportion.php

# Chí-kvadrát test dobré shody
* $H_0 = \pi_i = \pi_{0,i}$, $i = 1,...,K$
* $H_1 = non H_0$

* testují se četnosti v několika kategoriích současně
* shoda zjištěných a očekávaných četností (případně ve spec. případech shoda četností)
* testují se četnosti, testové kritérium napozorované - očekávané...
* volnost - počet kategorií - 1
* očekávané četnosti alespoň 5
* analyze -> nonparametric tests -> onesample -> settings -> chisq
* očekávané četnosti lze zadat v nastavení testu
* p-hodnota pro X2
    * transform -> compute variable -> 1-CDF.CHISQ(6,5) (hodnota 6 a stupňů volnosti 5)
* kritická hodnota - 0,05 a 5 dof - IDF.CHISQ(0,95;5)
* p-hodnota - test statistic

* kontingenčí tabulka - p-hodnota - descriptive statistics - crosstabs - rows x, columns y -> 

* když znám actual a expected a chci znát p-hodnotu
    * v Excelu funkce CHISQ.TEST()

# Koeficienty
* testuje se nulovost koeficientu
* p-hodnoty - approximate signficance

# Kontingenční tabulky
(projít přednášku! nějak mi ty zápisky nedávají smysl)
* závislost nominálních proměnných
* kontingenční tabulka
* sdružené absolutní četnosti, marginální relativní četnosti
* očekávaná četnost v případě nezávislosti $m_{i,j} = \frac{n_{i+} n_{+j}}{n}$
* $H_0 = p_{i+}p_{+j}$, $H_1 = non H_0$ testujeme tedy že četnosti odpovídají očekávaným četnostem
* $m_{ij} > 5$

# Závislost nominálních proměnných
* pearsonův kontingenční koeficient
* cramérovo v (maximální hodnota 1)
* Goodmanovo-Kruskalovo $\lambda$ (0 = není žádný vztah, 1 = perfektní vztah)
* informační koeficient
* Goodmanovo-Kruskalovo Tau

# Závislost ordinálních proměnných
* Spearmanův koeficient pořadové korelace
* míry založené na konkordantních a diskordantních párech
* Goodmanovo-Kruskalovo gamma, Kendallovo TauB, Kendallovo TauC, Stuartrovo TauC, SomersovoD
* shlukování proměnných - stromový diagram, koeficient tauB

# Koeficienty závislosti
* jedna nebo obě nominální
    * symetrická
        * Pearsonův kontingenční koeficient, Cramérovo V, Čuprovův kontingenční koeficient
    * asymetrická
        * Goodmanovo-Kruskalovo Lambda, Goodmanovo-Kruskalovo Tau, Informační koeficient
* obě ordinální
    * symetrická
        * Goodmanovo-Kruskalovo gamma, Kendallovo TauB, Kendallovo (Stuartovo) TauC, Spearmanův korelační koeficient
    * asymetrická
        * Somersovo D
* vysvětlovaná kvantitativní, vysvětlující nominální - koeficient éta
* obě dichotomicjké (čtyřpolní tabulka)
    * symetrická
        * koeficient phí, Yuleho Q, Yuleho koeficient vazby
    * asymetrická
        * poměr šancí

# Čtvercové tabulky
* vztah dvou proměnných, které nabývají stejných kategorií
* míry souhlasu
    * Cohenovo Kappa

# Dvě kvantitativní proměnné
* Pearsonův korelační koeficient
# Kvantitativní + nominální
* koeficient éta
* analýza rozptylu (ANOVA)

# Čtyřpolní tabulky
* závislost dvou dichotomických proměnných
* Yatesova korekce, věrohodnostní poměr
* korelační koeficient, koeficient asociace
* Mantelova-Haenszelova statistika chí-kvadrát
## Fisherův exaktní test
* v případě, že nejsou splněny podmínky pro chí-kvadrát test (četnosti)
* $H_0 = \pi_{11} = p_{1+}p_{+1}$
* alternativní hypotézy
    * ten výběr závisí na tom jestli je očekávaná větší nebo menší
    * $H_1 > \pi_{11} = p_{1+}p_{+1}$ 
    * $H_1 \neq \pi_{11} = p_{1+}p_{+1}$
    * $H_1 < \pi_{11} = p_{1+}p_{+1}$
## McNemarův test
* aplikace binomického testu na shodu četností v políčkách na vedlejší diagonále
* používá se při zkoumání změny, např. před anketou a po anketě
* $H_0 = \pi_{12} = \pi_{21}$
* $H_1 = \pi_{12} \neq \pi_{21}$
## Yuleho Q, Yuleho koeficient vazby, Hamannův koeficient
## Yuleho Q
* počítá se jako koeficient gamma, pro čtyřpolní tabulku se jen jmenuje takto, kdo ví proč
* ![Weka](./img/crosstab4.PNG)
* crosstabs, Gamma, Symmetric measures, Ordigan by Ordinal Gamma, -,39...
* zobrazuje se jako matice, je symetrická
* shluková hierarchická analýza
* rozsah -1 až 1, 1 perfektní pozitivní korelace (obě rostou spolu), -1 inverzní, 0 není asociace :)
* nevím co k ním napsat, jsou v té přednášce
## Poměr šancí
* koeficient relativního rizika
    * sloupcová proměnná x1 / celkem v řádku, sloupcová proměnná x2 / celkem v druhém řádku
    * ![Weka](./img/crosstab5.PNG)
* interpretuje se, kolikrát je větší šance
    * poměr šancí v obrázku nahoře vychází 3,398
    * např. že absolventi FISu mají 3x větší šanci se uplatnit ve stejném oboru
* kde je závislost na chí-kvadrátu tak tam je i závislost poměru šancí
* Yuleho Q, Yuleho Y je funkcí poměru šancí
    * ![Weka](./img/eq1.PNG)
* PSPP
    * crosstabs, Risk
    * Odds ratio for řádek (1/2) -> value 3,40
    * lower, upper -> interval pro spolehlivost
    * pozor, zdá se, že ty intervaly vychází nějak nesmyslně
* závislost lze zjistit z chisq
    * asymptotic sig. 0,035 < 0,05, na 5 % hladině tedy zamítáme hypotézu o nezávislosti, tj. jsou závislé

# Neparametrické testy
* Mannův-Whitneyho test (o shodě rozdělení)
    * jednostranná závislost, ordinální vysvětlované proměnná
* Kruskalův-Wallisův test (o shodě rozdělení)
    * jednostranná závislost, ordinální vysvětlovaná proměnná
* Mediánový test pro K výběrů (o shodě mediánů)
    * jednostranná závislost, ordinální vysvětlovaná proměnná
* Znaménkový test (dva závislé výběry)
* Wilcoxonův párový test (dva závislé výběry)
* Friedmanův test (více než dva závislé výběry)
    * test o shodě rozdělení
    * kódům odpovědi získaných od určitého respondenta přiřadíme pořadí k hodnot zjištěných u k sledovaných proměnných
* Kendallovo W (více než dva závislé výběry)
    * test o shodě rozdělení + určení míry souladu
* Cochranovo Q (více než dva závislé výběry)
    * test o shodě podílu jedné ze dvou kategorií


# Logistická regrese
* logistická regrese
    * binární logistická regrese
        * binární vysvětlovaná proměnná Y
        * vysvětlující jak kategoriální (nominální) tak i kvantitativní
        * $\pi = P(Y = 1)$
            * pravděpodobnost že Y = 1?
        * šance $\frac{\pi}{1-\pi}$
        * logit $\ln\frac{\pi}{1-\pi}$
        * odhad pravděpodobnosti lze získat na základě $\pi = \frac{e^{{\beta_0} + {\beta_1}x_1...}}{1 + e^{{\beta_0} + {\beta_1}x_1...}}$
        * změna šancí nastoupení jevu
        * ![logres](./img/logres.png)
        * v Excel souboru
            * nevím proč, ale přehazovala řádky i sloupce u procent - sloupce proto aby to šlo (aby tam byla kladná proměnná)
* multinomická logistická regrese
    * vysvětlovaná nominální s více než dvěma kategoriemi
    * vysvětlovaná proměnná má 3 kategorie
    * vysvětlující jak kategoriální (nominální) tak i kvantitativní
    * X nabývá 3 kategorií $z_1 = 1$ pro $x=1$ a $z_2 = 1$ pro $x=2$, jinak $z_j = 0$
    * rozdělíme na dvě kontingenční tabulky
    * např. žádný a malý přínos, střední přínos a velký přínos
    * dělají se dvě kontigenční tabulky - vždy jedna stejná kategorie
* vztah mezi parametrem ($\beta_0 = \ln{\frac{p_{1|0}}{1-p_{1|0}}}$ a $\beta_1 = \ln{\frac{p_{1|1}}{1-p_{1|1}}}$)
* p1,1 = první řádek, p1,0 = druhý řádek
* zkoumáme jen pro první sloupečkovou kategorii (ta by měla být pozitivní - teda ano)
* proměnné se nemusí překódovávat, SPSS to umí samo
* v ZT je otázka i na diskriminační analýzu, vysvětlovaná obecně nominální, vysvěltující pouze kvantitativní

# Diskriminační analýza
(projít prezentaci)

# Klasifikační stromy
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

# Shluková analýza
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