---
title: What we do
subtitle: Data Sharing
layout: page
show_sidebar: false
menubar: example_menu
---

### Key stakeholders in decision making

| Country       | Financing agent| Health Technology Assessment | Ministry of Health|
|---------------|----------------|------------------------------|-------------------|
| Poland        | [Narodowy Fundusz Zdrowia (NFZ)](http://www.nfz.gov.pl/) | [Agencja Oceny Technologii Medycznych i Taryfikacji (AOTMiT)](http://www.aotm.gov.pl/www/) | [Ministerstwo Zdrowia Rzeczypospolitej Polskiej (MZRP)](https://www.gov.pl/web/zdrowie/) |
| Hungary       | [Nemzeti Egészségbiztosítási Alapkezelő (NEAK)](http://www.neak.gov.hu) | [Országos Gyógyszerészeti és Élelmezés-egészségügyi Intézet (OGYÉI)](https://ogyei.gov.hu/tei) | [Emberi Erőforrások Minisztériuma (EMMI)](https://www.kormany.hu/hu/emberi-eroforrasok-miniszteriuma) |
| Lithuania     | [Valstybinė Ligonių Kasa (VLK)](http://www.vlk.lt/) | [Valstybiné Akreditavimo Sveikatos Prieziuros Veiklai Tarnyba (VASPVT)](http://www.vaspvt.gov.lt/) | [Lietuvos Respublikos sveikatos Apsaugos Ministerija (LRSAM)](http://sam.lrv.lt/lt/) |
| Slovakia      | [Všeobecná Zdravotná Poisťovňa (VsZP)](https://www.vszp.sk/) | [TBA]() | [Ministerstvo zdravotníctva Slovenskej Republiky (MZSR)](https://www.health.gov.sk/Titulka) |
| Czech Republic| [Všeobecná Zdravotní Pojišťovna (VZP)](https://www.vzp.cz/) | [Státní Ústav Pro Kontrolu Léčiv (SÚKL)](http://www.sukl.cz/) | [Ministerstvo zdravotnictví České Republiky (MZCR)](https://www.mzcr.cz/) |

### Products undergoing evaluation

This section demonstrates products undergoing evaluation in each of the participating countries.

#### Hungary

The products undergoing evaluation are published by the National Health Insurance Fund. This data is used to generate and populate the table below on product names and submission dates.

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
