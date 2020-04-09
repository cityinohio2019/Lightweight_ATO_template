id: risk_assessment_report.md
format: markdown
title: Risk Assessment Report
...

<style type="text/css" scoped>
    h2 { border-bottom:1px solid #888; margin-top: 3em; color: red;}
    h3 { border-bottom: 0.5px solid #aaa; color: #777; font-size: 14pt; font-weight: bold;}
    h4 { margin-top: 15px; font-weight: bold; font-size: 1em; }
    blockquote { color: #666; font-size:0.8em; margin: 0 10px; }
    .notice {color: red; font-size:3.0em; text-align:center; transform: scaleY(.85);
    font-weight: bold;}
    table { border: none; border-collapse: collapse; }
    th, td { border: 1px solid #888; padding: 15px; text-align: left;}
    @media all {
        .page-break     { display: none; }
    }
    .table-caption {
      color: red;
      text-align: center;
      font-style: italic;
      margin: 1em; 0 0.33em; 0;
    }
    table.table-ssp {
      margin-bottom: 1.0em;
      width: 100%;
    }
    table.table-ssp th, table.table-ssp td {
      padding: 4px;
    }
    td.td-header, th.th-header {
      color: white;
      background-color: rgb(31, 58, 105);
      text-align:center;
      font-weight: bold;
    }
    td.td-c-name-part, td.td-row-title {
      width: 125px;
      background-color: rgb(219, 228, 244);
      font-weight: bold;
      padding-left: 12px;
    }
    table.table-ssp td {
      padding-left: 12px;
    }
    .soft {
      color: #aaa;
    }
    @media print {
        h1.title {
            /* v-center, need absolute */
            position: absolute; /* repeats once */
            bottom: 50%;
            /* h-center, for element with absolute positioning */
            left: 0;
            right: 0;
            margin-left: 20%;
            margin-right: 20%;
        }
        .footer {
            position: fixed; /* repeats on every page */
            bottom: 0;
        }
        table.footer {
            width: 95%;
            display: table;
        }
        table.footer td {
            border: none;
            padding: 0px;
            padding-bottom: .1em;
        }
        .page-break { display: block; page-break-after: always; }
    }
</style>

<center>
<h1 class="title">{{project.system_info.system_name}}<br/>Risk Assessment Report<br/>for {{project.system_info.system_name}}</h1>
<img style="max-width:70%;height:auto;" src="{{static_asset_path_for('app.png')}}">
<br></br>
<h1>Prepared for</br/>{{project.system_info.system_org}}</h1>
<br></br>
{{project.risk_assessment_report_doc.rar_date}}
</center>




* * *

## Table of Contents

*   [1. RTM](#rtm)
    *   [1.1 Introduction](#introduction)
    *   [1.2 Plan of Action and Milestone Table](#rtmtable)

* * *

## 1. RTM
### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1.1 Introduction


###Section 1: Hardware? (need question module)
###Section 2: Published software? (need question module)
###Section 3: Address for office

###Section 4, This Text:
The Risk Assessment identifies risk to the system operation based on vulnerabilities (those areas that do not meet minimum requirements and for which adequate countermeasures have not been implemented). The RA also determines the likelihood of occurrence and suggests countermeasures to mitigate identified risks in an effort to provide an appropriate level-of-protection and to meet all minimum requirements imposed on the system.   

The system security policy requirements are being met at this time with the exception of those areas identified in this report. The countermeasures recommended in this report specify the additional security controls needed to meet policies and to effectively manage the security risk to the system and its operating environment. Ultimately, the Security Control Assessor and the Authorizing Official must determine whether the totality of the protection mechanisms approximate a sufficient level of security, and are adequate for the protection of this system and its resources/information. The Risk Assessment Results supplied critical information and should be carefully reviewed by the AO prior to making a final security authorization decision. The control categories for both technical and nontechnical control methods can be further classified as either preventive or detective. 
These two subcategories are explained as follows: 
* Preventive controls inhibit attempts to violate security policy and include such controls as access control enforcement, encryption, and authentication.
* Detective controls warn of violations or attempted violations of security policy and include such controls as audit trails, intrusion detection methods, and checksums

###Section 5, Control Analysis Table (populated with Greg code)
Note: Counts the amount of control categories and files them as preventive or defective. And out of those two subcategories, they are matrixed as either being implemented or not implemented.

Text:
Preventive controls provide greater risk mitigation than detective controls. Preventive controls properly implemented and operating as intended provide automatic risk mitigation without the need for additional manual procedures. Detective controls require additional procedures to ensure that risks, incidents, and vulnerabilities they uncover are properly mitigated or remediated.  






GREG CODE BELOW TO SET UP REMAINDER OF DOCUMENT
<br></br>

### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1.2 Requirement Traceability Matrix Table

{% set meta = {"current_family": "", "current_control": "", "current_control_part": ""} %}
{% for ctl in ["AC_11_a_1", "AC_11_a_2", "AC_23_1", "AC_23_2", "AC_23_3", "AC_2_a_1", "AC_2_a_2", "AC_2_b", "AC_2_c", "AC_2_d_1", "AC_2_d_2", "AC_2_d_3", "AC_2_d_4", "AC_2_e_1", "AC_2_e_2", "AC_2_f_1_a", "AC_2_f_1_b", "AC_2_f_1_c", "AC_2_f_1_d", "AC_2_f_1_e", "AC_2_f_2_a", "AC_2_f_2_b", "AC_2_f_2_c", "AC_2_f_2_d", "AC_2_f_2_e", "AC_2_g", "AC_2_h_1", "AC_2_h_2", "AC_2_h_3", "AC_2_i_1", "AC_2_i_2", "AC_2_i_3", "AC_2_j_1", "AC_2_j_2", "AC_2_k", "AC_3", "AC_3_my_org_1", "AC_4_1", "AC_4_2", "AC_4_21_1", "AC_4_21_2", "AC_4_21_3", "AC_6", "ac_6_9", "ac_6_9_test", "AU_12_a_1", "au_12_a_2", "au_12_a_2_test", "AU_12_b_1", "au_12_b_2", "au_12_b_2_test", "au_12_c", "au_12_c_test", "au_12_my_org_1", "au_12_my_org_2", "AU_2_a_1", "au_2_a_2", "au_2_a_2_test", "AU_2_b", "AU_2_c", "AU_2_d_1", "AU_2_d_2", "AU_2_d_3", "AU_6_a_1", "AU_6_a_2", "AU_6_a_3", "AU_6_b_1", "AU_6_b_2", "AU_6_my_org_1", "AU_6_my_org_2", "AU_6_my_org_3", "CA_3_a", "CA_3_b_1", "CA_3_b_2", "CA_3_b_3", "CA_3_c_1", "CA_3_c_2", "CA_5_a_1", "CA_5_a_2", "CA_5_b_1", "CA_5_b_2_a", "CA_5_b_2_b", "CA_5_b_2_c", "CA_5_my_org_1", "CA_7_a_1", "CA_7_a_2"]
   if "test" not in ctl %}
  {# Are we changing families? #}
  {% if ctl.split("_")[0].upper() != meta["current_family"].upper() %}
    {% set var_ignore = meta.update({"current_family": ctl.split("_")[0].upper()}) %}
    <h3 style="margin-bottom: 30px;">{{meta["current_family"]|upper}}</h3>
  {% endif %}
  {% set ctl_od_title = "nist_80053rev4_ssp_{}".format(ctl) %}
  {% set odl = ctl_od_title.split('_') %}
  {% set c_name = "{}-{}".format(odl[3].upper(), "".join(odl[4])) %}
  {# Are we changing control name? #}
  {% if c_name.upper() != meta["current_control"].upper() %}
    {# Close previous control table if this is not first time through loop #}
    {% if not loop.first %}
      </table>
    {% endif %}
    {% set var_ignore = meta.update({"current_control": c_name}) %}
      <h4 style="">{{meta["current_control"]|upper}} {{control_catalog[meta["current_control"]|upper]['title']}}</h4>
      <table class="table-ssp">
        <tr>
          <td colspan="2" class="td-header">
          {{meta["current_control"]|upper}}: What is the solution and how is it implemented?
        </td></tr>
  {% endif %}
  {% set c_name_part = "{}-{}".format(odl[3].upper(), " ".join(odl[4:])) %}
  <tr>
    <td class="td-c-name-part">{{c_name_part}}</td>
    <td>
      {{control_catalog[meta["current_control"]|upper]['title']}}
    </td>
  </tr>
  {% if not loop.last %}
    {% if loop.nextitem.split("_")[0].upper() != meta["current_family"].upper() %}
      </table>
    {% endif %}
  {% endif %}
{% endfor %}<!-- /for ctl in -->






