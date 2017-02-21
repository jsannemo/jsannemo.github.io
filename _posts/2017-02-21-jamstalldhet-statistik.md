---
layout: post
description: Vad är "mest jämställt"? En riksdag med 43.6% kvinnor eller en Melodifestival med 100% vita programledare?
title: "Jämställdhet och statistik"
---

Intuitivt kanske man tycker att det senare är mer problematiskt. I [Gomorron Sverige](http://www.svtplay.se/video/12366054/gomorron-sverige/gomorron-sverige-17-feb-06-25?start=auto) (inslaget börjar ca 2:15h) tycktes det lite kort att "det är för vitt" bland Melodifestivalprogramledarna, något som fick omnämnanden i skvallerpressen efteråt ([Aftonbladet](http://www.aftonbladet.se/nojesbladet/melodifestivalen/a/4azmV/kritiken-hasse-verkar-bakom-flotet), [Expressen](http://www.expressen.se/noje/harda-kritiken-mot-svt-ar-for-vitt/)). 43.6% är ju trots allt "nästan" hälften, medan 0% icke-vita är en klar underrepresentation. Hur händer det?

Till riksdagen får den som fyller 18 senast på valdagen, samt är eller har varit folkbokförd i Sverige kandidera.
2013 uppgick detta till c:a 3 443 tusen män och 3 593 tusen kvinnor ([Andel vuxna kvinnor och män, SCB](http://www.statistikdatabasen.scb.se/pxweb/sv/ssd/START__HE__HE0103__HE0103B/Vuxna/table/tableViewLayout1/?rxid=46f3b4f0-fb63-418e-ad3b-9fe455eca89f)). Detta ger ungefär 48.9% män och 51.1% kvinnor. I valet 2014 valdes dock 152 (43.6%) kvinnor och 197 (56.4%) män in i riksdagen ([Andel kvinnliga och manliga ledamöter efter valet 2014 SCB](http://www.scb.se/sv_/Hitta-statistik/Statistik-efter-amne/Demokrati/Allmanna-val/Allmanna-val-nominerade-och-valda/12352/12359/Behallare-for-Press/386623/)). Kvinnor är med andra ord underrepresenterade med hela 5.3 procentenheter mot andelen kvinnor som får kandidera.

Om vi antar att varje riksdagsledamot är ett oberoende val urval med hela befolkningen som population förväntar vi oss att antalet kvinnor följer en [binomialfördelning](https://en.wikipedia.org/wiki/Binomial_distribution) med \\(n = 349\\) och \\(p = 0.511\\). 

<p align="center">
<img align="center" alt="Sannolikhetsfördelning över antal kvinnliga ledamöter" src="https://lh3.googleusercontent.com/-URdB2rZxYO8/WKx3B_rxkgI/AAAAAAAAGQE/y54abfhEktUtbekQcBhbAq-O-egG4qVRgCLcB/s0/Screenshot+from+2017-02-21+18-20-19.png">
</p>

Sannolikheten att högst 152 kvinnliga ledamöter väljs in under det antagendet är 0.0028, vilket är löjligt liten. Inte blir det bättre av att detta var den andra minskningen av andel kvinnor i rad. 2006 hade riksdagen hela 47.3% kvinnor,  och 2010 något mindre med 45.0%. Med andra ord kan hypotesen att kvinnors underrepresentation i riksdagen bara är på grund av slumpen förkastas med rätt hög sannolikhet.

Andelen vita och icke-vita svenskar är svårare att hitta statistik över. Tobias Hübinette sätter i en [debattartikel från 2015](http://www.aftonbladet.se/debatt/article20439966.ab) andelen med "någon form av bakgrund i Afrika, Asien eller Latinamerika" till 15%. [SCB](http://www.scb.se/Statistik/BE/BE0101/2010A01L/Utrikes_fodda.pdf) gav 2010 andelen "inrikes födda med två inrikes födda föräldrar" till 74% (men poängterar att en stor andel med den sortens utom-svensk bakgrund är finska invandrare, som nog till största del är vita). Om vi använder det första alternativet som uppskattning för andel vita får vi därmed 85%, och 74% som den andra, så låt oss säga 74% vita som en pessimistisk skattning (i meningen att den maximerar underrepresentationen).

Utifrån samma antangande (att varje programledare väljs uniformt ur hela populationen) är sannolikheten att tre vita programledare väljs under en och samma Melodifestival lika med \\(0.74^3 = 0.405\\). Givet Melodifestivaler med 3 programledare förväntar vi oss alltså att ungefär 40% av dessa har just tre vita programledare.

För att kunna säga något konkret om underrepresentation måste vi titta under  en lite längre period. Låt oss istället titta på alla [programledare under 2010-talet](https://sv.wikipedia.org/wiki/Melodifestivalen#2010-talet).  Antalet programledare har under dessa år varit:

- 2010: 3 vita, 0 icke-vita
- 2011: 2 vita, 0 icke-vita
- 2012: 2 vita, 1 icke-vit
- 2013: 1 vit, 1 icke-vit
- 2014: 1 vit, 1 icke-vit
- 2015: 2 vita, 0 icke-vita
- 2016: 6 vita, 2 icke-vita
- 2017: 3 vita, 0 icke-vita

Totalt sett är detta 20 vita programledare och 5 icke-vita programledare, d.v.s 80% vita programledare och 20% icke-vita programledare. Motsvarande sannolikhetsfördelning blir då:

<p align="center">
<img align="center" alt="Sannolikhetsfördelning över antal icke-vita programledare" src="https://lh3.googleusercontent.com/-OAXypkYRdeU/WKx-jRujo1I/AAAAAAAAGQg/rmmTimZV4e8-_CQQKZUtYixN5r6L8PzkACLcB/s0/Screenshot+from+2017-02-21+18-52-38.png">
</p>

Sannolikheten att få högst 5 icke-vita programledare är då ca 0.334, d.v.s. vi förväntar oss den underrepresentationen varje tredje gång detta väljs. Med andra ord är detta ett ganska troligt scenario, och säger inte jättemycket om huruvida SVT väljer vita programledare till Melodifestivalen i större grad än vad man förväntar sig. Det kan lika gärna vara ett statistiskt fenomen.

Vad är poängen med den här texten? Statistik och sannolikhetslära är ofta icke-intuitiv, och avvikelser från vad man förväntar sig kan förvåna. Även om underrepresentationen av icke-vita i årets Melodifestival (26 procentenheter) - eller till och med senaste 8 årens Melodifestivaler (6 procentenheter) - är större än underrepresentationen av kvinnor i riksdagen (bara 5.3 enheter), är det senare (än så länge) mer skevt. Med ett så stort urval som riksdagen har är det väldigt tydligt att något är fel, medan en till synes större underrepresentation med ett så litet urval som Melodifestivalen är svårare att tyda något ur.
