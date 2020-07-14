**Patient with Medicare Number and a Locally Defined Identifier Type Closed Slice ** *[[Draft](http://hl7.org/fhir/r4/valueset-publication-status.html)]*

Prototype derived profile uses open closed slice to allow maximum of one Medicare Numvber and maximum of one locally defined Identifier types (not defined in AU Base).

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
        <td><a href="Patient-test-example-patient-medicare-testident-ax.html">Patient with Medicare Number and a valid locally defined identifier</a></td>
        <td>test-example-patient-medicare-testident-ax</td>
        <td>Pass</td>
        <td>Pass</td>
        <td></td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-ay.html">Patient with valid locally defined identifier</a></td>
        <td>test-example-patient-medicare-testident-ay</td>
        <td>Pass</td>
        <td></td>
        <td></td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-az.html">Patient with Medicare Number</a></td>
        <td>test-example-patient-medicare-testident-az</td>
        <td>Pass</td>
        <td></td>
        <td></td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-ba.html">Patient with two Medicare Number and two valid locally defined identifiers</a></td>
        <td>test-example-patient-medicare-testident-ba</td>
        <td>Fail</td>
        <td></td>
        <td></td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-bb.html">Patient with a valid Medicare Number and a non-valid locally defined identifier with Identifier.system only</a></td>
        <td>test-example-patient-medicare-testident-bb</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>Profile http://hl7.org.au/fhir/StructureDefinition/identifier-patient-test-ident, Element 'Patient.identifier[1].value': minimum required = 1, but only found 0</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-dva-bc.html">Patient with Medicare Number, locally defined identifier and DVA number</a></td>
        <td>test-example-patient-medicare-testident-dva-bc</td>
        <td>Pass</td>
        <td></td>
        <td></td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-dva-bd.html">Patient with DVA number only; with no Medicare Number and no locally defined identifier</a></td>
        <td>test-example-patient-medicare-testident-dva-bd</td>
        <td>Pass</td>
        <td></td>
        <td></td>
      </tr>
     </tbody>
</table>