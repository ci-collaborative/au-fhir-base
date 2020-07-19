**Patient with Medicare Number and Patient Test Identifier Closed Slice** *[[Draft](http://hl7.org/fhir/r4/valueset-publication-status.html)]*

Prototype derived profile uses open closed slice to allow maximum of two identifiers, one Medicare Numvber and one Patient Test Identifier. Patient Test Identifier is intended to demonstrate an identifier with a data type profile that is not present in AU Base and has been added in the derived profile e.g. could be local to a specific implementation only.

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
        <td><a href="Patient-test-example-patient-identifier-value-only-u.html">Patient with only identifier.value</a></td>
        <td>test-example-patient-identifier-value-only-u</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-identifier-u.html">Patient with identifier.value and system (uuid)</a></td>
        <td>test-example-patient-identifier-u</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-u.html">Patient with IHI</a></td>
        <td>test-example-patient-ihi-u</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-u.html">Patient with a valid IHI and a non-valid IHI and Medicare Number</a></td>
        <td>test-example-patient-ihi-medicare-u</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-u.html">Patient with IHI and Medicare Number and DVA number</a></td>
        <td>test-example-patient-ihi-medicare-dva-u</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-mr-u.html">Patient with IHI and Medicare Number and DVA number and MRN</a></td>
        <td>test-example-patient-ihi-medicare-dva-mr-u</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-local-identifiers-u.html">Patient with HPI-O scoped MRN and Local namespace MRN</a></td>
        <td>test-example-patient-local-identifiers-u</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-u.html">Patient with Medicare Number and a valid Patient Test Identifier</a></td>
        <td>test-example-patient-medicare-testident-u</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-testident-u.html">Patient with valid Patient Test Identifier</a></td>
        <td>test-example-patient-testident-u</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-u.html">Patient with Medicare Number</a></td>
        <td>test-example-patient-medicare-u</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-mult-medicare-testident-u.html">Patient with two Medicare Number and two valid Patient Test Identifiers</a></td>
        <td>test-example-patient-mult-medicare-testident-u</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-invalid-testident-u.html">Patient with a valid Medicare Number and a non-valid Patient Test Identifier with Identifier.system only</a></td>
        <td>test-example-patient-medicare-invalid-testident-u</td>test-example-patient-medicare-invalid-testident-u
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-dva-u.html">Patient with Medicare Number, Patient Test Identifier and DVA number</a></td>
        <td>test-example-patient-medicare-testident-dva-u</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
     </tbody>
</table>