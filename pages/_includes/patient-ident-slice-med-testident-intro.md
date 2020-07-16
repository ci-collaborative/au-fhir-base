**Patient with Medicare Number and a Locally Defined Identifier** *[[Draft](http://hl7.org/fhir/r4/valueset-publication-status.html)]*

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
        <td><a href="Patient-test-example-patient-identifier-value-only-t.html">Patient with only identifier.value</a></td>
        <td>test-example-patient-identifier-value-only-t</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-identifier-t.html">Patient with identifier.value and system (uuid)</a></td>
        <td>test-example-patient-identifier-t</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-t.html">Patient with IHI</a></td>
        <td>test-example-patient-ihi-t</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-t.html">Patient with a valid IHI and a non-valid IHI and Medicare Number</a></td>
        <td>test-example-patient-ihi-medicare-t</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-t.html">Patient with IHI and Medicare Number and DVA number</a></td>
        <td>test-example-patient-ihi-medicare-dva-t</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
     <tr>
        <td><a href="Patient-test-example-patient-ihi-medicare-dva-mr-t.html">Patient with IHI and Medicare Number and DVA number and MRN</a></td>
        <td>test-example-patient-ihi-medicare-dva-mr-t</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-local-identifiers-t.html">Patient with HPI-O scoped MRN and Local namespace MRN</a></td>
        <td>test-example-patient-local-identifiers-t</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-t.html">Patient with Medicare Number and a valid locally defined identifier</a></td>
        <td>test-example-patient-medicare-testident-t</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-testident-t.html">Patient with valid locally defined identifier</a></td>
        <td>test-example-patient-testident-t</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-t.html">Patient with Medicare Number</a></td>
        <td>test-example-patient-medicare-t</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-mult-medicare-testident-t.html">Patient with two Medicare Number and two valid locally defined identifiers</a></td>
        <td>test-example-patient-mult-medicare-testident-t</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-inv-testident-t.html">Patient with a valid Medicare Number and a non-valid locally defined identifier with Identifier.system only</a></td>
        <td>test-example-patient-medicare-inv-testident-t</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-dva-t.html">Patient with Medicare Number, locally defined identifier and DVA number</a></td>
        <td>test-example-patient-medicare-testident-dva-t</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
     </tbody>
</table>