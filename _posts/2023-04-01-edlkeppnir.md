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
  table { width: 100%; border-collapse: collapse; }
  th, td { border: 1px solid #ddd; padding: 8px; text-align: center; }
  th { background-color: #f4f4f4; }
  @media screen and (max-width: 600px) {
    table { display: block; overflow-x: auto; white-space: nowrap; }
  }
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

    {% assign file = "/assets/pdfs/forkeppnir/undankeppni" | append: fn | append: ".pdf" %}
    {% assign sol  = "/assets/pdfs/forkeppnir/Lausnir/undankeppni" | append: fn | append: "-lausn.pdf" %}

    {% assign exam_exist = site.static_files | where: "path", file | first %}
    {% if exam_exist %}
      <tr>
        <td><a href="{{ file | relative_url }}" target="_blank">Forkeppni {{ year }}</a></td>
        <td>
          {% assign sol_exist = site.static_files | where: "path", sol | first %}
          {% if sol_exist %}<a href="{{ sol | relative_url }}" target="_blank">Lausnir</a>{% else %}–{% endif %}
        </td>
      </tr>
    {% endif %}
  {% endfor %}
</table>

## Lokakeppnin

Efstu sextán úr forkeppninni fara í fræðilega og verklega lokakeppni. Efstu þátttakendum er síðan boðið í Ólympíulið Íslands í eðlisfræði að sumri.

<table>
  <tr>
    <th>Keppni</th>
    <th>Lausnir</th>
  </tr>

  {% assign years = (3..25) | reverse %}
  {% for i in years %}
    {% assign year = i | plus: 2000 %}
    {% assign fn = i %}{% if i < 10 %}{% assign fn = "0" | append: i %}{% endif %}

    {% assign file = "/assets/pdfs/lokakeppnir/fraedileg" | append: fn | append: ".pdf" %}
    {% assign sol  = "/assets/pdfs/lakakeppnir/lausnir/fraedileg" | append: fn | append: "-lausn.pdf" %}

    {% assign exam_exist = site.static_files | where: "path", file | first %}
    {% if exam_exist %}
      <tr>
        <td><a href="{{ file | relative_url }}" target="_blank">Lokakeppni {{ year }}</a></td>
        <td>
          {% assign sol_exist = site.static_files | where: "path", sol | first %}
          {% if sol_exist %}<a href="{{ sol | relative_url }}" target="_blank">Lausnir</a>{% else %}–{% endif %}
        </td>
      </tr>
    {% endif %}
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

    {% assign t_is = "/assets/pdfs/eupho/eupho" | append: y | append: "-t-isl.pdf" %}
    {% assign t_en = "/assets/pdfs/eupho/eupho" | append: y | append: "-t-eng.pdf" %}
    {% assign e_is = "/assets/pdfs/eupho/eupho" | append: y | append: "-e-isl.pdf" %}
    {% assign e_en = "/assets/pdfs/eupho/eupho" | append: y | append: "-e-eng.pdf" %}
    {% assign s_t  = "/assets/pdfs/eupho/lausnir/eupho" | append: y | append: "-t-sol.pdf" %}
    {% assign s_e  = "/assets/pdfs/eupho/lausnir/eupho" | append: y | append: "-e-sol.pdf" %}

    <tr>
      <td>20{{ y }}</td>

      <td>
        {% assign t_is_ok = site.static_files | where: "path", t_is | first %}
        {% assign t_en_ok = site.static_files | where: "path", t_en | first %}
        {% if t_is_ok %}<a href="{{ t_is | relative_url }}" target="_blank">[IS]</a>{% else %}[IS]{% endif %}
        /
        {% if t_en_ok %}<a href="{{ t_en | relative_url }}" target="_blank">[EN]</a>{% else %}[EN]{% endif %}
      </td>

      <td>
        {% assign e_is_ok = site.static_files | where: "path", e_is | first %}
        {% assign e_en_ok = site.static_files | where: "path", e_en | first %}
        {% if e_is_ok %}<a href="{{ e_is | relative_url }}" target="_blank">[IS]</a>{% else %}[IS]{% endif %}
        /
        {% if e_en_ok %}<a href="{{ e_en | relative_url }}" target="_blank">[EN]</a>{% else %}[EN]{% endif %}
      </td>

      <td>
        {% assign s_t_ok = site.static_files | where: "path", s_t | first %}
        {% assign s_e_ok = site.static_files | where: "path", s_e | first %}
        {% if s_t_ok %}<a href="{{ s_t | relative_url }}" target="_blank">[Fræðilegt]</a>{% else %}[Fræðilegt]{% endif %}
        /
        {% if s_e_ok %}<a href="{{ s_e | relative_url }}" target="_blank">[Verklegt]</a>{% else %}[Verklegt]{% endif %}
      </td>
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
    <td>Eitt falin hleðsla 2020</td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2020/E1-hidden-charge-WIN.exe' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2020/E1-hidden-charge-OSX' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2020/E1-hidden-charge-Linux' | relative_url }}" download>Download</a></td>
  </tr>

  <tr>
    <td>Tveir svarti kassi 2020</td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2020/E2-black-box-WIN.exe' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2020/E2-black-box-OSX' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2020/E2-black-box-Linux' | relative_url }}" download>Download</a></td>
  </tr>

  <tr>
    <td>Eitt falin vír 2021</td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2021/E1_hidden_wire_win.exe' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2021/E1_hidden_wire_osx' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2021/E1_hidden_wire_linux' | relative_url }}" download>Download</a></td>
  </tr>

  <tr>
    <td>Tveir heitur sívalningur 2021</td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2021/E2_hot_cylinder_win.exe' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2021/E2_hot_cylinder_osx' | relative_url }}" download>Download</a></td>
    <td><a href="{{ '/assets/pdfs/eupho/exp-eupho2021/E2_hot_cylinder_linux' | relative_url }}" download>Download</a></td>
  </tr>
</table>

Forritin eru skipanalínuforrit og aðgengileg fyrir Linux, MacOS og Windows. Hafið samband ef ykkur tekst ekki að keyra þau. Á Mac og Linux gæti þurft að nota **chmod +x skráarnafn**.

## Aðrar keppnir

Það eru fleiri keppnir sem hægt er að taka þátt í og gagnlegt er að skoða

- OPhO
- APhO
- BCAUPC
- INPhO
- USAPhO
