---
title: Eddington tilraunin
description: Er hægt að nota sólmyrkva til þess að staðfesta almennu afsæðiskenninguna?
author: mbh
date: 2024-08-12 11:33:00 +0800
categories: [Outreach]
tags: [Outreach]
pin: true
math: true
image:
  path: /assets/img/einstein-eddington.jpg
  alt: Þjóðverjinn Albert Einstein (vinstri) og Bretinn Arthur Eddington (hægri) hittast eftir fyrri heimsstyrjöldina til að ræða tilraunina sem að Eddington framkvæmdi sem að staðfesti almennu afsæðiskenninguna. Síðan þá hafa fjölmargar tilraunir verið gerðar til að staðfesta almennu afstæðiskenninguna.
---

Á þrítugsafmælinu mínu, 12. ágúst 2026, verður almyrkvi á sólu. Hann mun sjást á vestanverðu landinu, meðal annars á höfuðborgarsvæðinu en í Reykjavík mun hann endast í 59 sekúndur. Besta útsýnið verður þó líklegast á Snæfelsnesinu og á Vestfjörðum. Sólmyrkvinn mun vara lengst á Látrabjargi, eða í 2 mínútur og 13 sekúndur.

Ég ætla að framkvæma Eddington tilraunina á afmælinu mínu. Það er kannski viðeigandi því að ég stunda rannsóknir á svartholum en tilvist þeirra er spáð fyrir um af almennu afstæðiskenningunni sem að Alberts Einstein setti fram árið 1915 í miðri fyrri heimsstyrjöldinni. Það þótti eftirtektarvert á þeim tíma þegar að Bretinn, Arthur Eddington, staðfesti með mælingu á sólmyrkva árið 1919, í fyrsta sinn kenningu Einstein.

Í þessari bloggfærslu ætla ég að rekja svolítið hvaða lore liggur á bak við þessa merku tilraun, svo ætla ég að útskýra hvernig að við Stjörnu-Sævar ætlum að framkvæma þessa tilraun í sólmyrkvanum 2026. Áhugasamir sem að vilja aðstoða við að framkvæma þessa eða aðrar mælingar í sólmyrkvanum eru beðnir um að hafa samband við mig á netfangi matthias.harksen[hjá]gmail.com.

Sjá einnig: https://www.mathpages.com/rr/s6-03/6-03.htm

## Tvær Newtonskar útleiðslur á ljóssveigju

Það er engin sérstaða í því að ljós sveigi í kringum sólina. Reyndar spáir Newtonska aflfræðin einnig fyrir að ljós muni sveigja í kringum sólina. Hinsvegar munar faktor tveimur á kenningunum sem var það sem að Eddington tilraunin skar úr um til að greina hvort kenningin væri nákvæmari í þessu atriði.

Fyrsta útleiðslan byggir á [newtonian-deflection.pdf](/assets/files/newtonian-deflection.pdf) og hin er byggð á [0508030.pdf](/assets/files/0508030.pdf).

![Ljóssveigja samkvæmt tveimur kenningum](/assets/img/svg/ljossveigja.svg){: .w-100 .mx-auto .d-block }

Lítum á ögn með massa $m$ sem byrjar með upphafshraða $v_0$ í $x = -\infty$ og $y=0$. Látum massa $M \geq m$ vera staðsetann í $(0,b)$ þar sem að $b$ er svokölluð kennilengd árekstrarins (e. *impact parameter*). Eini krafturinn sem að verkar á massann $m$ í þessu ferli er þyngdarkrafturinn. Það er fræg niðurstaða eftir Newton að einu hugsanlegu ferlarnar sem koma til greina fyrir hreyfingu agnarinnar í slíku miðlægu mætti eru keilusniðin. Það fer eftir gildinu á $v_0$ hvort að hreyfingin verður sporbaugur eða breiðbogi. Við athugum að í punkti $(x,y)$ þá er þyngdarkrafturinn sem að verkar á ögnina með massa $m$ gefinn með:

$$ \vec{F}_G = \frac{GMm}{(x^2+(y-b)^2)^{3/2}} \begin{pmatrix} x \\ y-b \end{pmatrix} $$

En heildarkrafturinn er tengdur skriðþungabreytingunni samkvæmt $\vec{F}_{\text{heild}} = \frac{d \vec{p}}{dt} = \vec{F}_G$. Varðveislulögmálin segja okkur síðan að heildarhverfiþunginn sé varðveittur þannig að

$$ mv_0 b = L = (\vec{r} \times \vec{p})_z = m(x v_y - y v_x) $$

og það að heildarorkan sé varðveitt segir okkur að

$$ \frac{1}{2}mv_0^2 = E = \frac{1}{2}m (v_x^2 + v_y^2) - \frac{GMm}{\sqrt{x^2+(y-b)^2}}  $$

Við getum litið á hverfiþungavarðveisluna og orkuvarðveisluna sem jöfnuhneppi sem leyfir okkur að ákvarða breytistærðirnar $v_x = \frac{dx}{dt}$ og $v_y = \frac{dy}{dt}$ sem fall af $x,y$. Með það í huga þá sjáum við eftir smá algebru að $v_y = \frac{1}{x}(v_0 b + v_x y)$ og með því að stinga því inn í orkujöfnuna við fáum eftirfarandi $2.$ stigs margliðu fyrir $v_x$

$$(1+\frac{y^2}{x^2})v_x^2 + \frac{2v_0 b y}{x^2} v_x  + v_0^2 (\frac{b^2}{x^2}-1) - \frac{2GM}{\sqrt{x^2 + (y-b)^2}} = 0 $$

sem gefur því að

$$ v_x = \frac{-v_0 b y \pm x v_0 \sqrt{x^2+y^2 - b^2 + \frac{2GM}{v_0^2} \frac{x^2+y^2}{\sqrt{x^2+(y-b)^2}}}}{x^2+y^2}$$

En við athugum svo að með keðjureglunni má umrita lárétta þáttinn þannig að

$$ F_x = \frac{dp_x}{dt} = \frac{dp_x}{dx} \frac{dx}{dt} + \frac{dp_x}{dy} \frac{dy}{dt} = \frac{dp_x}{dx}v_x + \frac{dp_x}{dy}v_y $$

og eins fæst fyrir lóðrétta þáttinn

$$ F_y = \frac{dp_y}{dt} = \frac{dp_y}{dx} \frac{dx}{dt} + \frac{dp_y}{dy} \frac{dy}{dt} = \frac{dp_y}{dx}v_x + \frac{dp_y}{dy}v_y $$

þar sem að þættir kraftsins $F_x$ og $F_y$ eru þekktir samkvæmt þyngdarlögmálinu og $v_x$ og $v_y$ þekkt þá má nota þetta til þess að ákvarða 




## Almenna afstæðiskenningin 1915


## Eddington tilraunin 1919



## Afmælistilraunin 2026


