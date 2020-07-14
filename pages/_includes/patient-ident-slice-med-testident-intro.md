**Patient with Medicare Number and a Locally Defined Identifier Type** *[[Draft](http://hl7.org/fhir/r4/valueset-publication-status.html)]*

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
        <td><a href="Patient-test-example-patient-medicare-testident-aq.html">Patient with Medicare Number and a valid locally defined identifier</a></td>
        <td>test-example-patient-medicare-testident-aq</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-ar.html">Patient with valid locally defined identifier</a></td>
        <td>test-example-patient-medicare-testident-ar</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-as.html">Patient with Medicare Number</a></td>
        <td>test-example-patient-medicare-testident-as</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-at.html">Patient with two Medicare Number and two valid locally defined identifiers</a></td>
        <td>test-example-patient-medicare-testident-at</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-au.html">Patient with a valid Medicare Number and a non-valid locally defined identifier with Identifier.system only</a></td>
        <td>test-example-patient-medicare-testident-au</td>
        <td>Fail</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-dva-av.html">Patient with Medicare Number, locally defined identifier and DVA number</a></td>
        <td>test-example-patient-medicare-testident-dva-av</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
      <tr>
        <td><a href="Patient-test-example-patient-medicare-testident-dva-aw.html">Patient with DVA number only; with no Medicare Number and no locally defined identifier</a></td>
        <td>test-example-patient-medicare-testident-dva-aw</td>
        <td>Pass</td>
        <td>Fail</td>
        <td>Internal error: Problem evaluating slicing expression for element in profile http://hl7.org.au/fhir/StructureDefinition/patient-ident-slice-med-testident-closedslice path Patient.identifier[0] (fhirPath = true and $this.conformsTo('http://hl7.org.au/fhir/StructureDefinition/au-medicarecardnumber')): Not supported yet</td>
      </tr>
     </tbody>
</table>