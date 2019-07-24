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
CBP Test Plan 2 (Draft GE 10)
</center>


<h2>1 Introduction</h2>

<h3>1.1 Scope</h3>

<h3>1.2 Background</h3>

<div style="font-weight: bold;">
  <p style="text-align: center;">
    SYSTEM INFORMATION
  </p>
</div>

<div>
  <p>{{project.system_info.system_short_name}} is a {% filter lower %}{{project.system_info.system_type.text}}{% endfilter %} hosted in the {{project.system_info.system_hosting.text}} environment.
  </p>
  <p>
    {{project.system_info.system_description}}
  </p>
</div>

<h3>1.3 Project References</h3>

[//]: # (Table 2: Project References. Contains columns for Document Name, Document Version/Date, and Document Location)

<h2>2 Roles and Responsibilities</h2>

[//]: # (Table 3: Organizational Roles and Responsibilities. Contains columns for Name, Team Role, Task, and Length of Project & Percentage of Time Allocated)

<h2> 3 Schedule</h2>

[//]: # (Security Test Schedule. Contains columns for Systems Test Step and Dates for System Testing Steps)

<h2>4 Scope of Testing</h2>

<h3>4.1 Controls to be Tested</h3>

<h3>4.2 Controls Not to be Tested</h3>

<h3>4.3 Assumptions For Test Execution</h3>

<h3>4.4 Test Completion Criteria</h3>

<h2>5 Test Strategy</h2>

<h2>6 Security Test Results</h2>



[//]: # (Table: Type, Name, Version)

<h2>Control Test and Validation</h2>


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

<p>Other testing</p>
