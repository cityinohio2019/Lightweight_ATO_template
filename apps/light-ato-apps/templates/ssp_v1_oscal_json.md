id: ssp_v1_oscal_json
format: oscal_json
title: SSP OSCAL JSON
...
  { "system-security-plan" : 
    { "uuid" : "2fa78e07-74ef-4cd6-8124-bc0050c0c4df",
      "metadata" : 
      { "title" : "FedRAMP System Security Plan (SSP)",
        "published" : "2020-07-01T00:00:00.00-04:00",
        "last-modified" : "2020-07-01T00:00:00.00-04:00",
        "version" : "0.0",
        "oscal-version" : "1.0-Milestone3",
        "revision-history" : 
        [ 
          { "published" : "2019-06-01T00:00:00.00-04:00",
            "version" : "1.0",
            "oscal-version" : "1.0-Milestone3",
            "properties" : 
            [ 
              { "name" : "party-uuid",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "6b286b5d-8f07-4fa7-8847-1dd0d88f73fb" } ],
            "remarks" : "Initial publication." },
          
          { "published" : "2020-06-01T00:00:00.00-04:00",
            "version" : "2.0",
            "oscal-version" : "1.0-Milestone3",
            "properties" : 
            [ 
              { "name" : "party-id",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "csp" } ],
            "remarks" : "Updated for annual assessment." } ],
        "properties" : 
        [ 
          { "name" : "marking",
            "value" : "Controlled Unclassified Information" } ],
        "roles" : 
        [ 
          { "id" : "prepared-by",
            "title" : "Prepared By",
            "desc" : "The organization that prepared this SSP. If developed in-house, this is the CSP itself." },
          
          { "id" : "prepared-for",
            "title" : "Prepared For",
            "desc" : "The organization for which this SSP was prepared. Typically the CSP." },
          
          { "id" : "content-approver",
            "title" : "System Security Plan Approval",
            "desc" : "The individual or individuals accountable for the accuracy of this SSP." },
          
          { "id" : "cloud-service-provider",
            "title" : "Cloud Service Provider",
            "short-name" : "CSP" },
          
          { "id" : "system-owner",
            "title" : "Information System Owner",
            "desc" : "The individual within the CSP who is ultimately accountable for everything related to this system." },
          
          { "id" : "authorizing-official",
            "title" : "Authorizing Official",
            "desc" : "The individual or individuals who must grant this system an authorization to operate." },
          
          { "id" : "authorizing-official-poc",
            "title" : "Authorizing Official's Point of Contact",
            "desc" : "The individual representing the authorizing official." },
          
          { "id" : "system-poc-management",
            "title" : "Information System Management Point of Contact (POC)",
            "desc" : "The highest level manager who responsible for system operation on behalf of the System Owner." },
          
          { "id" : "system-poc-technical",
            "title" : "Information System Technical Point of Contact",
            "desc" : "The individual or individuals leading the technical operation of the system." },
          
          { "id" : "system-poc-other",
            "title" : "General Point of Contact (POC)",
            "desc" : "A general point of contact for the system, designated by the system owner." },
          
          { "id" : "information-system-security-officer",
            "title" : "System Information System Security Officer (or Equivalent)",
            "desc" : "The individual accountable for the security posture of the system on behalf of the system owner." },
          
          { "id" : "privacy-poc",
            "title" : "Privacy Official's Point of Contact",
            "desc" : "The individual responsible for the privacy threshold analysis and if necessary the privacy impact assessment." },
          
          { "id" : "asset-owner",
            "title" : "Owner of an inventory item within the system." },
          
          { "id" : "asset-administrator",
            "title" : "Administrative responsibility an inventory item within the system." },
          
          { "id" : "isa-poc-local",
            "title" : "ICA POC (Local)",
            "desc" : "The point of contact for an interconnection on behalf of this system.",
            "remarks" : "Remove this role if there are no ICAs." },
          
          { "id" : "isa-poc-remote",
            "title" : "ICA POC (Remote)",
            "desc" : "The point of contact for an interconnection on behalf of this external system to which this system connects.",
            "remarks" : "Remove this role if there are no ICAs." },
          
          { "id" : "isa-authorizing-official-local",
            "title" : "ICA Signatory (Local)",
            "desc" : "Responsible for signing an interconnection security agreement on behalf of this system.",
            "remarks" : "Remove this role if there are no ICAs." },
          
          { "id" : "isa-authorizing-official-remote",
            "title" : "ICA Signatory (Remote)",
            "desc" : "Responsible for signing an interconnection security agreement on behalf of the external system to which this system connects.",
            "remarks" : "Remove this role if there are no ICAs." },
          
          { "id" : "consultant",
            "title" : "Consultant",
            "desc" : "Any consultants involved with developing or maintaining this content." },
          
          { "id" : "admin-unix",
            "title" : "[SAMPLE]Unix Administrator",
            "desc" : "This is a sample role." },
          
          { "id" : "admin-client",
            "title" : "[SAMPLE]Client Administrator",
            "desc" : "This is a sample role." },
          
          { "id" : "program-director",
            "title" : "[SAMPLE]Program Director",
            "desc" : "This is a sample role." },
          
          { "id" : "fedramp-pmo",
            "title" : "Federal Risk and Authorization Management Program (FedRAMP) Program Management Office (PMO)",
            "short-name" : "FedRAMP PMO" },
          
          { "id" : "fedramp-jab",
            "title" : "Federal Risk and Authorization Management Program (FedRAMP) Joint Authorization Board (JAB)",
            "short-name" : "FedRAMP JAB" } ],
        "locations" : 
        [ 
          { "uuid" : "27b78960-59ef-4619-82b0-ae20b9c709ac",
            "title" : "CSP HQ",
            "address" : 
            { "type" : "work",
              "postal-address" : 
              [ "Suite 0000",
                "1234 Some Street" ],
              "city" : "Haven",
              "state" : "ME",
              "postal-code" : "00000" },
            "remarks" : "There must be one location identifying the CSP's primary business address, such as the CSP's HQ, or the address of the system owner's primary business location." },
          
          { "uuid" : "16adcc8d-65d8-4583-80d3-9cf007744fec",
            "title" : "Primary Data Center",
            "address" : 
            { "postal-address" : 
              [ "2222 Main Street" ],
              "city" : "Anywhere",
              "state" : "--",
              "postal-code" : "00000-0000" },
            "properties" : 
            [ 
              { "name" : "conformity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "data-center" },
              
              { "name" : "conformity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "primary-data-center" } ],
            "remarks" : "There must be one location for each data center.\\n\\nThere must be at least two data centers.\\n\\nFor a data center, briefly summarize the components at this location.\\n\\nAll data centers must have a conformity tag of \\\"data-center\\\".\\n\\nA primary data center must also have a conformity tag of \\\"primary-data-center\\\"." },
          
          { "uuid" : "ad321514-7b9f-4374-8409-efb18eea6e5d",
            "title" : "Secondary Data Center",
            "address" : 
            { "postal-address" : 
              [ "3333 Small Road" ],
              "city" : "Anywhere",
              "state" : "--",
              "postal-code" : "00000-0000" },
            "properties" : 
            [ 
              { "name" : "conformity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "data-center" },
              
              { "name" : "conformity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "alternate-data-center" } ],
            "remarks" : "There must be one location for each data center.\\n\\nThere must be at least two data centers.\\n\\nFor a data center, briefly summarize the components at this location.\\n\\nAll data centers must have a conformity tag of \\\"data-center\\\"\\n\\nAn alternate or backup data center must also have a conformity tag of \\\"alternate-data-center\\\"." } ],
        "parties" : 
        [ 
          { "uuid" : "6b286b5d-8f07-4fa7-8847-1dd0d88f73fb",
            "type" : "organization",
            "party-name" : "Cloud Service Provider (CSP) Name",
            "short-name" : "CSP Acronym\/Short Name",
            "location-uuids" : 
            [ "27b78960-59ef-4619-82b0-ae20b9c709ac" ],
            "remarks" : "Replace sample CSP information." },
          
          { "uuid" : "77e0e2c8-2560-4fe9-ac78-c3ff4ffc9f6d",
            "type" : "organization",
            "party-name" : "Federal Risk and Authorization Management Program: Program Management Office",
            "short-name" : "FedRAMP PMO",
            "links" : 
            [ 
              { "href" : "https:\/\/fedramp.gov",
                "text" : "" } ],
            "addresses" : 
            [ 
              { "type" : "work",
                "postal-address" : 
                [ "1800 F St. NW",
                  "" ],
                "city" : "Washington",
                "state" : "DC",
                "postal-code" : "",
                "country" : "US" } ],
            "email-addresses" : 
            [ "info@fedramp.gov" ],
            "remarks" : "This party entry must be present in a FedRAMP SSP.\\n\\nThe uuid may be different; however, the uuid must be associated with the \\\"fedramp-pmo\\\" role in the responsible-party assemblies." },
          
          { "uuid" : "49017ec3-9f51-4dbd-9253-858c2b1295fd",
            "type" : "organization",
            "party-name" : "Federal Risk and Authorization Management Program: Joint Authorization Board",
            "short-name" : "FedRAMP JAB",
            "remarks" : "This party entry must be present in a FedRAMP SSP.\\n\\nThe uuid may be different; however, the uuid must be associated with the \\\"fedramp-jab\\\" role in the responsible-party assemblies." },
          
          { "uuid" : "78992555-4a99-4eaa-868c-f2c249679dd3",
            "type" : "organization",
            "party-name" : "External Organization",
            "short-name" : "External",
            "remarks" : "Generic placeholder for any external organization." },
          
          { "uuid" : "f595397b-cbe4-4a87-8c86-9bff91c4e7fd",
            "type" : "organization",
            "party-name" : "Agency Name",
            "short-name" : "A.N.",
            "remarks" : "Generic placeholder for an authorizing agency." },
          
          { "uuid" : "8e3d39da-4851-4d2a-adb5-4b5585ded952",
            "type" : "organization",
            "party-name" : "Name of Consulting Org",
            "short-name" : "NOCO",
            "links" : 
            [ 
              { "href" : "https:\/\/consulting.sample",
                "text" : "" } ],
            "addresses" : 
            [ 
              { "type" : "work",
                "postal-address" : 
                [ "3333 Corporate Way" ],
                "city" : "Washington",
                "state" : "DC",
                "postal-code" : "",
                "country" : "US" } ],
            "email-addresses" : 
            [ "poc@consulting.sample" ] },
          
          { "uuid" : "80361ec4-bfce-4b5c-85c8-313d6ebd220b",
            "type" : "organization",
            "party-name" : "[SAMPLE]Remote System Org Name" },
          
          { "uuid" : "09ad840f-aa79-43aa-9f22-25182c2ab11b",
            "type" : "person",
            "party-name" : "[SAMPLE]ICA POC's Name",
            "properties" : 
            [ 
              { "name" : "title",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Individual's Title" } ],
            "email-addresses" : 
            [ "person@ica.org.example" ],
            "telephone-numbers" : 
            [ 
              { "number" : "202-555-1212" } ],
            "member-of-organizations" : 
            [ "80361ec4-bfce-4b5c-85c8-313d6ebd220b" ] },
          
          { "uuid" : "f0bc13a4-3303-47dd-80d3-380e159c8362",
            "type" : "organization",
            "party-name" : "[SAMPLE]Example IaaS Provider",
            "short-name" : "E.I.P.",
            "remarks" : "Underlying service provider. Leveraged Authorization." },
          
          { "uuid" : "3360e343-9860-4bda-9dfc-ff427c3dfab6",
            "type" : "person",
            "party-name" : "[SAMPLE]Person Name 1",
            "properties" : 
            [ 
              { "name" : "title",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Individual's Title" } ],
            "addresses" : 
            [ 
              { "postal-address" : 
                [ "Mailstop A-1" ] } ],
            "email-addresses" : 
            [ "name@org.domain" ],
            "telephone-numbers" : 
            [ 
              { "number" : "202-000-0001" } ],
            "member-of-organizations" : 
            [ "6b286b5d-8f07-4fa7-8847-1dd0d88f73fb" ],
            "location-uuids" : 
            [ "27b78960-59ef-4619-82b0-ae20b9c709ac" ] },
          
          { "uuid" : "36b8d6c0-3b25-42cc-b529-cf4066145cdd",
            "type" : "person",
            "party-name" : "[SAMPLE]Person Name 2",
            "properties" : 
            [ 
              { "name" : "title",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Individual's Title" } ],
            "addresses" : 
            [ 
              { "type" : "work",
                "postal-address" : 
                [ "Address Line" ],
                "city" : "City",
                "state" : "ST",
                "postal-code" : "00000",
                "country" : "US" } ],
            "email-addresses" : 
            [ "name@org.domain" ],
            "telephone-numbers" : 
            [ 
              { "number" : "202-000-0002" } ],
            "member-of-organizations" : 
            [ "6b286b5d-8f07-4fa7-8847-1dd0d88f73fb" ] },
          
          { "uuid" : "0cec09d9-20c6-470b-9ffc-85763375880b",
            "type" : "person",
            "party-name" : "[SAMPLE]Person Name 3",
            "properties" : 
            [ 
              { "name" : "title",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Individual's Title" } ],
            "addresses" : 
            [ 
              { "type" : "work",
                "postal-address" : 
                [ "Address Line" ],
                "city" : "City",
                "state" : "ST",
                "postal-code" : "00000",
                "country" : "US" } ],
            "email-addresses" : 
            [ "name@org.domain" ],
            "telephone-numbers" : 
            [ 
              { "number" : "202-000-0003" } ],
            "member-of-organizations" : 
            [ "6b286b5d-8f07-4fa7-8847-1dd0d88f73fb" ] },
          
          { "uuid" : "f75e21f6-43d8-46ab-890d-7f2eebc5a830",
            "type" : "person",
            "party-name" : "[SAMPLE]Person Name 4",
            "properties" : 
            [ 
              { "name" : "title",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Individual's Title" } ],
            "addresses" : 
            [ 
              { "type" : "work",
                "postal-address" : 
                [ "Address Line" ],
                "city" : "City",
                "state" : "ST",
                "postal-code" : "00000",
                "country" : "US" } ],
            "email-addresses" : 
            [ "name@org.domain" ],
            "telephone-numbers" : 
            [ 
              { "number" : "202-000-0004" } ],
            "member-of-organizations" : 
            [ "6b286b5d-8f07-4fa7-8847-1dd0d88f73fb" ] },
          
          { "uuid" : "132953a9-640c-46f7-9de9-3fa15ec99361",
            "type" : "person",
            "party-name" : "[SAMPLE]Person Name 5",
            "properties" : 
            [ 
              { "name" : "title",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Individual's Title" } ],
            "addresses" : 
            [ 
              { "type" : "work",
                "postal-address" : 
                [ "Address Line" ],
                "city" : "City",
                "state" : "ST",
                "postal-code" : "00000",
                "country" : "US" } ],
            "email-addresses" : 
            [ "name@org.domain" ],
            "telephone-numbers" : 
            [ 
              { "number" : "202-000-0005" } ],
            "member-of-organizations" : 
            [ "6b286b5d-8f07-4fa7-8847-1dd0d88f73fb" ] },
          
          { "uuid" : "4fded5fd-7a65-47ea-bd76-df57c46e27d1",
            "type" : "person",
            "party-name" : "[SAMPLE]Person Name 6",
            "properties" : 
            [ 
              { "name" : "title",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Individual's Title" } ],
            "addresses" : 
            [ 
              { "type" : "work",
                "postal-address" : 
                [ "Address Line" ],
                "city" : "City",
                "state" : "ST",
                "postal-code" : "00000",
                "country" : "US" } ],
            "email-addresses" : 
            [ "name@org.domain" ],
            "telephone-numbers" : 
            [ 
              { "number" : "202-000-0006" } ],
            "member-of-organizations" : 
            [ "78992555-4a99-4eaa-868c-f2c249679dd3" ] },
          
          { "uuid" : "db234cb7-1776-425c-9ac4-b067c1723011",
            "type" : "person",
            "party-name" : "[SAMPLE]Person Name 7",
            "properties" : 
            [ 
              { "name" : "title",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Individual's Title" } ],
            "addresses" : 
            [ 
              { "type" : "work",
                "postal-address" : 
                [ "Address Line" ],
                "city" : "City",
                "state" : "ST",
                "postal-code" : "00000",
                "country" : "US" } ],
            "email-addresses" : 
            [ "name@org.domain" ],
            "telephone-numbers" : 
            [ 
              { "number" : "202-000-0007" } ],
            "member-of-organizations" : 
            [ "6b286b5d-8f07-4fa7-8847-1dd0d88f73fb" ] },
          
          { "uuid" : "b306f5af-b93a-4a7f-a2b2-37a44fc92a79",
            "type" : "organization",
            "party-name" : "[SAMPLE] IT Department" },
          
          { "uuid" : "59cdc953-5902-4fa4-a878-f3163854624c",
            "type" : "organization",
            "party-name" : "[SAMPLE]Security Team" } ],
        "responsible-parties" : 
        { "cloud-service-provider" : 
          { "party-uuids" : 
            [ "6b286b5d-8f07-4fa7-8847-1dd0d88f73fb" ],
            "remarks" : "Exactly one" },
          "prepared-by" : 
          { "party-uuids" : 
            [ "3360e343-9860-4bda-9dfc-ff427c3dfab6" ],
            "remarks" : "Exactly one" },
          "prepared-for" : 
          { "party-uuids" : 
            [ "6b286b5d-8f07-4fa7-8847-1dd0d88f73fb" ] },
          "content-approver" : 
          { "party-uuids" : 
            [ "3360e343-9860-4bda-9dfc-ff427c3dfab6",
              "36b8d6c0-3b25-42cc-b529-cf4066145cdd" ],
            "remarks" : "One or more" },
          "system-owner" : 
          { "party-uuids" : 
            [ "3360e343-9860-4bda-9dfc-ff427c3dfab6" ],
            "remarks" : "Exactly one" },
          "authorizing-official" : 
          { "party-uuids" : 
            [ "49017ec3-9f51-4dbd-9253-858c2b1295fd",
              "4fded5fd-7a65-47ea-bd76-df57c46e27d1" ],
            "remarks" : "One or more" },
          "system-poc-management" : 
          { "party-uuids" : 
            [ "0cec09d9-20c6-470b-9ffc-85763375880b" ],
            "remarks" : "Exactly one" },
          "system-poc-technical" : 
          { "party-uuids" : 
            [ "f75e21f6-43d8-46ab-890d-7f2eebc5a830" ],
            "remarks" : "Exactly one" },
          "information-system-security-officer" : 
          { "party-uuids" : 
            [ "132953a9-640c-46f7-9de9-3fa15ec99361" ],
            "remarks" : "Exactly one" },
          "authorizing-official-poc" : 
          { "party-uuids" : 
            [ "4fded5fd-7a65-47ea-bd76-df57c46e27d1" ],
            "remarks" : "Exactly one" },
          "privacy-poc" : 
          { "party-uuids" : 
            [ "db234cb7-1776-425c-9ac4-b067c1723011" ],
            "remarks" : "Exactly one" },
          "fedramp-pmo" : 
          { "party-uuids" : 
            [ "77e0e2c8-2560-4fe9-ac78-c3ff4ffc9f6d" ],
            "remarks" : "Exactly one" },
          "fedramp-jab" : 
          { "party-uuids" : 
            [ "49017ec3-9f51-4dbd-9253-858c2b1295fd" ],
            "remarks" : "Exactly one" } },
        "remarks" : "This OSCAL-based FedRAMP SSP Template can be used for the FedRAMP Low, Moderate, and\n            High baselines.\\n\\nGuidance for OSCAL-based FedRAMP Tailored content has not yet been developed." },
      "import-profile" : 
      { "href" : "#890170c3-d4fa-4d25-ab96-8e4bf7cc237c" },
      "system-characteristics" : 
      { "system-ids" : 
        [ 
          { "identifier-type" : "https:\/\/fedramp.gov",
            "id" : "F00000000" } ],
        "system-name" : "System's Full Name",
        "system-name-short" : "System's Short Name or Acronym",
        "description" : "Describe the purpose and functions of this system here.",
        "properties" : 
        [ 
          { "name" : "authorization-type",
            "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
            "value" : "fedramp-agency" },
          
          { "name" : "security-eauth-level",
            "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
            "class" : "security-eauth",
            "value" : "2" },
          
          { "name" : "identity-assurance-level",
            "value" : "2" },
          
          { "name" : "authenticator-assurance-level",
            "value" : "2" },
          
          { "name" : "federation-assurance-level",
            "value" : "2" } ],
        "annotations" : 
        [ 
          { "name" : "cloud-service-model",
            "value" : "saas",
            "remarks" : "Remarks are required if service model is \\\"other\\\". Optional otherwise." },
          
          { "name" : "cloud-deployment-model",
            "value" : "government-only-cloud",
            "remarks" : "Remarks are required if deployment model is \\\"hybrid-cloud\\\" or \\\"other\\\". Optional\n               otherwise." } ],
        "security-sensitivity-level" : "low",
        "system-information" : 
        { "properties" : 
          [ 
            { "name" : "privacy-sensitive",
              "value" : "yes" },
            
            { "name" : "pta-1",
              "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
              "class" : "pta",
              "value" : "yes" },
            
            { "name" : "pta-2",
              "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
              "class" : "pta",
              "value" : "yes" },
            
            { "name" : "pta-3",
              "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
              "class" : "pta",
              "value" : "yes" },
            
            { "name" : "pta-4",
              "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
              "class" : "pta",
              "value" : "no" },
            
            { "name" : "sorn-id",
              "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
              "class" : "pta",
              "value" : "[No SORN ID]" } ],
          "information-types" : 
          [ 
            { "uuid" : "06ecba4f-db96-4491-a3a2-7febfa227435",
              "title" : "Information Type Name",
              "description" : "A description of the information.",
              "information-type-ids" : 
              { "https:\/\/doi.org\/10.6028\/NIST.SP.800-60v2r1" : 
                { "id" : "C.2.4.1" } },
              "confidentiality-impact" : 
              { "base" : "fips-199-moderate",
                "selected" : "fips-199-moderate",
                "adjustment-justification" : "Required if the base and selected values do not match." },
              "integrity-impact" : 
              { "base" : "fips-199-moderate",
                "selected" : "fips-199-moderate",
                "adjustment-justification" : "Required if the base and selected values do not match." },
              "availability-impact" : 
              { "base" : "fips-199-moderate",
                "selected" : "fips-199-moderate",
                "adjustment-justification" : "Required if the base and selected values do not match." } } ] },
        "security-impact-level" : 
        { "security-objective-confidentiality" : "fips-199-moderate",
          "security-objective-integrity" : "fips-199-moderate",
          "security-objective-availability" : "fips-199-moderate" },
        "status" : 
        { "state" : "operational",
          "remarks" : "Remarks are required if status\/state is \\\"other\\\". Optional otherwise." },
        "authorization-boundary" : 
        { "description" : "A holistic, top-level explanation of the FedRAMP authorization boundary.",
          "diagrams" : 
          { "dbf46c27-52a9-49c4-beb6-b6399cd75497" : 
            { "description" : "A diagram-specific explanation.",
              "links" : 
              [ 
                { "href" : "#d2eb3c18-6754-4e3a-a933-03d289e3fad5",
                  "rel" : "diagram",
                  "text" : "" } ],
              "caption" : "Authorization Boundary Diagram" } } },
        "network-architecture" : 
        { "description" : "A holistic, top-level explanation of the network architecture.",
          "diagrams" : 
          { "e97c3395-433a-48c1-8cc7-dd1e1555941c" : 
            { "description" : "A diagram-specific explanation.",
              "links" : 
              [ 
                { "href" : "#61081e81-850b-43c1-bf43-1ecbddcb9e7f",
                  "rel" : "diagram",
                  "text" : "" } ],
              "caption" : "Network Diagram" } } },
        "data-flow" : 
        { "description" : "A holistic, top-level explanation of the system's data flows.",
          "diagrams" : 
          { "e3b98448-4219-46a5-b229-412423c566f3" : 
            { "description" : "A diagram-specific explanation.",
              "links" : 
              [ 
                { "href" : "#ac5d7535-f3b8-45d3-bf3b-735c82c64547",
                  "rel" : "diagram",
                  "text" : "" } ],
              "caption" : "Data Flow Diagram" } } } },
      "system-implementation" : 
      { "properties" : 
        [ 
          { "name" : "users-internal",
            "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
            "value" : "0" },
          
          { "name" : "users-external",
            "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
            "value" : "0" },
          
          { "name" : "users-internal-future",
            "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
            "value" : "0" },
          
          { "name" : "users-external-future",
            "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
            "value" : "0" } ],
        "leveraged-authorizations" : 
        [ 
          { "uuid" : "5a9c98ab-8e5e-433d-a7bd-515c07cd1497",
            "title" : "Name of Underlying System",
            "party-uuid" : "f0bc13a4-3303-47dd-80d3-380e159c8362",
            "date-authorized" : "2015-01-01",
            "remarks" : "The leveraged-authorizaton assembly is supposed to have a required uuid flag instead of an optional id flag. This will be fixed in the syntax shortly.\\n\\nUse one leveraged-authorization assembly for each underlying system. (In the legacy world, these may be general support systems." } ],
        "users" : 
        { "9cb0fab0-78bd-44ba-bcb8-3e9801cc952f" : 
          { "title" : "[SAMPLE]Unix System Administrator",
            "properties" : 
            [ 
              { "name" : "sensitivity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "high" } ],
            "annotations" : 
            [ 
              { "name" : "privilege-level",
                "value" : "privileged" },
              
              { "name" : "type",
                "value" : "internal" } ],
            "role-ids" : 
            [ "admin-unix" ],
            "authorized-privileges" : 
            [ 
              { "title" : "Full administrative access (root)",
                "functions-performed" : 
                [ "Add\/remove users and hardware",
                  "install and configure software",
                  "OS updates, patches and hotfixes",
                  "perform backups" ] } ] },
          "16ec71e7-025c-43e4-9d3f-3acb485fac2e" : 
          { "title" : "[SAMPLE]Client Administrator",
            "properties" : 
            [ 
              { "name" : "sensitivity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "moderate" } ],
            "annotations" : 
            [ 
              { "name" : "privilege-level",
                "value" : "non-privileged" },
              
              { "name" : "type",
                "value" : "external" } ],
            "role-ids" : 
            [ "external" ],
            "authorized-privileges" : 
            [ 
              { "title" : "Portal administration",
                "functions-performed" : 
                [ "Add\/remove client users",
                  "Create, modify and delete client applications" ] } ] },
          "ba7708c1-4041-48ab-9b7b-1ddb5e175fe0" : 
          { "title" : "[SAMPLE]Program Director",
            "properties" : 
            [ 
              { "name" : "sensitivity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "limited" } ],
            "annotations" : 
            [ 
              { "name" : "privilege-level",
                "value" : "no-logical-access" },
              
              { "name" : "type",
                "value" : "internal" } ],
            "role-ids" : 
            [ "program-director" ],
            "authorized-privileges" : 
            [ 
              { "title" : "Administrative Access Approver",
                "functions-performed" : 
                [ "Approves access requests for administrative accounts." ] },
              
              { "title" : "Access Approver",
                "functions-performed" : 
                [ "Approves access requests for administrative accounts." ] } ] } },
        "components" : 
          { {% for component in system.producer_elements %}
            "{{ component.uuid }}" : 
              { "component-type" : "{{ component.element_type }}",
                "title" : "{{ component.name }}",
                "description" : "{% if component.description %}{{ component.description|safe}}{% else %}<p>None.</p>{% endif %}",
                "status" : 
                { "state" : "operational" } 
              }{% if loop.last %}{% else %},{% endif %}{% endfor %}
          },
        "system-inventory" : 
        { "inventory-items" : 
          { "98e37f90-fbb5-4177-badb-9b55229cc183" : 
            { "asset-id" : "unique-asset-id",
              "description" : "Flat-File Example (No implemented-component).",
              "properties" : 
              [ 
                { "name" : "ipv4-address",
                  "value" : "10.1.1.1" },
                
                { "name" : "ipv6-address",
                  "value" : "0000:0000:0000:0000" },
                
                { "name" : "virtual",
                  "value" : "no" },
                
                { "name" : "public",
                  "value" : "no" },
                
                { "name" : "fqdn",
                  "value" : "dns.name" },
                
                { "name" : "uri",
                  "value" : "uniform.resource.identifier" },
                
                { "name" : "netbios-name",
                  "value" : "netbios-name" },
                
                { "name" : "mac-address",
                  "value" : "00:00:00:00:00:00" },
                
                { "name" : "software-name",
                  "value" : "software-name" },
                
                { "name" : "version",
                  "value" : "V 0.0.0" },
                
                { "name" : "asset-type",
                  "value" : "os" },
                
                { "name" : "vendor-name",
                  "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                  "value" : "Vendor Name" },
                
                { "name" : "model",
                  "value" : "Model Number" },
                
                { "name" : "patch-level",
                  "value" : "Patch-Level" },
                
                { "name" : "serial-number",
                  "value" : "Serial #" },
                
                { "name" : "asset-tag",
                  "value" : "Asset Tag" },
                
                { "name" : "vlan-id",
                  "value" : "VLAN Identifier" },
                
                { "name" : "network-id",
                  "value" : "Network Identifier" },
                
                { "name" : "scan-type",
                  "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                  "value" : "infrastructure" },
                
                { "name" : "scan-type",
                  "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                  "value" : "database" },
                
                { "name" : "validation",
                  "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                  "value" : "component-id" } ],
              "annotations" : 
              [ 
                { "name" : "allows-authenticated-scan",
                  "value" : "no",
                  "remarks" : "If no, explain why. If yes, omit remarks field." },
                
                { "name" : "baseline-configuration-name",
                  "value" : "Baseline Config. Name" },
                
                { "name" : "physical-location",
                  "value" : "Physical location of Asset" },
                
                { "name" : "is-scanned",
                  "value" : "yes",
                  "remarks" : "If no, explain why. If yes, omit remarks field." },
                
                { "name" : "function",
                  "value" : "Required brief, text-based description.",
                  "remarks" : "Optional, longer, formatted description." } ],
              "responsible-parties" : 
              { "asset-owner" : 
                { "party-uuids" : 
                  [ "db234cb7-1776-425c-9ac4-b067c1723011" ] },
                "asset-administrator" : 
                { "party-uuids" : 
                  [ "b306f5af-b93a-4a7f-a2b2-37a44fc92a79" ] } },
              "remarks" : "COMMENTS: Additional information about this item." },
            "c916d3c5-229e-4786-bf3f-4d71baa0e7a5" : 
            { "asset-id" : "unique-asset-ID",
              "description" : "Component Inventory Example",
              "properties" : 
              [ 
                { "name" : "ipv4-address",
                  "value" : "10.2.2.2" },
                
                { "name" : "ipv6-address",
                  "value" : "0000:0000:0000:0000" },
                
                { "name" : "mac-address",
                  "value" : "00:00:00:00:00:00" },
                
                { "name" : "virtual",
                  "value" : "no" },
                
                { "name" : "public",
                  "value" : "no" },
                
                { "name" : "fqdn",
                  "value" : "dns.name" },
                
                { "name" : "uri",
                  "value" : "uniform.resource.locator" },
                
                { "name" : "netbios-name",
                  "value" : "netbios-name" },
                
                { "name" : "patch-level",
                  "value" : "Patch-Level" } ],
              "annotations" : 
              [ 
                { "name" : "baseline-configuration-name",
                  "value" : "Baseline Configuration Name" },
                
                { "name" : "physical-location",
                  "value" : "Physical location of Asset" },
                
                { "name" : "scan-authenticated",
                  "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                  "value" : "no",
                  "remarks" : "If no, explain why. If yes, omit remark." },
                
                { "name" : "scan-latest",
                  "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                  "value" : "yes",
                  "remarks" : "If no, explain why. If yes, omit remark." } ],
              "responsible-parties" : 
              { "asset-owner" : 
                { "party-uuids" : 
                  [ "3360e343-9860-4bda-9dfc-ff427c3dfab6" ] },
                "asset-administrator" : 
                { "party-uuids" : 
                  [ "b306f5af-b93a-4a7f-a2b2-37a44fc92a79" ] } },
              "implemented-components" : 
              { "05ceb8df-52e7-49db-9719-891723f366bd" : 
                {  } },
              "remarks" : "COMMENTS: If needed, provide additional information about this inventory item." },
            "37c00d5a-ccf2-4112-a0ee-8460be8cff40" : 
            { "asset-id" : "unique-asset-id",
              "description" : "None.",
              "properties" : 
              [ 
                { "name" : "ipv4-address",
                  "value" : "10.3.3.3" } ],
              "annotations" : 
              [ 
                { "name" : "is-scanned",
                  "value" : "yes" } ],
              "implemented-components" : 
              { "1541015b-6d19-42cb-a991-624cc082ed4d" : 
                {  } } },
            "fb7a84fb-7e30-4f5b-9997-2ecd4d270bdd" : 
            { "asset-id" : "unique-asset-id",
              "description" : "None.",
              "properties" : 
              [ 
                { "name" : "ipv4-address",
                  "value" : "10.4.4.4" } ],
              "annotations" : 
              [ 
                { "name" : "is-scanned",
                  "value" : "yes" } ],
              "implemented-components" : 
              { "05ceb8df-52e7-49db-9719-891723f366bd" : 
                {  } } },
            "779d4e89-bba6-432c-b50d-d699fe534129" : 
            { "asset-id" : "unique-asset-id",
              "description" : "None.",
              "properties" : 
              [ 
                { "name" : "ipv4-address",
                  "value" : "10.5.5.5" } ],
              "annotations" : 
              [ 
                { "name" : "is-scanned",
                  "value" : "yes" } ],
              "implemented-components" : 
              { "8f230d84-2f9b-44a3-acdb-019566ab2554" : 
                {  } } },
            "20b207d5-5e77-4501-b02d-5d2a6e88db85" : 
            { "asset-id" : "unique-asset-id",
              "description" : "None.",
              "properties" : 
              [ 
                { "name" : "ipv4-address",
                  "value" : "10.6.6.6" } ],
              "annotations" : 
              [ 
                { "name" : "is-scanned",
                  "value" : "no",
                  "remarks" : "Asset wasn't running at time of scan." } ],
              "implemented-components" : 
              { "05ceb8df-52e7-49db-9719-891723f366bd" : 
                {  } } },
            "79b4f0d1-91ab-49e8-af28-045c12aa9272" : 
            { "asset-id" : "unique-asset-id",
              "description" : "None.",
              "properties" : 
              [ 
                { "name" : "ipv4-address",
                  "value" : "10.7.7.7" } ],
              "annotations" : 
              [ 
                { "name" : "is-scanned",
                  "value" : "yes" } ],
              "implemented-components" : 
              { "1541015b-6d19-42cb-a991-624cc082ed4d" : 
                {  } } },
            "b31b360d-b58b-4c7c-b344-68e17238d858" : 
            { "asset-id" : "unique-asset-id",
              "description" : "None.",
              "properties" : 
              [ 
                { "name" : "ipv4-address",
                  "value" : "10.8.8.8" } ],
              "annotations" : 
              [ 
                { "name" : "is-scanned",
                  "value" : "no",
                  "remarks" : "Asset wasn't running at time of scan." } ],
              "implemented-components" : 
              { "05ceb8df-52e7-49db-9719-891723f366bd" : 
                {  } } },
            "55b55b3d-3bd9-409a-bc87-3b9a2074bacd" : 
            { "asset-id" : "10.10.10.0",
              "description" : "IPv4 Production Subnet.",
              "properties" : 
              [ 
                { "name" : "ipv4-subnet",
                  "value" : "10.10.10.0\/24" } ],
              "annotations" : 
              [ 
                { "name" : "is-scanned",
                  "value" : "yes" } ] },
            "c0dbefa1-c8e8-4ca8-bd73-67cb7b1fa3f6" : 
            { "asset-id" : "10.10.20.0",
              "description" : "IPv4 Management Subnet.",
              "properties" : 
              [ 
                { "name" : "ipv4-subnet",
                  "value" : "10.10.20.0\/24" } ],
              "annotations" : 
              [ 
                { "name" : "is-scanned",
                  "value" : "yes" } ] } } } },
      "control-implementation" : 
      { "description" : "FedRAMP SSP Template Section 13\\n\\nThis description field is required by OSCAL. FedRAMP does not require any specific\n            information here.",

        "implemented-requirements" : 
        [
          {% for control in system.root_element.selected_controls_oscal_ctl_ids %}
            {% if control.lower() in control_catalog %}
            { "uuid" : "{{ system.control_implementation_as_dict[control]['elementcontrol_uuid'] }}",
              "control-id": "{{ control.lower() }}",
              "statements":
              { "{{ control.lower() }}_stmt" :
                { "uuid" : "{{ system.control_implementation_as_dict[control]['combined_smt_uuid'] }}",
                  "title": "{{ control_catalog[control.lower()]['title'] }}",
                  "description" : "{#control_catalog[control.lower()]['description']|safe#}",
                  "by-components" :{% if control in system.control_implementation_as_dict %}[
                    {% for smt in system.control_implementation_as_dict[control]['control_impl_smts'] %}
                      { "{{ smt.producer_element.uuid }}" : 
                        { "uuid" : "{{ smt.uuid }}",
                          "component-name": "{{ smt.producer_element.name }}",
                          "description" : "{{ smt.body|safe }}"
                        }
                      }{% if loop.last %}{% else %},{% endif %}
                    {% endfor %}]
                  {% endif %}
                }
              }
            }{% if loop.last %}{% else %},{% endif %}
            {% endif %}
          {% endfor %}
        ]
      },

      "back-matter" : 
      { "resources" : 
        [ 
          { "uuid" : "3a5ca2de-0f66-47e6-844d-6ccdf214b767",
            "title" : "FedRAMP Applicable Laws and Regulations",
            "properties" : 
            [ 
              { "name" : "conformity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "fedramp-citations" } ],
            "rlinks" : 
            [ 
              { "href" : "https:\/\/www.fedramp.gov\/assets\/resources\/templates\/SSP-A12-FedRAMP-Laws-and-Regulations-Template.xlsx" } ] },
          
          { "uuid" : "12da89ef-51dd-4404-948d-e9f0e25b961e",
            "title" : "FedRAMP Master Acronym and Glossary",
            "properties" : 
            [ 
              { "name" : "conformity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "fedramp-acronyms" } ],
            "rlinks" : 
            [ 
              { "href" : "https:\/\/www.fedramp.gov\/assets\/resources\/documents\/FedRAMP_Master_Acronym_and_Glossary.pdf" } ] },
          
          { "uuid" : "d45612a9-cf25-4ef6-b2dd-69e38ba2967a",
            "title" : "[SAMPLE]Name or Title of Document",
            "properties" : 
            [ 
              { "name" : "type",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "law" },
              
              { "name" : "publication",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Publication Date" } ],
            "document-ids" : 
            [ 
              { "type" : "doi",
                "identifier" : "Identification Number" } ],
            "rlinks" : 
            [ 
              { "href" : "https:\/\/domain.example\/path\/to\/document.pdf" } ] },
          
          { "uuid" : "a8a0cc81-800f-479f-93d3-8b8743d9b98d",
            "title" : "[SAMPLE]Privacy-Related Law Citation",
            "properties" : 
            [ 
              { "name" : "type",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "law" },
              
              { "name" : "type",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "pii" },
              
              { "name" : "publication",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Publication Date" } ],
            "document-ids" : 
            [ 
              { "type" : "doi",
                "identifier" : "Identification Number" } ],
            "rlinks" : 
            [ 
              { "href" : "https:\/\/domain.example\/path\/to\/document.pdf" } ] },
          
          { "uuid" : "545e75c3-537f-48fe-9630-95337916d982",
            "title" : "[SAMPLE]Regulation Citation",
            "properties" : 
            [ 
              { "name" : "type",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "regulation" },
              
              { "name" : "publication",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Publication Date" } ],
            "document-ids" : 
            [ 
              { "type" : "doi",
                "identifier" : "Identification Number" } ],
            "rlinks" : 
            [ 
              { "href" : "https:\/\/domain.example\/path\/to\/document.pdf" } ] },
          
          { "uuid" : "9d6cf2b4-8e88-4040-a33c-7bc206553a1a",
            "title" : "[SAMPLE]Interconnection Security Agreement Title",
            "properties" : 
            [ 
              { "name" : "publication",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Date" },
              
              { "name" : "version",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Version" } ] },
          
          { "uuid" : "31a46c4f-2959-4287-bc1c-67297d7da60b",
            "desc" : "CSP Logo",
            "properties" : 
            [ 
              { "name" : "conformity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "prepared-for-logo" },
              
              { "name" : "conformity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "csp-logo" } ],
            "rlinks" : 
            [ 
              { "href" : ".\/logo.png",
                "media-type" : "image\/png" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ] },
          
          { "uuid" : "c5866ad8-8ed7-49b4-844a-0276fa9f8f51",
            "desc" : "Preparer Logo",
            "properties" : 
            [ 
              { "name" : "conformity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "prepared-by-logo" } ],
            "rlinks" : 
            [ 
              { "href" : ".\/party-1-logo.png",
                "media-type" : "image\/png" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ] },
          
          { "uuid" : "0846b6ef-cfa4-4bb3-8280-717f7e7b04d4  ",
            "desc" : "FedRAMP Logo",
            "properties" : 
            [ 
              { "name" : "conformity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "fedramp-logo" } ],
            "rlinks" : 
            [ 
              { "href" : "https:\/\/github.com\/GSA\/fedramp-automation\/raw\/master\/assets\/FedRAMP_LOGO.png" } ] },
          
          { "uuid" : "2c1747d6-874a-49a2-8488-2fd9735416bf",
            "desc" : "3PAO Logo",
            "properties" : 
            [ 
              { "name" : "conformity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "3pao-logo" } ],
            "rlinks" : 
            [ 
              { "href" : ".\/logo.png",
                "media-type" : "image\/png" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ] },
          
          { "uuid" : "d2eb3c18-6754-4e3a-a933-03d289e3fad5",
            "desc" : "The primary authorization boundary diagram.",
            "rlinks" : 
            [ 
              { "href" : ".\/diagrams\/boundary.png" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ],
            "remarks" : "Section 9.2, Figure 9-1 Authorization Boundary Diagram (graphic)\\n\\nThis should be referenced in the\n               system-characteristics\/authorization-boundary\/diagram\/link\/@href flag using a value\n               of \\\"#d2eb3c18-6754-4e3a-a933-03d289e3fad5\\\"" },
          
          { "uuid" : "61081e81-850b-43c1-bf43-1ecbddcb9e7f",
            "desc" : "The primary network diagram.",
            "rlinks" : 
            [ 
              { "href" : ".\/diagrams\/network.png" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ],
            "remarks" : "Section 9.4, Figure 9-2 Network Diagram (graphic)\\n\\nThis should be referenced in the\n               system-characteristics\/network-architecture\/diagram\/link\/@href flag using a value\n               of \\\"#61081e81-850b-43c1-bf43-1ecbddcb9e7f\\\"" },
          
          { "uuid" : "ac5d7535-f3b8-45d3-bf3b-735c82c64547",
            "desc" : "The primary data flow diagram.",
            "rlinks" : 
            [ 
              { "href" : ".\/diagrams\/dataflow.png" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ],
            "remarks" : "Section 10, Figure 10-1 Data Flow Diagram (graphic)\\n\\nThis should be referenced in the\n               system-characteristics\/data-flow\/diagram\/link\/@href flag using a value\n               of \\\"#ac5d7535-f3b8-45d3-bf3b-735c82c64547\\\"" },
          
          { "uuid" : "090ab379-2089-4830-b9fd-26d0729e22e9",
            "title" : "Policy Title",
            "desc" : "Policy document",
            "properties" : 
            [ 
              { "name" : "type",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "policy" },
              
              { "name" : "publication",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Date" },
              
              { "name" : "version",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Version" } ],
            "rlinks" : 
            [ 
              { "href" : ".\/sample_policy.pdf" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ],
            "remarks" : "Table 15-1 Attachments: Policy Attachment" },
          
          { "uuid" : "ab300133-d749-4abb-b858-1cd6ffd8af9e",
            "title" : "Policy Title",
            "desc" : "Policy document",
            "properties" : 
            [ 
              { "name" : "type",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "policy" },
              
              { "name" : "publication",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Date" },
              
              { "name" : "version",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Version" } ],
            "rlinks" : 
            [ 
              { "href" : ".\/sample_policy.pdf" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ],
            "remarks" : "Table 15-1 Attachments: Policy Attachment" },
          
          { "uuid" : "1002a58e-9e11-4aa6-9ab4-2bde52995952",
            "title" : "Procedure Title",
            "desc" : "Procedure document",
            "properties" : 
            [ 
              { "name" : "type",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "procedure" },
              
              { "name" : "publication",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Date" },
              
              { "name" : "version",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Version" } ],
            "rlinks" : 
            [ 
              { "href" : ".\/sample_procedure.pdf" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ],
            "remarks" : "Table 15-1 Attachments: Procedure Attachment" },
          
          { "uuid" : "4bb1e2e5-261c-4b5c-b22c-e1627c2e8be6",
            "title" : "Procedure Title",
            "desc" : "Procedure document",
            "properties" : 
            [ 
              { "name" : "type",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "procedure" },
              
              { "name" : "publication",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Date" },
              
              { "name" : "version",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Version" } ],
            "rlinks" : 
            [ 
              { "href" : ".\/sample_procedure.pdf" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ],
            "remarks" : "Table 15-1 Attachments: Procedure Attachment" },
          
          { "uuid" : "90a128ac-c850-48f6-8fff-a55692f80b41",
            "title" : "User's Guide",
            "desc" : "User's Guide",
            "properties" : 
            [ 
              { "name" : "conformity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "user-guide" },
              
              { "name" : "type",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "guide" },
              
              { "name" : "publication",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Date" },
              
              { "name" : "version",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Version" } ],
            "rlinks" : 
            [ 
              { "href" : ".\/sample_guide.pdf" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ],
            "remarks" : "Table 15-1 Attachments: User's Guide Attachment" },
          
          { "uuid" : "fab59751-b855-40cb-93c1-492562e20e18",
            "title" : "Privacy Impact Assessment",
            "properties" : 
            [ 
              { "name" : "conformity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "privacy-impact-assessment" },
              
              { "name" : "publication",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Date" },
              
              { "name" : "version",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Version" } ],
            "rlinks" : 
            [ 
              { "href" : ".\/pia.docx" } ],
            "attachments" : 
            [ 
              { "filename" : "pia.docx",
                "value" : "00000000" } ],
            "remarks" : "Table 15-1 Attachments: Privacy Impact Assessment" },
          
          { "uuid" : "489112e1-57f2-4c29-8dd0-95b1442fbf3b",
            "title" : "Document Title",
            "desc" : "Rules of Behavior",
            "properties" : 
            [ 
              { "name" : "conformity",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "rules-of-behavior" },
              
              { "name" : "type",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "rob" },
              
              { "name" : "publication",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Date" },
              
              { "name" : "version",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Version" } ],
            "rlinks" : 
            [ 
              { "href" : "https:\/\/sample" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ],
            "remarks" : "Table 15-1 Attachments: Rules of Behavior (ROB)" },
          
          { "uuid" : "c7860916-f2f4-43aa-b578-d48cf8e6d381",
            "title" : "Document Title",
            "desc" : "Contingency Plan (CP)",
            "properties" : 
            [ 
              { "name" : "type",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "plan" },
              
              { "name" : "publication",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Date" },
              
              { "name" : "version",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Version" } ],
            "rlinks" : 
            [ 
              { "href" : "https:\/\/sample" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ],
            "remarks" : "Table 15-1 Attachments: Contingency Plan (CP) Attachment" },
          
          { "uuid" : "ab56cf27-0dae-40d6-89b7-d750137309af",
            "title" : "Document Title",
            "desc" : "Configuration Management (CM) Plan",
            "properties" : 
            [ 
              { "name" : "type",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "plan" },
              
              { "name" : "publication",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Date" },
              
              { "name" : "version",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Version" } ],
            "rlinks" : 
            [ 
              { "href" : "https:\/\/sample" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ],
            "remarks" : "Table 15-1 Attachments: Configuration Management (CM) Plan Attachment" },
          
          { "uuid" : "3f771ab5-8016-4571-98d1-f0fb962e15e2",
            "title" : "Document Title",
            "desc" : "Incident Response (IR) Plan",
            "properties" : 
            [ 
              { "name" : "type",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "plan" },
              
              { "name" : "publication",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Date" },
              
              { "name" : "version",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Version" } ],
            "rlinks" : 
            [ 
              { "href" : "https:\/\/sample" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ],
            "remarks" : "Table 15-1 Attachments: Incident Response (IR) Plan Attachment" },
          
          { "uuid" : "49fb4631-1da2-41ca-b0b3-e1b1006d4025",
            "title" : "Separation of Duties Matrix",
            "desc" : "Separation of Duties Matrix",
            "properties" : 
            [ 
              { "name" : "publication",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Date" },
              
              { "name" : "version",
                "ns" : "https:\/\/fedramp.gov\/ns\/oscal",
                "value" : "Document Version" } ],
            "rlinks" : 
            [ 
              { "href" : "https:\/\/sample" } ],
            "attachments" : 
            [ 
              { "value" : "00000000" } ],
            "remarks" : "Table 15-1 Attachments: Separation of Duties Matrix Attachment" },
          
          { "uuid" : "9f1aae37-7359-411f-86c1-768aaab85e63",
            "title" : "FedRAMP High Baseline",
            "rlinks" : 
            [ 
              { "href" : "https:\/\/raw.githubusercontent.com\/usnistgov\/OSCAL\/v1.0.0-milestone3\/content\/fedramp.gov\/xml\/FedRAMP_HIGH-baseline_profile.xml",
                "media-type" : "application\/xml" } ],
            "remarks" : "Pointer to High baseline content in OSCAL." },
          
          { "uuid" : "890170c3-d4fa-4d25-ab96-8e4bf7cc237c",
            "title" : "FedRAMP Moderate Baseline",
            "rlinks" : 
            [ 
              { "href" : "https:\/\/raw.githubusercontent.com\/usnistgov\/OSCAL\/v1.0.0-milestone3\/content\/fedramp.gov\/xml\/FedRAMP_MODERATE-baseline_profile.xml",
                "media-type" : "application\/xml" } ],
            "remarks" : "Pointer to Moderate baseline content in OSCAL." },
          
          { "uuid" : "2acaf846-5496-4d36-8565-9a15b48aef2c",
            "title" : "FedRAMP Low Baseline",
            "rlinks" : 
            [ 
              { "href" : "https:\/\/raw.githubusercontent.com\/usnistgov\/OSCAL\/v1.0.0-milestone3\/content\/fedramp.gov\/xml\/FedRAMP_LOW-baseline_profile.xml",
                "media-type" : "application\/xml" } ],
            "remarks" : "Pointer to Low baseline content in OSCAL." } ] } } }
