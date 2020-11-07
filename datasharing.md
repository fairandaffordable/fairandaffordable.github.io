---
title: What we do
subtitle: Data Sharing
layout: page
show_sidebar: false
menubar: example_menu
---

## List of reimbursed pharmaceutical products


## Products undergoing evaluation

This section demonstrates products undergoing evaluation in each of the participating countries. The data in the tables below are sourced from local datasets from each country and updated regulary.

### Poland

### Hungary

The products undergoing evaluation are published by the National Health Insurance Fund. [This data](www.neak.gov.hu/felso_menu/szakmai_oldalak/gyogyszer_segedeszkoz_gyogyfurdo_tamogatas/egeszsegugyi_vallalkozasoknak/gyartok_forgalomba_hozok/KERELEM_IND_ELJ_GYOGYSZ_TAPSZ.html7?target=_blank) is used to generate and populate the table below on product names and submission dates.

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
