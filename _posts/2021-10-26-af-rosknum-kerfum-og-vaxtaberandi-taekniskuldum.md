---
layout: post
title: Af rosknum kerfum og vaxtaberandi tækniskuldum
description: Daginn eftir að ný tækni er tekin í notkun byrjar tæknileg skuld að telja. Tæknilega skuldin er vaxtaberandi skuld og getur líkt og peningaskuld sligað rekstur fyrirtækja. Stjórnunar- og tækniaðferðir DevOps er leiðin áfram.
summary: Daginn eftir að ný tækni er tekin í notkun byrjar tæknileg skuld að telja. Tæknilega skuldin er vaxtaberandi skuld og getur líkt og peningaskuld sligað rekstur fyrirtækja. Stjórnunar- og tækniaðferðir DevOps er leiðin áfram.
tags: 
    - legacy systems
    - technical debt
    - devops
    - cloud
---

![Roskin kerfi](https://s3.eu-west-1.amazonaws.com/olafur.org/mainframe.jpeg)

Daginn eftir að ný tækni er tekin í notkun byrjar tæknileg skuld að telja. Tæknilega skuldin er vaxtaberandi skuld og getur líkt og peningaskuld sligað rekstur fyrirtækja.

Fyrirtæki sem greiða ekki reglulega inn á tækniskuld sína geta lent í aðstæðum þar sem þau jafnvel ná ekki einu sinni að borga vextina og vandamálið stækkar með hverjum deginum. Slíkar aðstæður sliga alla framþróun og heldur fyrirtækjum í gíslingu.

Tími sem við vildum heldur verja í þróun nýjunga fuðrar upp í handvirkum síendurteknum rekstrarviðvikum og slökkvistarfi.

**Roskið kerfi (e. legacy systems):**
```text
Úrelt kerfi komið yfir miðjan aldur, sem er enn í notkun.
```
## Spírall ábyrgðarleysis og sakbendinga

Algengt viðkvæði í þessu er að það sé svo stutt í að einu eða fleiri grunnkerfum verði skipt út að það taki því ekki að tækla vandamálið núna. Allt verði miklu betra þegar nýja kerfið fari í loftið. Svo líða vikur, mánuðir og ár en aldrei kemur dagurinn þar sem okkur hafði verið lofað að allt yrði breytt.

Við endum svo í kúltúrlegum spíral þar sem forverum er bölvað fyrir allar vondu ákvarðanirnar en enginn tekur ábyrgð og gerir eitthvað í vandamálinu.

Svo endar með því að einhver stjórnandinn rífur upp tékkaheftið og setur í gang sársaukafulla big-bang innleiðingu á nýju kerfi með loforði um að öll vandamálin heyri sögunni til. Verkefnin lenda svo í tímaþröng og menn enda á að moka vandamálunum með sér inn í nýja kerfið og sagan endurtekur sig.

## Ný nálgun í stjórnun

Lausnin við að tækla hin rosknu kerfi er að hætta big-bang nálgun og tækla vandamálið í anda stjórnunar- og tækniaðferða sem kenndar eru við DevOps hugmyndafræðina:
- Hefjumst handa strax við að gera tækniumhverfið aðeins betra í dag en það var í gær án þess að kollvarpa neinu.
- Brjótum upp sílóin í kringum þróun (dev) og rekstur (ops) og setjum af stað fókuserað umbótateymi þróunar og reksturs sem hefur það eina markmið að bæta vinnuumhverfi allra hinna.
- Gerum það hluta af vinnunni að viðhalda gæðum og borga niður tækniskuld, verjum t.d. 20% af þróunartímanum. Tækniskuldin þarf að vera í föstum afborgunum.
- "Go slow to go faster". Fjárfesting í umbótum með vinnu fárra getur skilað sér margfalt í hraðari vinnu margra.
- Kúplum roskna kerfið í sundur og færum einn feril í einu yfir í nýrra umhverfi. Beitum [kyrkingaraðferðinni](https://dzone.com/articles/monolith-to-microservices-using-the-strangler-patt) (e. strangler pattern) til að minnka áhættu við umbreytinguna.
- Gerum starfsfólki kleift að verja tíma í lærdóm og hvetjum til tilrauna.
- Það er ekki raunhæft að ætla að endurskrifa allt. Setjum fókusinn á að frelsa gögnin og gera okkur auðvelt fyrir að vinna með þau. Komum gögnum inn í millilag og uppfærum svo hvaða gagnalindir millilagið sækir í eftir því sem grunnkerfin breytast.

## Vítahringur ósjálfbærrar pressu á nýjungar

Ástæður þess að við lendum á þessum stað geta verið skilningsleysi stjórnenda, röng þekkingarsamsetning, skortur á þróunarkúltúr eða sinnuleysi tæknistjórnenda. En ég hef líka séð mynstur ósjálfbærrar pressu á þróun nýjunga. Það er fídus með föstu umfangi sem verður að fara í loftið og tímamörkin eru óhagganleg. 

„Það er búið að lofa framkvæmdastjórninni þessu og við erum í vondum málum ef við stöndum ekki við okkar hlut“.

Stanslaus pressa þar sem við keyrum hvert verkefnið á fætur öðru með föstum tímamörkum og umfangi leiðir óhjákvæmilega til þess að gæðum er fórnað. Afsláttur af gæðum leiðir til hækkandi tækniskuldar. Hækkandi tækniskuld leiðir til hægari þróunar. Hægari þróun leiðir til frústreraðra stjórnenda sem telja bestu lausnina vera að að setja enn meiri pressu á IT um þróun nýjunga. Vítahringurinn endurtekur sig.

![Breyturnar fjórar](https://s3.eu-west-1.amazonaws.com/olafur.org/four-variables.png)

Í verkefnum sem þessum er stundum talað um [breyturnar fjórar](https://jchyip.medium.com/four-variables-cost-time-quality-scope-f29b4de8bfdf): Kostnað, tímamörk, gæði og umfang. Veldu þrjú atriði en fjórða þarf að vera sveigjanlegt. Að henda meiri pening (fólki) í verkið virkar sjaldan, að færa sífellt tímamörkin er ekki alltaf í boði og gefa afslátt af gæðum er eins og að pissa í skóinn sinn. Skynsamlegast er að umfangið sé sveigjanlegt. Við treystum teyminu til að setja eitthvað gagnlegt í loftið innan ákveðinna tímamarka.

Það þarf reynslumikla forritara og tæknistjórnendur með skýra sýn og bein í nefinu til að rjúfa þennan vítahring.

## DevOps er góður bisness

![](https://s3.eu-west-1.amazonaws.com/olafur.org/devops-handbook.png)

Í bókinni DevOps Handbook er fjallað um rannsókn sem gerð var á árangri fyrirtækja sem hafa tileinkað sér tækni- og vinnuaðferðir DevOps. Árangurinn er augljós nánast hvert sem litið er:

> *Furthermore, high performers were twice as likely to exceed profitability, market share, and productivity goals. And, for those organizations that provided a stock ticker symbol, we found that high performers had 50% higher market capitalization growth over three years. They also had higher employee job satisfaction, lower rates of employee burnout, and their employees were 2.2 times more likely to recommend their organization to friends as a great place to work. High performers also had better information security outcomes. By integrating security objectives into all stages of the development and operations processes, they spent 50% less time remediating security issues.*

*Kim, Gene; Humble, Jez; Debois, Patrick; Willis, John. [The DevOps Handbook](https://www.amazon.com/DevOps-Handbook-World-Class-Reliability-Organizations/dp/1942788002) (pp. 37-38). IT Revolution Press. Kindle Edition.*

Árangur með DevOps er í mínum huga samofinn við nýjan kúltúr og prinsip í stjórnun, tæknilegar aðferðir og skýjalausnir. Það er fyrst og fremst með nýtingu skýjalausna þar sem ofangreind þróun er að eiga sér stað. Stóru tæknifyrirtækin eru þar að gefa okkur aðgang að þeirri tækni sem gerði þeim sjálfum kleift að ná undraverðum árangri.

Spurningin sem stjórnendur ættu að spyrja sig nú: Hef ég efni á að fara ekki í DevOps umbreytingu og skýjavæðingu? Að ákveða að  gera það ekki er ákvörðun um að skerða eigin samkeppnismöguleika.