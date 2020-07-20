**Patient with Medicare Number and Patient Test Identifier Open Slice** *[[Draft](http://hl7.org/fhir/r4/valueset-publication-status.html)]*

Prototype derived profile uses open slice to allow maximum of one Medicare Number and maximum of one Patient Test Identifier. Patient Test Identifier is intended to demonstrate an identifier with a data type profile that is not present in AU Base and has been added in the derived profile e.g. could be local to a specific implementation only.

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
        <td><a href="Patient-test-example-patient-identifier-value-only-s.html">Patient with only identifier.value</a></td>
        <td>test-example-patient-identifier-value-only-s</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-identifier-s.html">Patient with identifier.value and system (uuid)</a></td>
        <td>test-example-patient-identifier-s</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-s.html">Patient with IHI</a></td>
        <td>test-example-patient-ihi-s</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-s.html">Patient with a valid IHI and a non-valid IHI and Medicare Number</a></td>
        <td>test-example-patient-ihi-medicare-s</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-s.html">Patient with IHI and Medicare Number and DVA number</a></td>
        <td>test-example-patient-ihi-medicare-dva-s</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
     <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-mr-s.html">Patient with IHI and Medicare Number and DVA number and MRN</a></td>
        <td>test-example-patient-ihi-medicare-dva-mr-s</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-local-identifiers-s.html">Patient with HPI-O scoped MRN and Local namespace MRN</a></td>
        <td>test-example-patient-local-identifiers-s</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-s.html">Patient with Medicare Number and a valid Patient Test Identifier</a></td>
        <td>test-example-patient-medicare-testident-s</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-testident-s.html">Patient with valid Patient Test Identifier</a></td>
        <td>test-example-patient-testident-s</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-s.html">Patient with Medicare Number</a></td>
        <td>test-example-patient-medicare-s</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-mult-medicare-testident-s.html">Patient with two Medicare Number and two valid Patient Test Identifiers</a></td>
        <td>test-example-patient-mult-medicare-testident-s</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-invalid-testident-s.html">Patient with a valid Medicare Number and a non-valid Patient Test Identifier with Identifier.system only</a></td>
        <td>test-example-patient-medicare-invalid-testident-s</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-dva-s.html">Patient with Medicare Number, Patient Test Identifier and DVA number</a></td>
        <td>test-example-patient-medicare-testident-dva-s</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
     </tbody>
</table>