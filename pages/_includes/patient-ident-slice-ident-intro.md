**Patient with Mandatory Identifier** *[[Draft](http://hl7.org/fhir/r4/valueset-publication-status.html)]*

Prototype derived profile uses uses cardinality to enforce at least one identifier.

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
        <td><a href="Patient-test-example-patient-identifier-value-only-n.html">Patient with only identifier.value</a></td>
        <td>test-example-patient-identifier-value-only-n</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-ident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-ihinumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-identifier-n.html">Patient with identifier.value and system (uuid)</a></td>
        <td>test-example-patient-identifier-n</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-ident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-ihinumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-n.html">Patient with IHI</a></td>
        <td>test-example-patient-ihi-n</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-ident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-ihinumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-n.html">Patient with a valid IHI and a non-valid IHI and Medicare Number</a></td>
        <td>test-example-patient-ihi-medicare-n</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-ident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-ihinumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-n.html">Patient with IHI and Medicare Number and DVA number</a></td>
        <td>test-example-patient-ihi-medicare-dva-n</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-ident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-ihinumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-mr-n.html">Patient with IHI and Medicare Number and DVA number and MRN</a></td>
        <td>test-example-patient-ihi-medicare-dva-mr-n</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-ident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-ihinumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-local-identifiers-n.html">Patient with HPI-O scoped MRN and Local namespace MRN</a></td>
        <td>test-example-patient-local-identifiers-n</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-ident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-ihinumber')): Not supported yet</td>
      </tr>
    </tbody>
</table>
