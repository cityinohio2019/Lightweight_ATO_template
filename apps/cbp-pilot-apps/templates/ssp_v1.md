id: ssp_v1
format: markdown
title: SSP v1
...
<style type="text/css" scoped>
    h2 { border-bottom:1px solid #888; }
    h3 { border-bottom: 0.5px solid #aaa; }
    h4 { margin-top: 15px; font-weight: bold; font-size: 1em; }
    blockquote { color: #666; font-size:0.8em; margin: 0 10px; }
    .notice {color: red; font-size:3.0em; text-align:center; transform: scaleY(.85);
    font-weight: bold;}
    table { border: none; border-collapse: collapse; }
    th, td { border: 1px solid #888; padding: 15px; text-align: left;}
    @media all {
        .page-break     { display: none; }
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

<!-- Cover page -->
<center>

<center>
<img style="max-width:70%;height:auto;" src="{{static_asset_path_for('U.S.-Customs-and-Border-Protection-CBP.png')}}">
<h1 class="title">{{project.system_info.system_name}}<br/>System Security Plan</h1>
</center>

<div class="page-break">
  <table class="footer">
    <tr>
      <td width="33%"><strong>{{project.system_info.system_short_name}}</strong></td>
      <td width="34%" style="text-align: center;"><strong>LIMITED OFFICIAL USE</strong></td>
      <td width="33%" style="text-align: right;"> <!-- page number --></td>
    </tr><tr>
      <td colspan="3">Security Test Plan</td>
    </tr>
  </table>
</div>

FOR OFFICIAL USE ONLY

DEPARTMENT OF HOMELAND SECURITY


{{project.system_profile.system_basics.system_name}}
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

<h2>1.  INFORMATION SYSTEM NAME/TITLE</h2>

This System Security Plan provides an overview of the security requirements for the Information System Name (Enter Information System Abbreviation) and describes the controls in place or planned for implementation to provide a level of security appropriate for the information to be transmitted, processed or stored by the system.  Information security is vital to our critical infrastructure and its effective performance and protection is a key component of our national security program.  Proper management of information technology systems is essential to ensure the confidentiality, integrity and availability of the data transmitted, processed or stored by the Enter Information System Abbreviation information system.

The security safeguards implemented for the Enter Information System Abbreviation system meet the policy and control requirements set forth in this System Security Plan.  All systems are subject to monitoring consistent with applicable laws, regulations, agency policies, procedures and practices.

<div style="text-align:center;">Table 1-1. Information System Name and Title</div>

<!-- Information System Table goes -->
<table border = "1">
    <tr>
      <td><strong>Unique Identifier</strong></td>
      <td><strong>Information System Name</strong></td>
      <td><strong>Information System Abbreviation</strong></td>
    </tr>
    <tr>
      <td>[[FedRAMP_Application_Number]]</td>
      <td>{{project.system_info.system_name}}</td>
      <td>{{project.system_info.system_short_name</td>
    </tr>
</table>


<h2>2.  INFORMATION SYSTEM CATEGORIZATION</h2>

The overall information system sensitivity categorization is recorded in Table 2 1. Security Categorization that follows.  Directions for attaching the FIPS 199 document may be found in the following section: Attachment 10, FIPS 199.

<div style="text-align:center;">Table 2-1. Security Categorization</div>

<!-- security categorization table goes here -->
<table border = "1">
    <tr>
      <td><strong>System Sensitivity Level</strong></td>
      <td>[[Security_Categorization_Level]]</td>
    </tr>
</table>

<h3>2.1 Information Types</h3>

This section describes how the information types used by the information system are categorized for confidentiality, integrity and availability sensitivity levels.

The following tables identify the information types that are input, stored, processed and/or output from Enter Information System Abbreviation.  The selection of the information types is based on guidance provided by Office of Management and Budget (OMB) Federal Enterprise Architecture Program Management Office Business Reference Model 2.0 and FIPS Pub 199, Standards for Security Categorization of Federal Information and Information Systems which is based on NIST Special Publication (SP) 800-60, Guide for Mapping Types of Information and Information Systems to Security Categories.  

The tables also identify the security impact levels for confidentiality, integrity and availability for each of the information types expressed as low, moderate, or high.  The security impact levels are based on the potential impact definitions for each of the security objectives (i.e., confidentiality, integrity and availability) discussed in NIST SP 800-60 and FIPS Pub 199.  
The potential impact is low if— 

• The loss of confidentiality, integrity, or availability could be expected to have a limited adverse effect on organizational operations, organizational assets, or individuals.
• A limited adverse effect means that, for example, the loss of confidentiality, integrity, or availability might: (i) cause a degradation in mission capability to an extent and duration that the organization is able to perform its primary functions, but the effectiveness of the functions is noticeably reduced; (ii) result in minor damage to organizational assets; (iii) result in minor financial loss; or (iv) result in minor harm to individuals.

The potential impact is moderate if— 

• The loss of confidentiality, integrity, or availability could be expected to have a serious adverse effect on organizational operations, organizational assets, or individuals.  
• A serious adverse effect means that, for example, the loss of confidentiality, integrity, or availability might: (i) cause a significant degradation in mission capability to an extent and duration that the organization is able to perform its primary functions, but the effectiveness of the functions is significantly reduced; (ii) result in significant damage to organizational assets; (iii) result in significant financial loss; or (iv) result in significant harm to individuals that does not involve loss of life or serious life threatening injuries.

The potential impact is high if— 

• The loss of confidentiality, integrity, or availability could be expected to have a severe or catastrophic adverse effect on organizational operations, organizational assets, or individuals.  
• A severe or catastrophic adverse effect means that, for example, the loss of confidentiality, integrity, or availability might: (i) cause a severe degradation in or loss of mission capability to an extent and duration that the organization is not able to perform one or more of its primary functions; (ii) result in major damage to organizational assets; (iii) result in major financial loss; or (iv) result in severe or catastrophic harm to individuals involving loss of life or serious life threatening injuries.  

<div style="text-align:center;">Table 2-2. Sensitivity Categorization of Information Types</div>

<!-- Sensitivity Categorization of Information Types Table goes -->
<table border = "1">
    <tr>
      <td><strong>Information Type(Use only information types from NIST SP 800-60, Volumes I and II as amended)</strong></td>
      <td><strong>NIST 800-60 identifier for Associated Information Type</strong></td>
      <td><strong>Confidentiality</strong></td>
      <td><strong>Integrity</strong></td>
      <td><strong>Availability</strong></td>
    </tr>
    <tr>
      <td>[[Information_Type]]</td>
      <td>[[NIST_Identifier]]</td>
      <td>[[Confidentiality_Level]]</td>
      <td>[[Integrity_Level]]</td>
      <td>[[Availability_Level]]</td>
    </tr>
    <tr>
      <td>[[Information_Type]]</td>
      <td>[[NIST_Identifier]]</td>
      <td>[[Confidentiality_Level]]</td>
      <td>[[Integrity_Level]]</td>
      <td>[[Availability_Level]]</td>
    </tr>
    <tr>
      <td>[[Information_Type]]</td>
      <td>[[NIST_Identifier]]</td>
      <td>[[Confidentiality_Level]]</td>
      <td>[[Integrity_Level]]</td>
      <td>[[Availability_Level]]</td>
    </tr>
</table>

<h2>2.2 Security Objectives Categorization</h2>
Based on the information provided in Table 2 2. Sensitivity Categorization of Information Types, for the Enter Information System Abbreviation, default to the high-water mark for the Information Types as identified in Table 2 3. Security Impact Level below.  

<div style="text-align:center;">Table 2-3. Security Impact Level</div>

<!-- Security Impact Level Table goes here -->
<table border = "1">
    <tr>
      <td><strong>Security Objective</strong></td>
      <td><strong>Low, Moderate or High</strong></td>
    </tr>
    <tr>
      <td><strong>Confidentiality</strong></td>
      <td>[[LOW_MODERATE_HIGH]]</td>
    </tr>
    <tr>
      <td><strong>Integrity</strong></td>
      <td>[[LOW_MODERATE_HIGH]]</td>
    </tr>
    <tr>
      <td><strong>Availability</strong></td>
      <td>[[LOW_MODERATE_HIGH]]</td>
    </tr>
</table>

Through review and analysis, it has been determined that the baseline security categorization for the Enter Information System Abbreviation system is listed in the Table 2 4. Baseline Security Configuration that follows. 

<div style="text-align:center;">Table 2-4. Baseline Security Configuration</div>

<!-- Security Impact Level Table goes here -->
<table border = "1">
    <tr>
      <td><strong>Information System Abbreviation Security Categorization</strong></td>
      <td>[[LOW_MODERATE_HIGH]]</td>
    </tr>
</table>

Using this categorization, in conjunction with the risk assessment and any unique security requirements, we have established the security controls for this system, as detailed in this SSP.  
  




<!-- Testing links -->
<a id="controls" name="controls"></a>
<h2>2. Security Controls Testing Loops</h2>




{% set meta = {"current_family": ""} %}
{% 
  for ctl in 
  ["AC_11_a_1", "AC_11_a_2", "AC_23_1", "AC_23_2", "AC_23_3", "AC_2_a_1", "AC_2_a_2", "AC_2_b", "AC_2_c", "AC_2_d_1", "AC_2_d_2", "AC_2_d_3", "AC_2_d_4", "AC_2_e_1", "AC_2_e_2", "AC_2_f_1_a", "AC_2_f_1_b", "AC_2_f_1_c", "AC_2_f_1_d", "AC_2_f_1_e", "AC_2_f_2_a", "AC_2_f_2_b", "AC_2_f_2_c", "AC_2_f_2_d", "AC_2_f_2_e", "AC_2_g", "AC_2_h_1", "AC_2_h_2", "AC_2_h_3", "AC_2_i_1", "AC_2_i_2", "AC_2_i_3", "AC_2_j_1", "AC_2_j_2", "AC_2_k", "AC_3", "AC_3_DHS_5_1_1_d", "AC_4_1", "AC_4_2", "AC_4_21_1", "AC_4_21_2", "AC_4_21_3", "AC_6", "ac_6_9", "ac_6_9_test", "AU_12_a_1", "au_12_a_2", "au_12_a_2_test", "AU_12_b_1", "au_12_b_2", "au_12_b_2_test", "au_12_c", "au_12_c_test", "au_12_dhs_5_3_g", "au_12_dhs_5_3_g_test", "AU_2_a_1", "au_2_a_2", "au_2_a_2_test", "AU_2_b", "AU_2_c", "AU_2_d_1", "AU_2_d_2", "AU_2_d_3", "AU_6_a_1", "AU_6_a_2", "AU_6_a_3", "AU_6_b_1", "AU_6_b_2", "AU_6_DHS_5_3_h", "AU_6_DHS_5_3_i", "AU_6_DHS_5_4_6_f", "CA_3_a", "CA_3_b_1", "CA_3_b_2", "CA_3_b_3", "CA_3_c_1", "CA_3_c_2", "CA_5_a_1", "CA_5_a_2", "CA_5_b_1", "CA_5_b_2_a", "CA_5_b_2_b", "CA_5_b_2_c", "CA_5_DHS_2_2_8_d", "CA_7_a_1", "CA_7_a_2", "CA_7_a_3", "CA_7_b_1", "CA_7_b_2", "CA_7_b_3", "CA_7_b_4", "CA_7_c_1", "CA_7_c_2", "CA_7_d_1", "CA_7_d_2", "CA_7_e_1", "CA_7_e_2", "CA_7_f_1", "CA_7_f_2", "CA_7_g_1", "CA_7_g_2", "CA_7_g_3", "CA_7_g_4", "CA_8_1", "CA_8_2", "CA_8_3", "CM_2_1", "CM_2_2", "CM_2_DHS_4_12_b", "CM_6_1_1_a", "CM_6_1_1_b", "CM_6_1_1_c", "CM_6_1_2_a", "CM_6_1_2_b", "CM_6_1_2_c", "CM_6_a_1", "CM_6_a_2", "CM_6_a_3", "CM_6_b", "CM_6_c_1", "CM_6_c_1_b", "CM_6_c_1_c", "CM_6_c_2_a", "CM_6_c_2_b", "CM_6_c_2_c", "CM_6_c_3", "CM_6_c_4", "CM_6_c_5", "CM_6_d_1", "CM_6_d_2", "CM_6_DHS_3_7_e", "CM_6_DHS_3_7_f", "CM_6_DHS_4_12_f", "CM_6_DHS_4_12_j", "CM_6_DHS_4_5_2_b", "CM_6_DHS_4_8_4_a", "CM_6_DHS_5_4_5_d", "CM_6_DHS_5_4_5_e", "CM_7_a", "CM_7_b_1_a", "CM_7_b_1_b", "CM_7_b_1_c", "CM_7_b_1_d", "CM_7_b_2_a", "CM_7_b_2_b", "CM_7_b_2_c", "CM_7_b_2_d", "CM_8_a_1", "CM_8_a_2", "CM_8_a_3", "CM_8_a_4_1", "CM_8_a_4_2", "CM_8_b_1", "CM_8_b_2", "CM_8_DHS_4_12_c", "CM_8_DHS_4_6_a", "CP_2_a_1", "CP_2_a_2_1", "CP_2_a_2_2", "CP_2_a_2_3", "CP_2_a_3_1", "CP_2_a_3_2", "CP_2_a_3_3", "CP_2_a_4", "CP_2_a_5", "CP_2_a_6_1", "CP_2_a_6_2", "CP_2_b_1", "CP_2_b_2", "CP_2_c", "CP_2_d_1", "CP_2_d_2", "CP_2_e_1", "CP_2_e_2", "CP_2_f_1", "CP_2_f_2", "CP_4_a_1", "CP_4_a_2", "CP_4_a_3", "CP_4_b", "CP_4_C", "CP_4_DHS_3_5_2_f", "IA_2", "IA_2_1", "IA_2_12_1", "IA_2_12_2", "IA_2_2", "IA_2_8", "IA_2_9", "IA_2_DHS_5_1_a", "IA_2_DHS_5_1_d", "IR_4_a_1", "IR_4_a_2", "IR_4_a_3", "IR_4_a_4", "IR_4_a_5", "IR_4_b", "IR_4_c_1_a", "IR_4_c_1_b", "IR_4_c_1_c", "IR_4_c_2_a", "IR_4_c_2_b", "IR_4_c_2_c", "IR_5_1", "IR_5_2", "IR_6_a_1", "IR_6_a_2", "IR_6_b_1", "IR_6_b_2", "MP_4", "MP_4_a_1", "MP_4_a_2", "MP_4_a_3", "MP_4_a_4", "MP_4_b", "PL_2_a_1", "PL_2_a_2", "PL_2_a_3", "PL_2_a_4", "PL_2_a_5", "PL_2_a_6", "PL_2_a_7", "PL_2_a_8", "PL_2_a_9", "PL_2_b_1", "PL_2_b_2", "PL_2_c_1", "PL_2_c_2", "PL_2_d_1", "PL_2_d_2", "PL_2_d_3", "PL_2_e_1", "PL_2_e_2", "PL_8_a_1", "PL_8_a_2", "PL_8_a_3", "PL_8_b_1", "PL_8_b_2", "PL_8_c_1", "PL_8_c_2", "PL_8_c_3", "RA_2_a", "RA_2_b", "RA_2_c", "RA_3_a_1", "RA_3_a_2", "RA_3_b_1", "RA_3_b_2_a", "RA_3_b_2_b", "RA_3_b_2_c", "RA_3_c_1", "RA_3_c_2", "RA_3_d_1", "RA_3_d_2", "RA_3_e_1", "RA_3_e_2_a", "RA_3_e_2_b", "RA_3_e_2_c", "RA_5_a_1_a", "RA_5_a_1_b", "RA_5_a_2_a", "RA_5_a_2_b", "RA_5_a_3_a", "RA_5_a_3_b", "RA_5_b_1_1", "RA_5_b_1_2", "RA_5_b_1_3", "RA_5_b_2_1", "RA_5_b_2_2", "RA_5_b_3", "RA_5_c_1", "RA_5_c_2", "RA_5_d_1", "RA_5_d_2", "RA_5_e_1", "RA_5_e_2", "RA_5_e_3", "SA_11_1", "SA_22_a", "SA_22_b_1", "SA_22_b_2", "SA_9_a_1", "SA_9_a_2", "SA_9_a_3", "SA_9_b_1", "SA_9_b_2", "SA_9_c_1", "SA_9_c_2", "SC_12_1_a", "SC_12_1_b", "SC_12_1_c", "SC_12_1_d", "SC_12_1_e", "SC_12_2", "SC_12_DHS_4_6_b", "SC_12_DHS_5_5_3_a", "SC_12_DHS_5_5_3_b", "SC_12_DHS_5_5_3_c", "SC_12_DHS_5_5_3_i", "SC_13_1", "SC_13_2", "SC_13_3", "SC_13_DHS_5_4_6_k", "SC_13_DHS_5_5_1_b", "SC_13_DHS_5_5_1_c", "SC_13_DHS_5_5_2_v", "SC_13_DHS_5_7_d", "SC_18_a", "SC_18_b_1", "SC_18_b_2", "SC_18_c_1", "SC_18_c_2", "SC_18_c_3", "SC_23", "SC_23_3_1", "SC_23_3_2", "SC_23_3_3", "SC_24_1", "SC_24_2", "SC_24_3", "SC_24_4", "SC_24_5", "SC_28_1_1", "SC_28_1_2", "SC_28_1_3", "SC_7_a_1", "SC_7_a_2", "SC_7_a_3", "SC_7_a_4", "SC_7_b_1", "SC_7_b_2", "SC_7_C", "SC_8_1", "SC_8_2", "SI_10_1", "SI_10_2", "SI_13_a_1", "SI_13_a_2", "SI_13_b_1", "SI_13_b_2", "SI_13_b_3", "SI_2_3_a", "SI_2_3_b_1", "SI_2_3_b_2", "SI_2_a_1", "SI_2_a_2", "SI_2_a_3", "SI_2_b_1", "SI_2_b_2", "SI_2_c_1", "SI_2_c_2", "SI_2_c_3", "SI_2_c_4", "SI_2_d", "SI_4_a_1_1", "SI_4_a_1_2_a", "SI_4_a_1_2_b", "SI_4_a_2_1", "SI_4_a_2_2", "SI_4_a_2_3", "SI_4_b_1", "SI_4_b_2", "SI_4_c_1", "SI_4_c_2", "SI_4_d_1", "SI_4_d_2", "SI_4_d_3", "SI_4_e", "SI_4_f", "SI_4_g_1", "SI_4_g_2", "SI_4_g_3", "SI_4_g_4_a", "SI_4_g_4_b"]

%}
  {# Are we changing families? #}
  {% if ctl.split("_")[0].upper() != meta["current_family"].upper() %}
    {% set var_ignore = meta.update({"current_family": ctl.split("_")[0].upper()}) %}
    <h2 style="margin-bottom: 30px;">{{meta["current_family"]|upper}}</h2>
  {% endif %}
  {% set ctl_od_title = "nist_80053rev4_ssp_{}".format(ctl) %}
  {% set odl = ctl_od_title.split('_') %}
  {% set c_name = "{}-{}".format(odl[3].upper(), " ".join(odl[4:])) %}
<div>
  <div style="border-bottom:1px solid #999; font-weight: bold; margin-bottom: 0.5em;">Control {{c_name}} <!-- {{ctl_od_title}} --></div>
  {% for se in ["se_cace_elk", "se_cace_auditing_splunk_elk", "se_cace_ci_cd_jenkins_gitlab_aqua_sonarqube", "se_ciso_policy_soc_stp", "se_sams_system"] %}
    {% if project[se] %}
      {% for od in project[se].output_documents %}
        {% if ctl_od_title == od %}
          {% set odl = od.split('_') %}
          {% set c_name = "{}-{}".format(odl[3].upper(), " ".join(odl[4:])) %}
          <div style="font-style: italic;">{{project[se]}}<span class="soft">&nbsp;&nbsp;&nbsp;&nbsp;{{od}}</span></div>
          <quote>
            {{project[se].output_documents[od]}}
          </quote>
        {% endif %}
      {% endfor %}<!-- /for od in -->
    {% else %}
      <div style="color:#aaa;">&nbsp;{{se}} not completed</div>
    {% endif %}
  {% endfor %}<!-- /for se in -->
</div>
{% endfor %}<!-- /for ctl in -->



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

