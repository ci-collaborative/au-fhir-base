**Patient with Medicare Number and Patient Test Identifier** *[[Draft](http://hl7.org/fhir/r4/valueset-publication-status.html)]*

Prototype derived profile uses open slice to allow maximum of one Medicare Numvber and maximum of one Patient Test Identifier. Patient Test Identifier is intended to demonstrate an identifier with a data type profile that is not present in AU Base and has been added in the derived profile e.g. could be local to a specific implementation only.

#### Test Examples

<table class="list" style="width:100%">
    <colgroup>
       <col span="1" style="width: 24%;"/>
       <col span="1" style="width: 25%;"/>
       <col span="1" style="width: 10%;"/>
       <col span="1" style="width: 10%;"/>
       <col span="1" style="width: 15%;"/>
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
        <td><a href="Patient-test-example-patient-identifier-value-only-t.html">Patient with only identifier.value</a></td>
        <td>test-example-patient-identifier-value-only-t</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-identifier-t.html">Patient with identifier.value and system (uuid)</a></td>
        <td>test-example-patient-identifier-t</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-t.html">Patient with IHI</a></td>
        <td>test-example-patient-ihi-t</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-t.html">Patient with a valid IHI and a non-valid IHI and Medicare Number</a></td>
        <td>test-example-patient-ihi-medicare-t</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>NOTE that when inheriting with profile, an 'invalid' IHI just reads as 'some other identifier type' so this won't fail an invalid IHI.</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-t.html">Patient with IHI and Medicare Number and DVA number</a></td>
        <td>test-example-patient-ihi-medicare-dva-t</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
     <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-mr-t.html">Patient with IHI and Medicare Number and DVA number and MRN</a></td>
        <td>test-example-patient-ihi-medicare-dva-mr-t</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-local-identifiers-t.html">Patient with HPI-O scoped MRN and Local namespace MRN</a></td>
        <td>test-example-patient-local-identifiers-t</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-t.html">Patient with Medicare Number and a valid Patient Test Identifier</a></td>
        <td>test-example-patient-medicare-testident-t</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-testident-t.html">Patient with valid Patient Test Identifier</a></td>
        <td>test-example-patient-testident-t</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-t.html">Patient with Medicare Number</a></td>
        <td>test-example-patient-medicare-t</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-mult-medicare-testident-t.html">Patient with two Medicare Number and two valid Patient Test Identifiers</a></td>
        <td>test-example-patient-mult-medicare-testident-t</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-invalid-testident-t.html">Patient with a valid Medicare Number and a non-valid Patient Test Identifier with Identifier.system only</a></td>
        <td>test-example-patient-medicare-invalid-testident-t</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>NOTE that when inheriting with profile, an 'invalid' Patient Test Identifier just reads as 'some other identifier type' due to how the data type profile is defined.</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-dva-t.html">Patient with Medicare Number, Patient Test Identifier and DVA number</a></td>
        <td>test-example-patient-medicare-testident-dva-t</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
     </tbody>
</table>