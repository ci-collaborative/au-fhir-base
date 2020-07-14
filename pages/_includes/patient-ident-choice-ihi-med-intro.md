**Patient with IHI and Medicare Number** *[[Draft](http://hl7.org/fhir/r4/valueset-publication-status.html)]*

Prototype derived profile uses open slice to allow max one IHI, max one Medicare Number, and any other identifiers.

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
        <td><a href="Patient-test-example-patient-identifier-value-only-j.html">Patient with only identifier.value</a></td>
        <td>test-example-patient-identifier-value-only-j</td>
        <td>x</td>
        <td>x</td>
        <td>x</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-identifier-j.html">Patient with identifier.value and system (uuid)</a></td>
        <td>test-example-patient-identifier-j</td>
        <td>x</td>
        <td>x</td>
        <td>x</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-j.html">Patient with IHI</a></td>
        <td>test-example-patient-ihi-j</td>
        <td>x</td>
        <td>x</td>
        <td>x</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-j.html">Patient with a valid IHI and a non-valid IHI and Medicare Number</a></td>
        <td>test-example-patient-ihi-medicare-j</td>
        <td>x</td>
        <td>x</td>
        <td>x</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-j.html">Patient with IHI and Medicare Number and DVA number</a></td>
        <td>test-example-patient-ihi-medicare-dva-j</td>
        <td>x</td>
        <td>x</td>
        <td>x</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-mr-j.html">Patient with IHI and Medicare Number and DVA number and MRN</a></td>
        <td>test-example-patient-ihi-medicare-dva-mr-j</td>
        <td>x</td>
        <td>x</td>
        <td>x</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-local-identifiers-j.html">Patient with HPI-O scoped MRN and Local namespace MRN</a></td>
        <td>test-example-patient-local-identifiers-j</td>
        <td>x</td>
        <td>x</td>
        <td>x</td>
      </tr>
    </tbody>
</table>