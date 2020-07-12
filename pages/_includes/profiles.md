# {{ page.title }}

These Profiles have been defined for this implementation guide.

## Administration Profiles
* [AU Base Patient](StructureDefinition-au-patient.html) - patient demographic with local identifiers and attributes 
* [AU Base Practitioner](StructureDefinition-au-practitioner.html) - individual practitioner with local identifiers and attributes
* [AU Base Practitioner Role](StructureDefinition-au-practitionerrole.html) - location based practitioner provider in a role
* [AU Base Organisation](StructureDefinition-au-organization.html) - responsible legal organisation
* [AU Base Healthcare Service](StructureDefinition-au-healthcareservice.html) - service delivery entity provided by an organisation
* [AU Base Location](StructureDefinition-au-location.html) - location with local identifiers
* [AU Base Related Person](StructureDefinition-au-relatedperson.html) - a related person with local identifiers
* [AU Base Encounter](StructureDefinition-au-encounter.html) - encounter with extensions

## Medications Profiles
* [AU Base Medication](StructureDefinition-au-medication.html) - medication details with common local coding and content
* [AU Base Medication Request](StructureDefinition-au-medicationrequest.html) - prescribing/ordering details with common local coding and content
* [AU Base Medication Dispense](StructureDefinition-au-medicationdispense.html) - dispensing details with common local coding and content
* [AU Base Medication Statement](StructureDefinition-au-medicationstatement.html) - medication history common local coding and content
* [AU Base Medication Administration](StructureDefinition-au-medicationadministration.html) - medication administration record with common local coding and content
* [AU Base Immunisation](StructureDefinition-au-immunization.html) - immunisation record with common local coding 
* [AU Medicine List](StructureDefinition-au-medlist.html) - medicine list with core localisation concepts

## Orders and Observations Profiles
* [AU Assertion of No Relevant Finding](StructureDefinition-au-norelevantfinding.html) - observation with assertion of no relevant finding
* [AU Base Body Structure](StructureDefinition-au-bodystructure.html) - body structure with local coding 
* [AU Base Diagnostic Report](StructureDefinition-au-diagnosticreport.html) - diagnostic report with localisation concepts
* [AU Base Specimen](StructureDefinition-au-specimen.html) - specimen details with local coding
* [AU Diagnostic Observation](StructureDefinition-au-diagnostic-observation.html) - observation for diagnostic reporting
* [AU Diagnostic Service Request](StructureDefinition-au-diagnostic-servicerequest.html) - diagnostic service request with localisation concepts

## Clinical Profiles
* [AU Base Condition](StructureDefinition-au-condition.html) - condition with local coding for clinical condition, body site and clinical finding.
* [AU Base Allergy Intolerance](StructureDefinition-au-allergyintolerance.html) - allergy intolerance with local coding

## Composition Profiles
* [AU Base Composition](StructureDefinition-au-composition.html) - composition pattern aligned with local CDA requirements

## Profiles on Data Types 
* [AU Base Address](StructureDefinition-au-address.html) - well defined representation of an Australian address
* [AU Base Dosage](StructureDefinition-au-dosage.html) - dosage information with common local coding

### Profiles on Identifier Data Type
* [AU IHI Number](StructureDefinition-au-ihinumber.html) - identifier profile for an Australian Individual Healthcare Identifier
* [AU Medicare Card Number](StructureDefinition-au-medicarecardnumber.html) - identifier profile for an Australian Medicare card number
* [AU Medical Record Number](StructureDefinition-au-medicalrecordnumber.html) - identifier profile for an Australian medical record number
* [AU DVA Number](StructureDefinition-au-dvanumber.html) - identifier profile for an Australian Department of Veterans' Affairs (DVA) Number
* [AU HPI-O Number](StructureDefinition-au-hpionumber.html) - identifier profile for an Australian Healthcare Provider Identifier – Organisation
* [AU HPI-I Number](StructureDefinition-au-hpiinumber.html) - identifier profile for a Healthcare Provider Identifier - Individual - HPI-I
* [AU ABN Number](StructureDefinition-au-abnnumber.html) - identifier profile for an Australian Business Number - ABN

## Prototype profiles to help define the mechanism for reference / inclusion of Identifier data type profiles 
See ([au-fhir-base/issues/429](https://github.com/hl7au/au-fhir-base/issues/429))

#### Guidance only
Demonstrates inclusion of Identifier data type profiles by guidance only - no direct reference in an AU Base StructureDefinition. Demonstrates some basic derived profiles using this option with simple identifier constraints.
* [AU Base Patient with Guidance only](StructureDefinition-au-patient-without-local-ident.html)
  * [Patient with Mandatory Identifier](StructureDefinition-patient-without-local-ident-ident.html)
  * [Patient with Mandatory IHI](StructureDefinition-patient-without-local-ident-ihi.html)
  * [Patient with IHI and Medicare Number](StructureDefinition-patient-without-local-ident-ihi-med.html) - derived profile uses open slice to allow max one IHI, max one Medicare Number, and any other identifiers

#### Allowed types
Demonstrates inclusion of Identifier data type profiles by adding as a set of allowed types on the identifier element (in addition to the base Identifier type). Demonstrates some basic derived profiles using this option with simple identifier constraints.
* [AU Base Patient with Allowed types](StructureDefinition-au-patient-ident-choice.html)
  * [Patient with Mandatory Identifier](StructureDefinition-patient-ident-choice-ident.html)
  * [Patient with Mandatory IHI](StructureDefinition-patient-ident-choice-ihi.html) 
  * [Patient with IHI and Medicare Number](StructureDefinition-patient-ident-choice-ihi-med.html) - derived profile uses open slice to allow max one IHI and max one Medicare Number, and any other identifiers
  * [Patient with IHI and Medicare Number Closed Slice](StructureDefinition-patient-ident-choice-ihi-med-closedslice.html) - derived profile uses closed slice to allow only max two identifiers; a single IHI and a single Medicare Number
  * [Patient with IHI and Medicare Number Closed Type](StructureDefinition-patient-ident-choice-ihi-med-closedtype.html) - derived profile uses allowed types to only allow IHIs and Medicare Numbers

#### Slices
Demonstrates inclusion of Identifier data type profiles by slicing on the identifier element and defining a slice for each identifier we decide is relevant to the base resource profile. Demonstrates some basic derived profiles using this option with simple identifier constraints.
* [AU Base Patient with Slices](StructureDefinition-au-patient-ident-slice.html) 
  * [Patient with Mandatory Identifier](StructureDefinition-patient-ident-slice-ident.html) 
  * [Patient with Mandatory IHI](StructureDefinition-patient-ident-slice-ihi.html) 
  * [Patient with IHI and Medicare Number](StructureDefinition-patient-ident-slice-ihi-med.html) 

