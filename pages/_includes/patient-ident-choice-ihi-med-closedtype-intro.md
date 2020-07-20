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
        <td><a href="Patient-test-example-patient-identifier-value-only-l.html">Patient with only identifier.value</a></td>
        <td>test-example-patient-identifier-value-only-l</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-identifier-l.html">Patient with identifier.value and system (uuid)</a></td>
        <td>test-example-patient-identifier-l</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-l.html">Patient with IHI</a></td>
        <td>test-example-patient-ihi-l</td>
        <td>Pass</td>
        <td>Pass</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-l.html">Patient with a valid IHI and a non-valid IHI and Medicare Number</a></td>
        <td>test-example-patient-ihi-medicare-l</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-l.html">Patient with IHI and Medicare Number and DVA number</a></td>
        <td>test-example-patient-ihi-medicare-dva-l</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-mr-l.html">Patient with IHI and Medicare Number and DVA number and MRN</a></td>
        <td>test-example-patient-ihi-medicare-dva-mr-l</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-local-identifiers-l.html">Patient with HPI-O scoped MRN and Local namespace MRN</a></td>
        <td>test-example-patient-local-identifiers-l</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-l.html">Patient with Medicare Number and a valid Patient Test Identifier</a></td>
        <td>test-example-patient-medicare-testident-l</td>
        <td>?</td>
        <td>?</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-testident-l.html">Patient with valid Patient Test Identifier</a></td>
        <td>test-example-patient-testident-l</td>
        <td>?</td>
        <td>?</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-l.html">Patient with Medicare Number</a></td>
        <td>test-example-patient-medicare-l</td>
        <td>?</td>
        <td>?</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-mult-medicare-testident-l.html">Patient with two Medicare Number and two valid Patient Test Identifiers</a></td>
        <td>test-example-patient-mult-medicare-testident-l</td>
        <td>?</td>
        <td>?</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-invalid-testident-l.html">Patient with a valid Medicare Number and a non-valid Patient Test Identifier with Identifier.system only</a></td>
        <td>test-example-patient-medicare-invalid-testident-l</td>
        <td>?</td>
        <td>?</td>
        <td>-</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-dva-l.html">Patient with Medicare Number, Patient Test Identifier and DVA number</a></td>
        <td>test-example-patient-medicare-testident-dva-l</td>
        <td>?</td>
        <td>?</td>
        <td>-</td>
      </tr>
    </tbody>
</table>


