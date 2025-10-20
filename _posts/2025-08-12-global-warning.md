---
title: Hnattræn hlýnun
description: Hér kafa ég örlítið í eðlisfræðilíkön fyrir hnattrænni hlýnun og hvernig Ísland lítur út í samanburði.
author: mbh
date: 2025-08-10 11:33:00 +0800
categories: [Physics]
tags: [Physics]
pin: false
math: true
image:
  path: /assets/img/global-warming.jpg
  alt: Hnattræn hlýnun. Heimild 
---

## Staðhæfing

Útblástur koltvísýrings af mannavöldum leiðir til aukinnar hlýnunar.

## Einfalt líkan fyrir hitastigi jarðarinnar

Hér er ágætis youtube myndband sem fer yfir þetta:

{% include embed/youtube.html id="gM3dLL6f0ms" %}

Hér er ágætis skýringarmynd, eftir Sabine Hossenfelder, sem útskýrir ferlið sem við erum að fara að skoða:

![Sabine mynd](/assets/img/infographic-greenhouse.jpg)

### Bare rock líkanið eða smástirnislíkanið

Byrjum á því að rifja upp Stefan Boltzmann lögmálið sem segir að útgeislun frá fullkomnum svarthlut er gefið með

$$
P = \sigma A T^4
$$

þar sem  
- $\sigma$ er fasti sem nefnist **Stefan–Boltzmann fastinn**,  
- $A$ er yfirborðsflatarmál hlutarins, oft yfirborðsflatarmál kúlu: $4 \pi r^2$,  
- $T$ er hitastig hlutarins í Kelvin gráðum.

---

Með sama móti má segja að **jörðin geislar frá sér** þar eð hún er sjálf svarthlutur. Þetta kerfi, þar sem sólargeislar lenda á jörðinni og hita hana upp sem sinn eigin svarthlut, nær **varmajafnvægi** sem ákvarðar hitastig jarðar.

Við höfum því að jafnvægi næst þegar

$$
\sigma 4 \pi R_S^2 T_S^4 \cdot \frac{\pi R_J^2}{4 \pi D^2}
=
\sigma 4 \pi R_J^2 T_J^4
$$

þar sem  
- $R_S$ er radíus sólar,  
- $T_S$ er hitastig sólar,  
- $R_J$ er radíus jarðar,  
- $T_J$ er hitastig jarðar,  
- $D$ er fjarlægðin milli sólar og jarðar, stjarnfræðieiningin AU.

---

Með því að leysa fyrir hitastig jarðar fæst

$$
T_J = T_S \sqrt{\frac{R_S}{2 D}} = 278\,\text{K} = 5{,}1^\circ \text{C}
$$

Þar sem við notuðum

- $T_S = 5778\,\text{K}$  
- $R_S = 6{,}95 \times 10^8\,\text{m}$  
- $D = 1{,}5 \times 10^{11}\,\text{m}$

---

Þetta er sem sagt **hitastig jarðar einungis vegna varmajafnvægis við sólina**. Þetta er áður en við bætum við öllum öðrum **umhverfisþáttum** í líkanið, sem geta bæði aukið eða minnkað þetta gildi.

Stærsti þátturinn sem bætist við síðar er **lofthjúpur jarðar**, en aðrir þættir eru til dæmis

- Endurkast sólarljóss af yfirborði jarðar  
- Innri varmageislun jarðar, til dæmis frá kjarna  
- Möndulhalli jarðar hefur áhrif á **staðbundið** en ekki **hnattrænt** hitastig

---

Það er mikilvægt á þessum tímapunkti að benda á að jafnan hér að ofan gefur **mjög gott mat á meðalhitastigi** hnatta sem **hafa engan lofthjúp**. Þess vegna kallast það stundum loftsteinalíkanið.

- Fyrir **Mars** gefur jafnan hér að ofan meðalhitastig á yfirborði um það bil **–52°C**, sem er ekki fjarri raunverulegu meðalhitastigi, –63°C.  
- Fyrir **tunglið** þurfum við að taka með inn í reikninginn bæði **útgeislun frá jörðinni** og **frá sólinni**.

Ef við bætum við stuðli $\alpha$ sem metur endurskinshlutfall hnattarins, það er hversu stórt hlutfall af sólargeisluninni hnötturinn endurkastar frá sér, þá fæst enn betra mat sem er þá gefið með

$$ T_J = \alpha $$

Við sýnum síðan töflu sem metur þessi hitastig fyrir plánetur og tungl í sólkerfinu okkar með og án endurskinshlutfallsins $\alpha$.

table here

Eftir stuttan útreikning fæst þá að hitastig tunglsins er

$$
T_T = \ldots
$$

## loft slagsmál

Það eru nokkrir punktar sem flestir ættu að sammælast um áður en umræða um loftlagsmálin getur hafist.

- Koltvísýringur er gróðurhúsalofttegund en það þýðir að aukinn styrkur koltvísýrings í andrúmsloftinu eykur hitastig jarðarinnar.
- Meðalhitastig jarðarinnar hefur hlýnað frá tímabilinu sem kallast litla ísöldin.
- Mannkynið hefur breytt umhverfinu sínu til dæmis með útblæstri, mannvirkjum og losun úrgangs í sjó.

Ef einhver hafnar ofangreindum punktum þá er lítil ástæða til þess að halda umræðunni áfram. Það sem er hins vegar til umræðu eru eftirfarandi punktar

- Mannfólk er **helsti** áhrifavaldur í hnattrænni hlýnun.
- Hlýnun jarðar er slæm fyrir framtíðarhorfur mannkynsins.

Þetta eru punktarnir sem eru til umræðu. Til að vísa í Richard Feynman  
I would rather have questions that cannot be answered than answers that cannot be questioned.  
Það er síðan heil umræða í kringum það hvort að seinni tveir punktarnir eru eitthvað sem stjórnmálamenn hafa verið að advókera fyrir eða hvort að sérfræðingarnir sem rannsaka hnattræna hlýnun myndu vera sammála síðustu tveimur punktunum. Hér þarf að skoða greinar sem tala um viðhorf sérfræðinga á hnattræna hlýnun og hvort að þeir myndu segja að það væru marktækar sönnur fyrir seinni tveimur punktunum.

## Hverjar eru helstu gróðurhúsalofttegundirnar

- Vatnsgufa
- Koltvísýringur
- Metangas

## Greinar sem mig langar að lesa

Hér er ágætis youtube myndband sem fer yfir þetta

{% include embed/youtube.html id="gM3dLL6f0ms" %}

https://www.youtube.com/watch?v=gM3dLL6f0ms

https://arxiv.org/pdf/1802.02695

## Hvers vegna skiptir koltvísýringur máli

Við skoðum nú einfalt líkan þar sem við bætum við lofthjúp og skoðum hvernig mismunandi gildi á koltvísýring í efnasamsetningu lofthjúpsins breyta hitastiginu.

## Er koltvísýringur að aukast

## Hvað myndi gerast ef allur ís jarðarinnar myndi bráðna

## En við búum á Íslandi, ættum við ekki að fagna hnattrænni hlýnun

Nei. Golfstraumurinn mun hverfa. Skoðum það líkan örlítið.

## Guðfinna Aðalgeirsdóttir

Sá Íslendingur sem hefur eflaust starfað mest 
