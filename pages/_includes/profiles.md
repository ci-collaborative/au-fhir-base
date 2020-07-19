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
* [AU PAI-O Identifier](StructureDefinition-au-paioidentifier.html) - identifier profile for a My Health Record Assigned Identity - Organisation (PAI-O)
* [AU ABN Number](StructureDefinition-au-abnnumber.html) - identifier profile for an Australian Business Number - ABN
* [AU NATA Accreditation Number](StructureDefinition-au-nataaccreditationnumber.html) - identifier profile for a National Association of Testing Authorities (NATA) accreditation number
* [AU NATA Site Number](StructureDefinition-au-natasitenumber.html) - identifier profile for a National Association of Testing Authorities (NATA) site number
* [AU AHPRA Registration Number](StructureDefinition-au-ahpraregistrationnumber.html) - identifier profile for an Australian Health Practitioner Regulation Agency (AHPRA) Registration Number
* [AU Employee Number](StructureDefinition-au-employeenumber.html) - identifier profile for an employee number

## Prototype profiles to help define the mechanism for reference / inclusion of Identifier data type profiles 
See ([au-fhir-base/issues/429](https://github.com/hl7au/au-fhir-base/issues/429))

#### Guidance only
Demonstrates inclusion of Identifier data type profiles by guidance only - no direct reference in an AU Base StructureDefinition. Demonstrates some basic derived profiles using this option with simple identifier constraints.

<table class="list" style="width:100%">
    <colgroup>
       <col span="1" style="width: 25%;"/>
       <col span="1" style="width: 25%;"/>
       <col span="1" style="width: 50%;"/>
    </colgroup>
	<tbody>
      <tr>
        <th>AU Base Profile</th>
        <th>Derived Profile</th>
        <th>Description</th>
      </tr>
      <tr>
        <td rowspan="5"><a href="StructureDefinition-au-patient-guidance.html">AU Base Patient with Guidance only</a></td>
        <td><a href="StructureDefinition-patient-guidance-ident.html">Patient with Mandatory Identifier</a></td>
        <td>Derived profile uses cardinality to enforce at least one identifier</td>
      </tr>
      <tr>
        <td><a href="StructureDefinition-patient-guidance-ihi.html">Patient with Mandatory IHI</a></td>
        <td>Derived profile uses open slice to mandate one and only one IHI</td>
      </tr>
      <tr>
        <td><a href="StructureDefinition-patient-guidance-ihi-med.html">Patient with IHI and Medicare Number</a></td>
        <td>Derived profile uses open slice to allow max one IHI, max one Medicare Number, and any other identifiers</td>
      </tr>
      <tr>
        <td><a href="StructureDefinition-patient-guidance-ihi-med-closedslice.html">Patient with IHI and Medicare Number Closed Slice</a></td>
        <td>Derived profile uses closed slice to allow only max two identifiers; a single IHI and a single Medicare Number</td>
      </tr>
      <tr>
        <td><a href="StructureDefinition-patient-guidance-ihi-med-closedtype.html">Patient with IHI and Medicare Number Closed Type</a></td>
        <td>Derived profile uses allowed types to only allow IHIs and Medicare Numbers</td>
      </tr>
    </tbody>
</table>

#### Allowed types
Demonstrates inclusion of Identifier data type profiles by adding as a set of allowed types on the identifier element (in addition to the base Identifier type). Demonstrates some basic derived profiles using this option with simple identifier constraints.

<table class="list" style="width:100%">
    <colgroup>
       <col span="1" style="width: 25%;"/>
       <col span="1" style="width: 25%;"/>
       <col span="1" style="width: 50%;"/>
    </colgroup>
	<tbody>
      <tr>
        <th>AU Base Profile</th>
        <th>Derived Profile</th>
        <th>Description</th>
      </tr>
      <tr>
        <td rowspan="7"><a href="StructureDefinition-au-patient-ident-choice.html">AU Base Patient with Allowed types</a></td>
        <td><a href="StructureDefinition-patient-ident-choice-ident.html">Patient with Mandatory Identifier</a></td>
        <td>Derived profile uses cardinality to enforce at least one identifier</td>
      </tr>
      <tr>
        <td><a href="StructureDefinition-patient-ident-choice-ihi.html">Patient with Mandatory IHI</a></td>
        <td>Derived profile uses open slice to mandate one and only one IHI</td>
      </tr>
      <tr>
        <td><a href="StructureDefinition-patient-ident-choice-ihi-med.html">Patient with IHI and Medicare Number</a></td>
        <td>Derived profile uses open slice to allow max one IHI, max one Medicare Number, and any other identifiers</td>
      </tr>
      <tr>
        <td><a href="StructureDefinition-patient-ident-choice-ihi-med-closedslice.html">Patient with IHI and Medicare Number Closed Slice</a></td>
        <td>Derived profile uses closed slice to allow only max two identifiers; a single IHI and a single Medicare Number</td>
      </tr>
      <tr>
        <td><a href="StructureDefinition-patient-ident-choice-ihi-med-closedtype.html">Patient with IHI and Medicare Number Closed Type</a></td>
        <td>Derived profile uses allowed types to only allow IHIs and Medicare Numbers</td>
      </tr>
      <tr>
        <td><a href="StructureDefinition-patient-ident-choice-med-testident.html">Patient with Medicare Number and Patient Test Identifier</a></td>
        <td>Derived profile uses open slice to allow max one Medicare Number and max one of a Patient Test Identifier</td>
      </tr>
      <tr>
        <td><a href="StructureDefinition-patient-ident-choice-med-testident-closedslice.html">Patient with Medicare Number and Patient Test Identifier Closed Slice</a></td>
        <td>Derived profile uses closed slice to allow max two identifiers: Medicare Number and and a single Patient Test Identifier</td>
      </tr>
    </tbody>
</table>

#### Slices
Demonstrates inclusion of Identifier data type profiles by slicing on the identifier element and defining a slice for each identifier we decide is relevant to the base resource profile. Demonstrates some basic derived profiles using this option with simple identifier constraints.

<table class="list" style="width:100%">
    <colgroup>
       <col span="1" style="width: 25%;"/>
       <col span="1" style="width: 25%;"/>
       <col span="1" style="width: 50%;"/>
    </colgroup>
	<tbody>
      <tr>
        <th>AU Base Profile</th>
        <th>Derived Profile</th>
        <th>Description</th>
      </tr>
      <tr>
        <td rowspan="7"><a href="StructureDefinition-au-patient-ident-slice.html">AU Base Patient with Slices</a></td>
        <td><a href="StructureDefinition-patient-ident-slice-ident.html">Patient with Mandatory Identifier</a></td>
        <td>Derived profile uses cardinality to enforce at least one identifier</td>
      </tr>
      <tr>
        <td><a href="StructureDefinition-patient-ident-slice-ihi.html">Patient with Mandatory IHI</a></td>
        <td>Derived profile uses open slice to mandate one and only one IHI</td>
      </tr>
      <tr>
        <td><a href="StructureDefinition-patient-ident-slice-ihi-med.html">Patient with IHI and Medicare Number</a></td>
        <td>Derived profile uses open slice to allow max one IHI, max one Medicare Number, and any other identifiers</td>
      </tr>
      <tr>
        <td><a href="StructureDefinition-patient-ident-slice-ihi-med-closedslice.html">Patient with IHI and Medicare Number Closed Slice</a></td>
        <td>Derived profile uses closed slice to allow only max two identifiers; a single IHI and a single Medicare Number</td>
      </tr>
      <tr>
        <td>Patient with IHI and Medicare Number Closed Type</td>
        <td>Not possible when deriving from a sliced profile?</td>
      </tr>
      <tr>
        <td><a href="StructureDefinition-patient-ident-slice-med-testident.html">Patient with Medicare Number and Patient Test Identifier</a></td>
        <td>Derived profile uses open slice to allow max one Medicare Number, and max one Patient Test Identifier</td>
      </tr>
      <tr>
        <td><a href="StructureDefinition-patient-ident-slice-med-testident-closedslice.html">Patient with Medicare Number and Patient Test Identifier Closed Slice</a></td>
        <td>Derived profile uses closed slice to allow max two identifiers: Medicare Number and and a single Patient Test Identifier</td>
      </tr>
    </tbody>
</table>


#### Identifier Data Type
[Patient Test Identifier](StructureDefinition-identifier-patient-test-ident.html) - Patient Test Identifier is intended to demonstrate an identifier with a data type profile that is not present in AU Base and has been added in the derived profile e.g. could be local to a specific implementation only.

