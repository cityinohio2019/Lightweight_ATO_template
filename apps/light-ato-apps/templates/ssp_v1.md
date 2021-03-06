id: ssp_v1
format: markdown
title: SSP v1
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

<!-- Cover page -->
<center>

<center>
<img style="max-width:70%;height:auto;" src="{{static_asset_path_for('app.png')}}">
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

<div class="table-caption">Table 1-1. Information System Name and Title</div>

<!-- Information System Table goes -->
<table class="table-ssp" border="1">
    <tr>
      <th class="th-header">Unique Identifier</th>
      <th class="th-header">Information System Name</th>
      <th class="th-header">Information System Abbreviation</th>
    </tr>
    <tr>
      <td>{{project.fisma_level.application_number}}</td>
      <td>{{project.system_info.system_name}}</td>
      <td>{{project.system_info.system_short_name}}</td>
    </tr>
</table>


<h2>2.  INFORMATION SYSTEM CATEGORIZATION</h2>

The overall information system sensitivity categorization is recorded in Table 2 1. Security Categorization that follows.  Directions for attaching the FIPS 199 document may be found in the following section: Attachment 10, FIPS 199.

<div class="table-caption">Table 2-1. Security Categorization</div>

<!-- security categorization table goes here -->
<table class="table-ssp" border="1">
    <tr>
      <th class="th-header">System Sensitivity Level</th>
      <td>{{project.fisma_level.fisma_level}}</td>
    </tr>
</table>

<h3>2.1 Information Types</h3>

This section describes how the information types used by the information system are categorized for confidentiality, integrity and availability sensitivity levels.

The following tables identify the information types that are input, stored, processed and/or output from Enter Information System Abbreviation.  The selection of the information types is based on guidance provided by Office of Management and Budget (OMB) Federal Enterprise Architecture Program Management Office Business Reference Model 2.0 and FIPS Pub 199, Standards for Security Categorization of Federal Information and Information Systems which is based on NIST Special Publication (SP) 800-60, Guide for Mapping Types of Information and Information Systems to Security Categories. 

The tables also identify the security impact levels for confidentiality, integrity and availability for each of the information types expressed as low, moderate, or high.  The security impact levels are based on the potential impact definitions for each of the security objectives (i.e., confidentiality, integrity and availability) discussed in NIST SP 800-60 and FIPS Pub 199. 
The potential impact is low if—

* The loss of confidentiality, integrity, or availability could be expected to have a limited adverse effect on organizational operations, organizational assets, or individuals.
* A limited adverse effect means that, for example, the loss of confidentiality, integrity, or availability might: (i) cause a degradation in mission capability to an extent and duration that the organization is able to perform its primary functions, but the effectiveness of the functions is noticeably reduced; (ii) result in minor damage to organizational assets; (iii) result in minor financial loss; or (iv) result in minor harm to individuals.

The potential impact is moderate if—

* The loss of confidentiality, integrity, or availability could be expected to have a serious adverse effect on organizational operations, organizational assets, or individuals. 
* A serious adverse effect means that, for example, the loss of confidentiality, integrity, or availability might: (i) cause a significant degradation in mission capability to an extent and duration that the organization is able to perform its primary functions, but the effectiveness of the functions is significantly reduced; (ii) result in significant damage to organizational assets; (iii) result in significant financial loss; or (iv) result in significant harm to individuals that does not involve loss of life or serious life threatening injuries.

The potential impact is high if—

* The loss of confidentiality, integrity, or availability could be expected to have a severe or catastrophic adverse effect on organizational operations, organizational assets, or individuals. 
* A severe or catastrophic adverse effect means that, for example, the loss of confidentiality, integrity, or availability might: (i) cause a severe degradation in or loss of mission capability to an extent and duration that the organization is not able to perform one or more of its primary functions; (ii) result in major damage to organizational assets; (iii) result in major financial loss; or (iv) result in severe or catastrophic harm to individuals involving loss of life or serious life threatening injuries. 

