**Patient with Medicare Number and a Locally Defined Identifier Type** *[[Draft](http://hl7.org/fhir/r4/valueset-publication-status.html)]*

Prototype derived profile uses open slice to allow maximum of one Medicare Numvber and maximum of one locally defined Identifier types (not defined in AU Base).

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
        <td><a href="Patient-test-example-patient-medicare-testident-aa.html">Patient with Medicare Number and a valid locally defined identifier</a></td>
        <td>test-example-patient-medicare-testident-aa</td>
        <td>Pass</td>
        <td>Pass</td>
        <td></td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-ab.html">Patient with valid locally defined identifier</a></td>
        <td>test-example-patient-medicare-testident-ab</td>
        <td>Pass</td>
        <td>Pass</td>
        <td></td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-ac.html">Patient with Medicare Number</a></td>
        <td>test-example-patient-medicare-testident-ac</td>
        <td>Pass</td>
        <td>Pass</td>
        <td></td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-ad.html">Patient with two Medicare Number and two valid locally defined identifiers</a></td>
        <td>test-example-patient-medicare-testident-ad</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>Profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-choice-ihi-testident, Element 'Patient.identifier[medicareNumber]': max allowed = 1, but found 2</br>	Profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-choice-ihi-testident, Element 'Patient.identifier[testIdentifier]': max allowed = 1, but found 2</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-ag.html">Patient with a valid Medicare Number and a non-valid locally defined identifier with Identifier.system only</a></td>
        <td>test-example-patient-medicare-testident-ag</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>Profile http://hl7.org.au/fhir/StructureDefinition/identifier-patient-test-ident, Element 'Patient.identifier[1].value': minimum required = 1, but only found 0</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-dva-ah.html">Patient with Medicare Number, locally defined identifier and DVA number</a></td>
        <td>test-example-patient-medicare-testident-dva-ah</td>
        <td>Pass</td>
        <td>Pass</td>
        <td></td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-dva-ai.html">Patient with DVA number only; with no Medicare Number and no locally defined identifier</a></td>
        <td>test-example-patient-medicare-testident-dva-ai</td>
        <td>Pass</td>
        <td>Pass</td>
        <td></td>
      </tr>
     </tbody>
</table>