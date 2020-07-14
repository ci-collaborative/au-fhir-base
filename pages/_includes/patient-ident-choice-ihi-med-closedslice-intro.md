**Patient with IHI and Medicare Number Closed Slice** *[[Draft](http://hl7.org/fhir/r4/valueset-publication-status.html)]*

Prototype derived profile uses closed slice to allow only max two identifiers; a single IHI and a single Medicare Number.

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
        <td><a href="Patient-test-example-patient-identifier-value-only-k.html">Patient with only identifier.value</a></td>
        <td>test-example-patient-identifier-value-only-k</td>
        <td>x</td>
        <td>x</td>
        <td>x</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-identifier-k.html">Patient with identifier.value and system (uuid)</a></td>
        <td>test-example-patient-identifier-k</td>
        <td>x</td>
        <td>x</td>
        <td>x</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-k.html">Patient with IHI</a></td>
        <td>test-example-patient-ihi-k</td>
        <td>x</td>
        <td>x</td>
        <td>x</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-k.html">Patient with a valid IHI and a non-valid IHI and Medicare Number</a></td>
        <td>test-example-patient-ihi-medicare-k</td>
        <td>x</td>
        <td>x</td>
        <td>x</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-k.html">Patient with IHI and Medicare Number and DVA number</a></td>
        <td>test-example-patient-ihi-medicare-dva-k</td>
        <td>x</td>
        <td>x</td>
        <td>x</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-mr-k.html">Patient with IHI and Medicare Number and DVA number and MRN</a></td>
        <td>test-example-patient-ihi-medicare-dva-mr-k</td>
        <td>x</td>
        <td>x</td>
        <td>x</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-local-identifiers-k.html">Patient with HPI-O scoped MRN and Local namespace MRN</a></td>
        <td>test-example-patient-local-identifiers-k</td>
        <td>x</td>
        <td>x</td>
        <td>x</td>
      </tr>
    </tbody>
</table>