<div class="table-caption">Table 2-2. Sensitivity Categorization of Information Types</div>
<!-- Sensitivity Categorization of Information Types Table goes -->
{{project.technical_information.info_type_table_01}}

<h2>2.2 Security Objectives Categorization</h2>
Based on the information provided in Table 2 2. Sensitivity Categorization of Information Types, for the Enter Information System Abbreviation, default to the high-water mark for the Information Types as identified in Table 2 3. Security Impact Level below. 

<div class="table-caption">Table 2-3. Security Impact Level</div>

{{project.technical_information.security_impact_level}}

Through review and analysis, it has been determined that the baseline security categorization for the Enter Information System Abbreviation system is listed in the Table 2 4. Baseline Security Configuration that follows.

<div class="table-caption">Table 2-4. Baseline Security Configuration</div>

<!-- Security Impact Level Table goes here -->
<table class="table-ssp" border="1">
    <tr>
      <td class="td-row-title">Information System Abbreviation Security Categorization</td>
      <td>[[LOW_MODERATE_HIGH]]</td>
    </tr>
</table>

Using this categorization, in conjunction with the risk assessment and any unique security requirements, we have established the security controls for this system, as detailed in this SSP.


<h2>3.  INFORMATION SYSTEM OWNER</h2>

The following individual is identified as the system owner or functional proponent/advocate for this system.  

<div class="table-caption">Table 3-1. Information System Owner</div>

