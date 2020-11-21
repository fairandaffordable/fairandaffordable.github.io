---
title: What we do
subtitle: Data Sharing
layout: page
show_sidebar: false
menubar: example_menu
---

## List of reimbursed pharmaceutical products

The list of reimbursed medicinal products is updated every month in each country participating in FaAP. These lists are maintaned by different entities in each country (links are provided for the actual sources below):
* Poland - [Ministry of Health](https://www.gov.pl/web/zdrowie/obwieszczenia-ministra-zdrowia-lista-lekow-refundowanych?target=_blank) 
* Czech Republic - [State Institute for Drug Control](http://www.sukl.cz/sukl/seznam-leciv-a-pzlu-hrazenych-ze-zdrav-pojisteni?target=_blank)
* Slovakia - [Ministry of Health](https://www.mzsr.sk/?zoznam-kategorizovanych-liekov?target=_blank)
* Lithuania - [National Health Insurance Fund](http://www.vlk.lt/privalomojo-sveikatos-draudimo-taryba/privalomojo-sveikatos-draudimo-tarnybos-nutarimai?target=_blank)
* Hungary - [National Health Insurance Fund](http://neak.gov.hu/felso_menu/szakmai_oldalak/gyogyszer_segedeszkoz_gyogyfurdo_tamogatas/egeszsegugyi_vallalkozasoknak/pupha/Vegleges_PUPHA.html?target=_blank)

## Products undergoing evaluation

This section demonstrates products undergoing evaluation in each of the participating countries. The data in the tables below are sourced from local datasets from each country and updated regulary.

### Poland

The table below for products undergoing evaluation is populated by then [data source](https://bipold.aotm.gov.pl?target=_blank) maintained by AoTMiT.

<table id="table_id">
<thead>
<tr>
<th>Product</th>
<th>Submission Date</th>
</tr>
</thead>
{% for gyogyszer in site.data.neak_gyogyszerek %}
  <tr>
    <td>{{gyogyszer.Product}}</td>
    <td>{{gyogyszer.Submission}}</td>
  </tr>
{% endfor %}
</table>



### Hungary

The products undergoing evaluation are published by the National Health Insurance Fund. [This data](www.neak.gov.hu/felso_menu/szakmai_oldalak/gyogyszer_segedeszkoz_gyogyfurdo_tamogatas/egeszsegugyi_vallalkozasoknak/gyartok_forgalomba_hozok/KERELEM_IND_ELJ_GYOGYSZ_TAPSZ.html7?target=_blank) is used to generate and populate the table below on product names and submission dates.

<table id="table_id4">
<thead>
<tr>
<th>Product</th>
<th>Submission Date</th>
</tr>
</thead>
{% for gyogyszer in site.data.aotmit_gyogyszerek %}
  <tr>
    <td>{{gyogyszer.Product}}</td>
    <td>{{gyogyszer.Submission}}</td>
  </tr>
{% endfor %}
</table>

### Lithuania

The products undergoing evaluation are published by the State Medicines Control Agency of Lithuania (VVKT). [This data](https://vvkt.lt/index.php?2442135045) is used to generate and populate the table below on products (with ICD-10 codes) and submission dates.

<table id="table_id3">
<thead>
<tr>
<th>Product (ICD-10 code)</th>
<th>Submission Date</th>
</tr>
</thead>
{% for gyogyszer in site.data.vvkt_gyogyszerek %}
  <tr>
    <td>{{gyogyszer.Product}}</td>
    <td>{{gyogyszer.Submission}}</td>
  </tr>
{% endfor %}
</table>

### Slovakia

### Czech Republic

The products undergoing evaluation are published by the State Institute for Drug Control (SÚKL). [This data](http://www.sukl.cz/sukl/prehled-spravnich-rizeni?target=blank) is used to generate and populate the table below on product names and submission dates.

<table id="table_id2">
<thead>
<tr>
<th>Product</th>
<th>Submission Date</th>
</tr>
</thead>
{% for gyogyszer in site.data.sukl_gyogyszerek %}
  <tr>
    <td>{{gyogyszer.Product}}</td>
    <td>{{gyogyszer.Submission}}</td>
  </tr>
{% endfor %}
</table>
