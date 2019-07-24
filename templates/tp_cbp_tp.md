id: cbp_tp
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
  <p>{{project.cbp_system_info.system_short_name}} is a {% filter lower %}{{project.cbp_system_info.system_type.text}}{% endfilter %} hosted in the {{project.cbp_system_info.system_hosting.text}} environment.
  </p>
  <p>
    {{project.cbp_system_info.system_description}}
  </p>
</div>


<hr>
<div>
  <h3>Test Plan Introduction</h3>
  {% if project.cbp_test_plan %}
  {% for od in project.cbp_test_plan.output_documents %}
    <div style="margin: 12px 0 0 0;">
        {{project.cbp_test_plan.output_documents[od]}}
    </div>
    <small style="color: #aaa;">{{od}}</small>
  {% endfor %}
  {% endif %}
</div>
<hr>


<!--div>(goal)
  <h3>Audit and Accountability</h3>
  <h4>AC-6 (9)</h4>
  <p>
  {{project.audit_service.output_documents.nist_80053rev4_ssp_ac_6_9}}

  Test: {{project.audit_service.output_documents.nist_80053rev4_ssp_ac_6_9_test}}
  </p>
</div-->



<div>
  <h3>Controls to be tested</h3>
  {% if project.audit_service %}
  {% for od in project.audit_service.output_documents %}
    <div style="margin: 12px 0 0 0;">
        {{project.audit_service.output_documents[od]|striptags}}
    </div>
    <small style="color: #aaa;">{{od}}</small>
  {% endfor %}
  {% endif %}
</div>


<hr style="margin-top: 30px;">
<div>
	<p>Authoring hint</p>
	<ol>
		<li>Look at app.yaml</li>
		<li>Find the module id from which information will appear</li>
		<li>project.app_id.output_documents.ssp_template_control_number
			<br>project.infrastructure.output_documents.ssp_template_au_6|safe
			<br>project.audit_service.output_documents.nist_80053rev4_ssp_ac_6|safe
		</li>
	</ol>
</div>