<table class="table-ssp" border="1">
    <tr>
      <th class="th-header" colspan="2">Information System Owner Information</th>
    </tr>
    <tr>
      <td class="td-row-title">Name</td>
      <td>{{project.system_info.system_owner}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Title</td>
      <td>{{project.system_info_poc.system_owner_title}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Company / Organization</td>
      <td>{{project.system_info.system_org}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Phone Number</td>
      <td>{{project.system_info_poc.system_owner_phone}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Email Address</td>
      <td>{{project.system_info_poc.system_owner_email}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Address</td>
      <td>{{project.system_info_poc.system_owner_address}}</td>
    </tr>
</table>

<h2>4.  AUTHORIZING OFFICIAL</h2>

The Authorizing Official (AO) or Designated Approving Authority (DAA) for this information system is:

<div class="table-caption">Table 4-1. Information System Authorizing Official</div>

<table class="table-ssp" border="1">
    <tr>
      <th class="th-header" colspan="2">Information System Authorizing Official</th>
    </tr>
    <tr>
      <td class="td-row-title">Name</td>
      <td>{{project.system_info_poc.system_ao_name}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Title</td>
      <td>{{project.system_info_poc.system_ao_title}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Company / Organization</td>
      <td>{{project.system_info_poc.system_ao_org}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Phone Number</td>
      <td>{{project.system_info_poc.system_ao_phone}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Email Address</td>
      <td>{{project.system_info_poc.system_ao_email}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Address</td>
      <td>{{project.system_info_poc.system_ao_address}}</td>
    </tr>
</table>

<h2>5.  OTHER DESIGNATED CONTACTS</h2>

<div class="table-caption">Table 5-1. Information System Management Point of Contact</div>

<table class="table-ssp" border="1">
    <tr>
      <th class="th-header" colspan="2">Information System Management Point of Contact</th>
    </tr>
    <tr>
      <td class="td-row-title">Name</td>
      <td>{{project.system_info.system_pm}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Title</td>
      <td>{{project.system_info_poc.system_manager_title}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Company / Organization</td>
      <td>{{project.system_info.system_org}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Phone Number</td>
      <td>{{project.system_info_poc.system_manager_phone}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Email Address</td>
      <td>{{project.system_info_poc.system_manager_email}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Address</td>
      <td>{{project.system_info_poc.system_manager_address}}</td>
    </tr>
</table>

<div class="table-caption">Table 5-2. Information System Technical Point of Contact</div>

<table class="table-ssp" border="1">
    <tr>
      <th class="th-header" colspan="2">Information System Technical Point of Contact</th>
    </tr>
    <tr>
      <td class="td-row-title">Name</td>
      <td>{{project.system_info_poc.system_tech_name}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Title</td>
      <td>{{project.system_info_poc.system_tech_title}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Company / Organization</td>
      <td>{{project.system_info.system_admin_team}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Phone Number</td>
      <td>{{project.system_info_poc.system_tech_phone}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Email Address</td>
      <td>{{project.system_info_poc.system_tech_email}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Address</td>
      <td>{{project.system_info_poc.system_tech_address}}</td>
    </tr>
</table>

<h2>6.  ASSIGNMENT OF SECURITY RESPONSIBILITY</h2>

<div class="table-caption">Table 6-1. CSP name Internal ISSO (or Equivalent) Point of Contact</div>

<table class="table-ssp" border="1">
    <tr>
      <th class="th-header" colspan="2">CSP name Internal ISSO (or Equivalent) Point of Contact</th>
    </tr>
    <tr>
      <td class="td-row-title">Name</td>
      <td>{{project.system_info_poc.system_security_name}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Title</td>
      <td>{{project.system_info_poc.system_security_title}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Company / Organization</td>
      <td>{{project.system_info_poc.system_security_org}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Phone Number</td>
      <td>{{project.system_info_poc.system_security_phone}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Email Address</td>
      <td>{{project.system_info_poc.system_security_email}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Address</td>
      <td>{{project.system_info_poc.system_security_address}}</td>
    </tr>
</table>


<div class="table-caption">Table 6-2. AO Point of Contact</div>

<table class="table-ssp" border="1">
    <tr>
      <th class="th-header" colspan="2">AO Point of Contact</th>
    </tr>
    <tr>
      <td class="td-row-title">Name</td>
      <td>{{project.system_info_poc.system_ao_poc_name}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Title</td>
      <td>{{project.system_info_poc.system_ao_poc_title}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Company / Organization</td>
      <td>{{project.system_info_poc.system_ao_poc_org}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Phone Number</td>
      <td>{{project.system_info_poc.system_ao_poc_phone}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Email Address</td>
      <td>{{project.system_info_poc.system_ao_poc_email}}</td>
    </tr>
    <tr>
      <td class="td-row-title">Address</td>
      <td>{{project.system_info_poc.system_ao_poc_address}}</td>
    </tr>
</table>

<h2>7.  INFORMATION SYSTEM OPERATIONAL STATUS</h2>

The system is currently in the life-cycle phase shown in Table 7 1. System Status that follows.  (Only operational systems can be granted an ATO).

<div class="table-caption">Table 7-1. System Status</div>

<table class="table-ssp" border="1">
    <tr>
      <th class="th-header" colspan="3">System Status</th>
    </tr>
    <tr>
      <td>{% if project.system_info_technical.system_status == "operational" %}Operational (System is operating and in production) {% endif %} {% if project.system_info_technical.system_status == "under_dev" %} Under Development (System is being designed, developed, or implemented) {% endif %} {% if project.system_info_technical.system_status == "major_mod" %} Major Modification (System is undergoing a major change, development, or transition){% endif %} {% if project.system_info_technical.system_status == "other" %} Other ({{project.system_info_technical.choice_other}}){% endif %} </td>
    </tr>
    <tr>
</table>

<h2>8.  INFORMATION SYSTEM TYPE</h2>

Information systems, particularly those based on cloud architecture models, are made up of different service layers.  Below are some questions that help the system owner determine if their system is a cloud followed by specific questions to help the system owner determine the type of cloud.

<div class="table-caption">Table 8-1. Service Layers Represented in this SSP</div>

<table class="table-ssp" border="1">
    <tr>
      <th class="th-header" colspan="3">System Status</th>
    </tr>
    <tr>
      <td>{{project.system_info_technical.cloud_service_model.text}}
      {% if project.system_info_technical.cloud_service_model == "other" %}
    {{project.system_info_technical.cloud_service_model_other.text}}{% endif %} </td>
    </tr>
    <tr>
</table>

Note: Refer to NIST SP 800-145 for information on cloud computing architecture models.  

<h3>8.2.  Cloud Deployment Models</h3>

Information systems are made up of different deployment models.  The deployment models of the Enter Information System Abbreviation that are defined in this SSP and are not leveraged by any other FedRAMP Authorizations, are indicated in Table 8 2. Cloud Deployment Model Represented in this SSP that follows.

<div class="table-caption">Table 8-2. Cloud Deployment Model Represented in this SSP</div>

<table class="table-ssp" border="1">
    <tr>
      <th class="th-header" colspan="3">System Status</th>
    </tr>
    <tr>
      <td>{{project.system_info_technical.cloud_model.text}}
      {% if project.system_info_technical.cloud_model == "hybrid" %} {{project.system_info_technical.choice_hybrid.text}}{% endif %} </td>
    </tr>
    <tr>
</table>

<h3>8.3. Leveraged Authorizations</h3>

The {{project.system_info.system_name}} Choose an item leverages a pre-existing FedRAMP Authorization.  FedRAMP Authorizations leveraged by this Enter Information System Abbreviation are listed in Table 8 3. Leveraged Authorizations that follows.

<div class="table-caption">Table 8-3. Leveraged Authorizations</div>

{{project.system_info_technical.leveraged_authorizations}}

<h2>9.  GENERAL SYSTEM DESCRIPTION</h2>

<h3>9.1.  System Function or Purpose</h3>

{{project.system_info.system_description}}

<h3>9.2.  Information System Components and Boundaries</h3>

[[TBD]]

A detailed and explicit definition of the system authorization boundary diagram is represented in Figure 9-1. Authorization Boundary Diagram below.


<h3>9.3.  Types of Users</h3>

All personnel have their status categorized with a sensitivity level in accordance with PS-2.  Personnel (employees or contractors) of service providers are considered Internal Users.  All other users are considered External Users.  User privileges (authorization permission after authentication takes place) are described in Table 9 1. Personnel Roles and Privileges that follows.

<div class="table-caption">Table 9-1. Personnel Roles and Privileges</div>

{{project.system_info_technical.security_impact_users}}

<h3>9.4.  Network Architecture</h3>

The logical network topology is shown in Figure 9 2. Network Diagram mapping the data flow between components. 
The following Figure 9 2. Network Diagram(s) provides a visual depiction of the system network components that constitute Enter Information System Abbreviation.

<h2>10. SYSTEM ENVIRONMENT AND INVENTORY</h2>
Directions for attaching the FedRAMP Inventory Workbook may be found in the following section: Attachment 13, FedRAMP Inventory Workbook.

<h3>10.1. Data Flow</h3>
The data flow in and out of the system boundaries is represented in Figure 10 1. Data Flow Diagram below.

<h3>10.2. Ports, Protocols and Services</h3>

The Table 10 1. Ports, Protocols and Services below lists the ports, protocols and services enabled in this information system.  

<div class="table-caption">Table 10-1. Ports, Protocols and Services</div>

{{project.system_info_technical.ports_protocols_services}}

<h3>11. SYSTEM INTERCONNECTIONS</h3>

<div class="table-caption">Table 11-1. System Interconnections</div>

{{project.system_info_technical.system_interconnections}}


<h2>12. LAWS, REGULATIONS, STANDARDS AND GUIDANCE</h2>
A summary of FedRAMP Laws and Regulations is included in Attachment 12, FedRAMP Laws and Regulations.

<h3>12.1. Applicable Laws and Regulations</h3>
The FedRAMP Laws and Regulations can be found on this web page: Templates.
Table 12 1. Information System Name Laws and Regulations includes additional laws and regulations specific to Information System Name.

<div class="table-caption">Table 12-1. Information System Name Laws and Regulations</div>

{{project.system_info_technical.laws_regulations}}

<h3>12.2. Applicable Standards and Guidance</h3>
The FedRAMP Standards and Guidance be found on this web page: Templates
Table 12 2. Information System Name Standards and Guidance includes in this section any additional standards and guidance specific to Information System Name.

<div class="table-caption">Table 12-2. Information System Name Standards and Guidance</div>

{{project.system_info_technical.standards_guidance}}



<!-- Testing links -->
<a id="controls" name="controls"></a>
<h2>13. MINIMUM SECURITY CONTROLS</h2>

Security controls must meet minimum security control baseline requirements.  Upon categorizing a system as Low, Moderate, or High sensitivity in accordance with FIPS 199, the corresponding security control baseline standards apply.  Some of the control baselines have enhanced controls which are indicated in parentheses.  

Security controls that are representative of the sensitivity of Enter Information System Abbreviation are described in the sections that follow.  Security controls that are designated as “Not Selected” or “Withdrawn by NIST” are not described unless they have additional FedRAMP controls.  Guidance on how to describe the implemented standard can be found in NIST 800-53, Rev 4.  Control enhancements are marked in parentheses in the sensitivity columns.  

Systems that are categorized as FIPS 199 Low use the controls designated as Low, systems categorized as FIPS 199 Moderate use the controls designated as Moderate and systems categorized as FIPS 199 High use the controls designated as High.  

{% set meta = {"current_family": "", "current_control": "", "current_control_part": ""} %}
{% for ctl in ["AC_11_a_1", "AC_11_a_2", "AC_23_1", "AC_23_2", "AC_23_3", "AC_2_a_1", "AC_2_a_2", "AC_2_b", "AC_2_c", "AC_2_d_1", "AC_2_d_2", "AC_2_d_3", "AC_2_d_4", "AC_2_e_1", "AC_2_e_2", "AC_2_f_1_a", "AC_2_f_1_b", "AC_2_f_1_c", "AC_2_f_1_d", "AC_2_f_1_e", "AC_2_f_2_a", "AC_2_f_2_b", "AC_2_f_2_c", "AC_2_f_2_d", "AC_2_f_2_e", "AC_2_g", "AC_2_h_1", "AC_2_h_2", "AC_2_h_3", "AC_2_i_1", "AC_2_i_2", "AC_2_i_3", "AC_2_j_1", "AC_2_j_2", "AC_2_k", "AC_3", "AC_3_my_org_1", "AC_4_1", "AC_4_2", "AC_4_21_1", "AC_4_21_2", "AC_4_21_3", "AC_6", "ac_6_9", "ac_6_9_test", "AU_12_a_1", "au_12_a_2", "au_12_a_2_test", "AU_12_b_1", "au_12_b_2", "au_12_b_2_test", "au_12_c", "au_12_c_test", "au_12_my_org_1", "au_12_my_org_2", "AU_2_a_1", "au_2_a_2", "au_2_a_2_test", "AU_2_b", "AU_2_c", "AU_2_d_1", "AU_2_d_2", "AU_2_d_3", "AU_6_a_1", "AU_6_a_2", "AU_6_a_3", "AU_6_b_1", "AU_6_b_2", "AU_6_my_org_1", "AU_6_my_org_2", "AU_6_my_org_3", "CA_3_a", "CA_3_b_1", "CA_3_b_2", "CA_3_b_3", "CA_3_c_1", "CA_3_c_2", "CA_5_a_1", "CA_5_a_2", "CA_5_b_1", "CA_5_b_2_a", "CA_5_b_2_b", "CA_5_b_2_c", "CA_5_my_org_1", "CA_7_a_1", "CA_7_a_2", "CA_7_a_3", "CA_7_b_1", "CA_7_b_2", "CA_7_b_3", "CA_7_b_4", "CA_7_c_1", "CA_7_c_2", "CA_7_d_1", "CA_7_d_2", "CA_7_e_1", "CA_7_e_2", "CA_7_f_1", "CA_7_f_2", "CA_7_g_1", "CA_7_g_2", "CA_7_g_3", "CA_7_g_4", "CA_8_1", "CA_8_2", "CA_8_3", "CM_2_1", "CM_2_2", "CM_2_my_org_1", "CM_6_1_1_a", "CM_6_1_1_b", "CM_6_1_1_c", "CM_6_1_2_a", "CM_6_1_2_b", "CM_6_1_2_c", "CM_6_a_1", "CM_6_a_2", "CM_6_a_3", "CM_6_b", "CM_6_c_1", "CM_6_c_1_b", "CM_6_c_1_c", "CM_6_c_2_a", "CM_6_c_2_b", "CM_6_c_2_c", "CM_6_c_3", "CM_6_c_4", "CM_6_c_5", "CM_6_d_1", "CM_6_d_2", "CM_6my_org_1", "CM_6_my_org_2", "CM_6_my_org_3", "CM_6_my_org_4", "CM_6_my_org_5", "CM_6_my_org_6", "CM_6_my_org_7", "CM_6_my_org_8", "CM_7_a", "CM_7_b_1_a", "CM_7_b_1_b", "CM_7_b_1_c", "CM_7_b_1_d", "CM_7_b_2_a", "CM_7_b_2_b", "CM_7_b_2_c", "CM_7_b_2_d", "CM_8_a_1", "CM_8_a_2", "CM_8_a_3", "CM_8_a_4_1", "CM_8_a_4_2", "CM_8_b_1", "CM_8_b_2", "CM_8_my_org_1", "CM_8_my_org_2", "CP_2_a_1", "CP_2_a_2_1", "CP_2_a_2_2", "CP_2_a_2_3", "CP_2_a_3_1", "CP_2_a_3_2", "CP_2_a_3_3", "CP_2_a_4", "CP_2_a_5", "CP_2_a_6_1", "CP_2_a_6_2", "CP_2_b_1", "CP_2_b_2", "CP_2_c", "CP_2_d_1", "CP_2_d_2", "CP_2_e_1", "CP_2_e_2", "CP_2_f_1", "CP_2_f_2", "CP_4_a_1", "CP_4_a_2", "CP_4_a_3", "CP_4_b", "CP_4_C", "CP_4_my_org_1", "IA_2", "IA_2_1", "IA_2_12_1", "IA_2_12_2", "IA_2_2", "IA_2_8", "IA_2_9", "IA_2_my_org_1", "IA_2_my_org_2", "IR_4_a_1", "IR_4_a_2", "IR_4_a_3", "IR_4_a_4", "IR_4_a_5", "IR_4_b", "IR_4_c_1_a", "IR_4_c_1_b", "IR_4_c_1_c", "IR_4_c_2_a", "IR_4_c_2_b", "IR_4_c_2_c", "IR_5_1", "IR_5_2", "IR_6_a_1", "IR_6_a_2", "IR_6_b_1", "IR_6_b_2", "MP_4", "MP_4_a_1", "MP_4_a_2", "MP_4_a_3", "MP_4_a_4", "MP_4_b", "PL_2_a_1", "PL_2_a_2", "PL_2_a_3", "PL_2_a_4", "PL_2_a_5", "PL_2_a_6", "PL_2_a_7", "PL_2_a_8", "PL_2_a_9", "PL_2_b_1", "PL_2_b_2", "PL_2_c_1", "PL_2_c_2", "PL_2_d_1", "PL_2_d_2", "PL_2_d_3", "PL_2_e_1", "PL_2_e_2", "PL_8_a_1", "PL_8_a_2", "PL_8_a_3", "PL_8_b_1", "PL_8_b_2", "PL_8_c_1", "PL_8_c_2", "PL_8_c_3", "RA_2_a", "RA_2_b", "RA_2_c", "RA_3_a_1", "RA_3_a_2", "RA_3_b_1", "RA_3_b_2_a", "RA_3_b_2_b", "RA_3_b_2_c", "RA_3_c_1", "RA_3_c_2", "RA_3_d_1", "RA_3_d_2", "RA_3_e_1", "RA_3_e_2_a", "RA_3_e_2_b", "RA_3_e_2_c", "RA_5_a_1_a", "RA_5_a_1_b", "RA_5_a_2_a", "RA_5_a_2_b", "RA_5_a_3_a", "RA_5_a_3_b", "RA_5_b_1_1", "RA_5_b_1_2", "RA_5_b_1_3", "RA_5_b_2_1", "RA_5_b_2_2", "RA_5_b_3", "RA_5_c_1", "RA_5_c_2", "RA_5_d_1", "RA_5_d_2", "RA_5_e_1", "RA_5_e_2", "RA_5_e_3", "SA_11_1", "SA_22_a", "SA_22_b_1", "SA_22_b_2", "SA_9_a_1", "SA_9_a_2", "SA_9_a_3", "SA_9_b_1", "SA_9_b_2", "SA_9_c_1", "SA_9_c_2", "SC_12_1_a", "SC_12_1_b", "SC_12_1_c", "SC_12_1_d", "SC_12_1_e", "SC_12_2", "SC_12_my_org_1", "SC_12_my_org_2", "SC_12_my_org_3", "SC_12_my_org_4", "SC_12_my_org_5", "SC_13_1", "SC_13_2", "SC_13_3", "SC_13_my_org_1", "SC_13_my_org_2", "SC_13_my_org_3", "SC_13_my_org_4", "SC_13_my_org_5", "SC_18_a", "SC_18_b_1", "SC_18_b_2", "SC_18_c_1", "SC_18_c_2", "SC_18_c_3", "SC_23", "SC_23_3_1", "SC_23_3_2", "SC_23_3_3", "SC_24_1", "SC_24_2", "SC_24_3", "SC_24_4", "SC_24_5", "SC_28_1_1", "SC_28_1_2", "SC_28_1_3", "SC_7_a_1", "SC_7_a_2", "SC_7_a_3", "SC_7_a_4", "SC_7_b_1", "SC_7_b_2", "SC_7_C", "SC_8_1", "SC_8_2", "SI_10_1", "SI_10_2", "SI_13_a_1", "SI_13_a_2", "SI_13_b_1", "SI_13_b_2", "SI_13_b_3", "SI_2_3_a", "SI_2_3_b_1", "SI_2_3_b_2", "SI_2_a_1", "SI_2_a_2", "SI_2_a_3", "SI_2_b_1", "SI_2_b_2", "SI_2_c_1", "SI_2_c_2", "SI_2_c_3", "SI_2_c_4", "SI_2_d", "SI_4_a_1_1", "SI_4_a_1_2_a", "SI_4_a_1_2_b", "SI_4_a_2_1", "SI_4_a_2_2", "SI_4_a_2_3", "SI_4_b_1", "SI_4_b_2", "SI_4_c_1", "SI_4_c_2", "SI_4_d_1", "SI_4_d_2", "SI_4_d_3", "SI_4_e", "SI_4_f", "SI_4_g_1", "SI_4_g_2", "SI_4_g_3", "SI_4_g_4_a", "SI_4_g_4_b"]
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
      <h4 style="">{{meta["current_control"]|upper}}</h4>
        <p>CONTROL DESCRIPTION HERE</p>
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
      {% for se in ["se_aws_auditing_splunk_elk", "se_aws_ci_cd_jenkins_gitlab_aqua_sonarqube", "se_ciso_policy_soc_stp", "se_system_level"] %}
        {% if project[se] %}
          {% for od in project[se].output_documents if not "test" in od %}
            {% if ctl_od_title == od %}
              {% set odl = od.split('_') %}
              {% set c_name_part = "{}-{}".format(odl[3].upper(), " ".join(odl[4:])) %}
             <div class="soft" style="font-style: italic;">{{project[se]}}</div>
              <quote>
                {{project[se].output_documents[od]}}
              </quote>
            {% endif %}
          {% endfor %}<!-- /for od in -->
        {% else %}
          <div style="color:#aaa;">&nbsp;{{se}} not completed</div>
        {% endif %}
      {% endfor %}<!-- /for se in -->
      </td>
  </tr>
  {% if not loop.last %}
    {% if loop.nextitem.split("_")[0].upper() != meta["current_family"].upper() %}
      </table>
    {% endif %}
  {% endif %}
{% endfor %}<!-- /for ctl in -->
<!-- /Testing Links -->


