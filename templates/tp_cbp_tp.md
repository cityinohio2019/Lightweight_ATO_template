id: tp_cbp_tp
format: markdown
title: CBP Test Plan
...
<style type="text/css" scoped>
    h2 { border-bottom:1px solid #888; }
    h3 { border-bottom: 0.5px solid #aaa; }
    h4 { margin-top: 15px; font-weight: bold; font-size: 1em; }
    blockquote { color: #666; font-size:0.8em; margin: 0 10px; }
    .notice {color: red; font-size:3.0em; text-align:center; transform: scaleY(.85);
    font-weight: bold;}
    table, th, td { border: 1px solid #888; }
    th, td { padding: 15px; text-align: left;}
</style>

<center>
(DRAFT) CBP Test Plan 2
</center>

<div style="font-weight: bold;">
  <p style="text-align: center;">
    SYSTEM INFORMATION
  </p>
</div>

<div>
  <p>{{project.system_info.system_short_name}} is a {% filter lower %}{{project.cbp_system_info.system_type.text}}{% endfilter %} hosted in the {{project.system_info.system_hosting.text}} environment.
  </p>
  <p>
    {{project.system_info.system_description}}
  </p>
</div>


<div>
  <h3>Test Plan Introduction</h3>{{project.se_cace_elk}}{% if project.se_cace_elk %}

  {% for od in project.se_cace_elk.output_documents %}
    <div style="margin: 12px 0 0 0;">
        {{project.se_cace_elk.output_documents[od]}}
    </div>
    <small style="color: #aaa;">{{od}}</small>
  {% endfor %}
  {% endif %}
</div>

