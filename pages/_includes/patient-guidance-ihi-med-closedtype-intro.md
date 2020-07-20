**Patient with IHI and Medicare Number Closed Type** *[[Draft](http://hl7.org/fhir/r4/valueset-publication-status.html)]*

Prototype derived profile uses allowed types to only allow IHIs and Medicare Numbers.

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
        <td><a href="Patient-test-example-patient-identifier-value-only-f.html">Patient with only identifier.value</a></td>
        <td>test-example-patient-identifier-value-only-f</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-identifier-f.html">Patient with identifier.value and system (uuid)</a></td>
        <td>test-example-patient-identifier-f</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-f.html">Patient with IHI</a></td>
        <td>test-example-patient-ihi-f</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-f.html">Patient with a valid IHI and a non-valid IHI and Medicare Number</a></td>
        <td>test-example-patient-ihi-medicare-f</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-f.html">Patient with IHI and Medicare Number and DVA number</a></td>
        <td>test-example-patient-ihi-medicare-dva-f</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-mr-f.html">Patient with IHI and Medicare Number and DVA number and MRN</a></td>
        <td>test-example-patient-ihi-medicare-dva-mr-f</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-local-identifiers-f.html">Patient with HPI-O scoped MRN and Local namespace MRN</a></td>
        <td>test-example-patient-local-identifiers-f</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-f.html">Patient with Medicare Number and a valid Patient Test Identifier</a></td>
        <td>test-example-patient-medicare-testident-f</td>
        <td>?</td>
        <td>?</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-testident-f.html">Patient with valid Patient Test Identifier</a></td>
        <td>test-example-patient-testident-f</td>
        <td>?</td>
        <td>?</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-f.html">Patient with Medicare Number</a></td>
        <td>test-example-patient-medicare-f</td>
        <td>?</td>
        <td>?</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-mult-medicare-testident-f.html">Patient with two Medicare Number and two valid Patient Test Identifiers</a></td>
        <td>test-example-patient-mult-medicare-testident-f</td>
        <td>?</td>
        <td>?</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-invalid-testident-f.html">Patient with a valid Medicare Number and a non-valid Patient Test Identifier with Identifier.system only</a></td>
        <td>test-example-patient-medicare-invalid-testident-f</td>
        <td>?</td>
        <td>?</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-dva-f.html">Patient with Medicare Number, Patient Test Identifier and DVA number</a></td>
        <td>test-example-patient-medicare-testident-dva-f</td>
        <td>?</td>
        <td>?</td>
        <td>-</td>
      </tr>
    </tbody>
</table>

