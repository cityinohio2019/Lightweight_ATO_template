id: ssp_v1
format: markdown
title: SSP v1
...
<style type="text/css" scoped>
  h2 { border-bottom:1px solid #888; }
  h3 { border-bottom:0.5px solid #aaa; }
  h4 { font-weight:bold; font-size:0.9em; }
  blockquote { color: #666; font-size:0.8em;}
  .notice {color: red; font-size:3.0em; text-align:center; transform: scaleY(.85);
  font-weight: bold;}
  table, th, td { border: 1px solid #888; }
  th, td { padding: 15px; text-align: left;}
</style>

<!-- Cover page -->
<center>

FOR OFFICIAL USE ONLY

DEPARTMENT OF HOMELAND SECURITY


{{ project.system_profile.system_basics.system_name }}
System Security Plan (SSP)

**Updated (Date Information)**

**System Name:**  
**{{project.system_info.system_name}} {% if project.system_info.system_short_name %} ({{project.system_info.system_short_name}}){% endif %}**


<table border='3' width="400">
<tr><td>
<p>This document contains Sensitive Material
and is exempted from release under the Freedom of Information Act
by Exemption b(2).</p>
<p>Staff reviewing this document must hold a minimum of Public Trust
Level 1c clearance.</p>
</tr></td>
</table> 

<div style="height: 400px;">
  <!-- Spacer for cover page -->
</div>

* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *

</center>
<!-- /Cover page -->

<!-- System Information -->
<h2>1. System Information</h2>

{{project.system_info.output_documents.system_info}}

<!-- /System Information -->

<!-- Security Controls -->
<h2>2. Security Controls</h2>

<div>
{{project.se_cace_elk}}{% if project.se_cace_elk %}

  {% for od in project.se_cace_elk.output_documents %}
  {% set odl = od.split('_') %}
  {% if 'test' in odl %}
  {% else %}
  {% set c_name = "{}-{}".format(odl[3].upper(), " ".join(odl[4:])) %}
  <h4>Control {{c_name}}</h4>
    {{project.se_cace_elk.output_documents[od]}}
  {% endif %}
  {% endfor %}
{% endif %}
</div>

<!-- /Security Controls -->

