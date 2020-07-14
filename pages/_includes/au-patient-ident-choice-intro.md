**AU Base Patient Profile** *[[FMM Level 3](guidance.html)]*

_Prototype demonstrates inclusion of Identifier data type profiles by adding as a set of allowed types on the identifier element (in addition to the base Identifier type). See [au-fhir-base/issues/429](https://github.com/hl7au/au-fhir-base/issues/429)._

This profile defines a patient administration details structure that includes core localisation concepts for use in an Australian context.

#### Identifiers
These definitions (Identifier profiles) represent common data held in the Patient.identifier element:
* [Individual Healthcare Identifier - IHI](StructureDefinition-au-ihinumber.html) [<sup>[1]</sup>](http://ns.electronichealth.net.au/id/hi/ihi/1.0/index.html){:target="_blank"} [<sup>[2]</sup>](http://meteor.aihw.gov.au/content/index.phtml/itemId/432495){:target="_blank"}
* [Medicare Number](StructureDefinition-au-medicarecardnumber.html) [<sup>[1]</sup>](http://ns.electronichealth.net.au/id/medicare-number/index.html){:target="_blank"} [<sup>[2]</sup>](http://meteor.aihw.gov.au/content/index.phtml/itemId/270101){:target="_blank"}
* [DVA (Department of Veterans' Affairs) Number](StructureDefinition-au-dvanumber.html) [<sup>[1]</sup>](http://ns.electronichealth.net.au/id/dva/index.html){:target="_blank"} [<sup>[2]</sup>](http://meteor.aihw.gov.au/content/index.phtml/itemId/339127){:target="_blank"}
* [Health Care Card Number](StructureDefinition-au-tbd.html), [Pensioner Concession Card Number](StructureDefinition-au-tbd.html), [Commonwealth Seniors Health Card Number](StructureDefinition-au-tbd.html) [<sup>[1]</sup>](http://ns.electronichealth.net.au/id/centrelink-customer-reference-number/index.html){:target="_blank"} [<sup>[2]</sup>](http://meteor.aihw.gov.au/content/index.phtml/itemId/270098){:target="_blank"}
* [Medical Record Number](StructureDefinition-au-medicalrecordnumber.html) - ABN scoped[<sup>[1]</sup>](http://ns.electronichealth.net.au/id/abn-scoped/medicalrecord/1.0/index.html){:target="_blank"}, HPI-O scoped[<sup>[2]</sup>](http://ns.electronichealth.net.au/id/hpio-scoped/medicalrecord/1.0/index.html){:target="_blank"}
* [Private Health Insurance Member Number](StructureDefinition-au-tbd.html)

#### Extensions
Extensions used in this profile:
* Patient: [Indigenous Status](http://hl7.org.au/fhir/StructureDefinition/indigenous-status) [<sup>[1]</sup>](http://meteor.aihw.gov.au/content/index.phtml/itemId/602543){:target="_blank"}
* Patient: [Closing the Gap registration](http://hl7.org.au/fhir/StructureDefinition/closing-the-gap-registration) [<sup>[1]</sup>](http://meteor.aihw.gov.au/content/index.phtml/itemId/603679){:target="_blank"}
* Patient: [Birth Place](http://hl7.org/fhir/StructureDefinition/birthPlace) (Core Extension)
* Patient: [Mother's Maiden Name](http://hl7.org/fhir/StructureDefinition/patient-mothersMaidenName) (Core Extension)
* Patient: [interpreterRequired](http://hl7.org/fhir/StructureDefinition/patient-interpreterRequired) (Core Extension)
* Patient: [Date of Arrival in Australia](http://hl7.org.au/fhir/StructureDefinition/date-of-arrival) [<sup>[1]</sup>](https://www.abs.gov.au/AUSSTATS/abs@.nsf/Lookup/1200.0.55.007Main+Features12014,%20Version%201.5?OpenDocument){:target="_blank"} [<sup>[3]</sup>](https://meteor.aihw.gov.au/content/index.phtml/itemId/269447){:target="_blank"}
* Patient.birthDate: [Birth Time](http://hl7.org/fhir/STU3/extension-patient-birthtime.html) (Core Extension)
* Patient.birthDate, Patient.deceasedDateTime: [Date Accuracy Indicator](http://hl7.org.au/fhir/StructureDefinition/date-accuracy-indicator.html)

#### Usage Notes
Mutiple Individual Healthcare Identifiers are supported particularly to support the recording of IHI values where the status and/or record status varies (e.g. deceased, provisional).

Medicare Number is defined as a 10 or 11 digit number. Whilst 10 digits is not sufficient to uniquely identify an individual it is a supported entry where systems do not support 11 digit content. If required profiles can constrain this slice further to restrict usage to 11 digits only as desired.
Medicare Numbers are not used for uniquely identifying patients, they are identifying information that can be used in conjunction with other elements such as name and date of birth appropriately to confirm identity.

To indicate an interpreter service is required, extension interpreter required=true should be set. If the language for interpreter service is known then it should be included in communication.language with communication.preferred=true. If communication.preferred=true is not set when interpreter required=true then it may be understood that an interpreter is required but the language for the interpreter service is not known.

#### Test Examples

<table class="list" style="width:100%">
    <colgroup>
       <col span="1" style="width: 19%;"/>
       <col span="1" style="width: 25%;"/>
       <col span="1" style="width: 10%;"/>
       <col span="1" style="width: 10%;"/>
       <col span="1" style="width: 20%;"/>
    </colgroup>
	<tbody>
      <tr>
        <th>Test scenario</th>
        <th>resource id</th>
        <th>Expected</th>
        <th>Actual</th>
		<th>Notes</th>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-identifier-value-only-g.html">Patient with only identifier.value</a></td>
        <td>test-example-patient-identifier-value-only-g</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-identifier-g.html">Patient with identifier.value and system (uuid)</a></td>
        <td>test-example-patient-identifier-g</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-g.html">Patient with IHI</a></td>
        <td>test-example-patient-ihi-g</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-g.html">Patient with a valid IHI and a non-valid IHI and Medicare Number</a></td>
        <td>test-example-patient-ihi-medicare-g</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-g.html">Patient with IHI and Medicare Number and DVA number</a></td>
        <td>test-example-patient-ihi-medicare-dva-g</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-mr-g.html">Patient with IHI and Medicare Number and DVA number and MRN</a></td>
        <td>test-example-patient-ihi-medicare-dva-mr-g</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-local-identifiers-g.html">Patient with HPI-O scoped MRN and Local namespace MRN</a></td>
        <td>test-example-patient-local-identifiers-g</td>
         <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
    </tbody>
</table>