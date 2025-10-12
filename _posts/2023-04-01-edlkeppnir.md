---
title: Eðlisfræðikeppni framhaldsskólanna
description: Eðlisfræðikeppni framhaldsskólanna
author: mbh
date: 2023-04-01 20:00:00 +0800
categories: [Eðlisfræðikeppnir]
tags: [Eðlisfræðikeppnir]
pin: false
math: true
image:
  path: /assets/img/edlkeppni98.jpeg
  alt: Eðlisfræðikeppni framhaldsskólanna
---

## Mitt hlutverk

Ég hef verið listjóri fyrir íslenska Ólympíuliðið í eðlisfræði frá árinu 2019. Núverandi stjórnarmeðlimir eru Viðar Ágústsson, Ingibjörg Haraldsdóttir, Matthias Harksen og Unnar Bjarni Arnalds.

<style>
  /* ljós hamur sjálfgefið */
  table { width: 100%; border-collapse: collapse; }
  th, td { border: 1px solid #ddd; padding: 8px; text-align: center; }
  th { background-color: #f4f4f4; }
  @media screen and (max-width: 600px) {
    table { display: block; overflow-x: auto; white-space: nowrap; }
  }
  /* dökkur hamur með bæði kerfi og Chirpy rofa */
  @media (prefers-color-scheme: dark) {
    table { color: #e6e6e6; }
    th, td { border-color: rgba(255,255,255,0.18); }
    th { background-color: rgba(255,255,255,0.06); }
    a { color: #9ecbff; }
  }
  html[data-theme="dark"] table { color: #e6e6e6; }
  html[data-theme="dark"] th, html[data-theme="dark"] td { border-color: rgba(255,255,255,0.18); }
  html[data-theme="dark"] th { background-color: rgba(255,255,255,0.06); }
  html[data-theme="dark"] a { color: #9ecbff; }
</style>

## Forkeppnin

Á hverju ári er haldin forkeppni til að skera úr um hverjum eigi að bjóða í úrslitakeppnina.

<table>
  <tr>
    <th>Keppni</th>
    <th>Lausnir</th>
  </tr>

  {% assign years = (3..25) | reverse %}
  {% for i in years %}
    {% assign year = i | plus: 2000 %}
    {% assign fn = i %}{% if i < 10 %}{% assign fn = "0" | append: i %}{% endif %}
    {% assign file = "/assets/pdfs/forkeppnir/undankeppni" | append: fn | append: ".pdf" | relative_url %}
    {% assign sol  = "/assets/pdfs/forkeppnir/Lausnir/undankeppni" | append: fn | append: "-lausn.pdf" | relative_url %}
    <tr>
      <td><a href="{{ file }}" target="_blank">Forkeppni {{ year }}</a></td>
      <td>{% if i >= 19 %}<a href="{{ sol }}" target="_blank">Lausnir</a>{% else %}-{% endif %}</td>
    </tr>
  {% endfor %}
</table>

## Lokakeppnin

Efstu 16 keppendum í forkeppninni er boðið í fræðilega og verklega úrslitakeppni. Efstu keppendum verður síðan boðið í Ólympíulið Íslands í eðlisfræði það sumarið.

<table>
  <tr>
    <th>Keppni</th>
    <th>Lausnir</th>
  </tr>

  {% assign years = (3..25) | reverse %}
  {% for i in years %}
    {% assign year = i | plus: 2000 %}
    {% assign fn = i %}{% if i < 10 %}{% assign fn = "0" | append: i %}{% endif %}
    {% assign file = "/assets/pdfs/lokakeppnir/fraedileg" | append: fn | append: ".pdf" | relative_url %}
    {% assign sol  = "/assets/pdfs/lokakeppnir/lausnir/fraedileg" | append: fn | append: "-lausn.pdf" | relative_url %}
    <tr>
      <td><a href="{{ file }}" target="_blank">Lokakeppni {{ year }}</a></td>
      <td>{% if i >= 16 %}<a href="{{ sol }}" target="_blank">Lausnir</a>{% else %}-{% endif %}</td>
    </tr>
  {% endfor %}
</table>

## IPhO

Næstu alþjóðlegu Ólympíuleikar í eðlisfræði verða í

- Kólumbíu 2026  
- Ungverjalandi 2027  
- Suður Kóreu 2028  
- Ekvador 2029  

Hér má sjá gamlar keppnir ásamt lausnum.

## EuPhO

Hér má sjá gamlar keppnir ásamt íslenskum þýðingum og lausnum.

<table>
  <tr>
    <th>Ár</th>
    <th>Fræðilegt</th>
    <th>Verklegt</th>
    <th>Lausnir</th>
  </tr>

  {% assign years = (17..25) | reverse %}
  {% for y in years %}
    {% assign base = "/assets/pdfs/eupho/" | relative_url %}
    {% assign sol  = "/assets/pdfs/eupho/lausnir/" | relative_url %}
    <tr>
      <td>20{{ y }}</td>
      <td><a href="{{ base }}eupho{{ y }}-t-isl.pdf" target="_blank">[IS]</a> / <a href="{{ base }}eupho{{ y }}-t-eng.pdf" target="_blank">[EN]</a></td>
      <td><a href="{{ base }}eupho{{ y }}-e-isl.pdf" target="_blank">[IS]</a> / <a href="{{ base }}eupho{{ y }}-e-eng.pdf" target="_blank">[EN]</a></td>
      <td><a href="{{ sol }}eupho{{ y }}-t-sol.pdf" target="_blank">[Fræðilegt]</a> / <a href="{{ sol }}eupho{{ y }}-e-sol.pdf" target="_blank">[Verklegt]</a></td>
    </tr>
  {% endfor %}
</table>

Fyrir verklega hlutana frá 2020 og 2021 bendum við á eftirfarandi forrit

<table>
  <tr>
    <th>Verkefni</th>
    <th>Windows</th>
    <th>MacOS</th>
    <th>Linux</th>
  </tr>
  <tr>
    <td>E1 — Hidden Charge 2020</td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2020/E1-hidden-charge-WIN.exe' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2020/E1-hidden-charge-OSX' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2020/E1-hidden-charge-Linux' | relative_url }}" download>Download</a></td>
  </tr>
  <tr>
    <td>E2 — Black Box 2020</td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2020/E2-black-box-WIN.exe' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2020/E2-black-box-OSX' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2020/E2-black-box-Linux' | relative_url }}" download>Download</a></td>
  </tr>
  <tr>
    <td>E1 — Hidden Wire 2021</td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2021/E1_hidden_wire_win.exe' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2021/E1_hidden_wire_osx' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2021/E1_hidden_wire_linux' | relative_url }}" download>Download</a></td>
  </tr>
  <tr>
    <td>E2 — Hot Cylinder 2021</td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2021/E2_hot_cylinder_win.exe' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2021/E2_hot_cylinder_osx' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2021/E2_hot_cylinder_linux' | relative_url }}" download>Download</a></td>
  </tr>
</table>

Forritin eru skipanalínuforrit og eru aðgengileg fyrir Linux, MacOS og Windows. Hafið samband ef þið náið ekki að keyra þau. Á Mac og Linux gæti þurft að nota **chmod +x skráarnafn**.

## Aðrar keppnir

Það eru fleiri keppnir sem fólk getur tekið þátt í og gagnlegt er að skoða

- OPhO
- APhO
- BCAUPC
- INPhO
- USAPhO
