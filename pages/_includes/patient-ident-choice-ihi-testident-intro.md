**Patient with Medicare Number and a Locally Defined Identifier Type** *[[Draft](http://hl7.org/fhir/r4/valueset-publication-status.html)]*

Prototype derived profile uses open slice to allow maximum of one Medicare Numvber and maximum of one locally defined Identifier types (not defined in AU Base).

**Test Examples**

[Patient with Medicare Number and a valid locally defined identifier](Patient-test-example-patient-medicare-valid-testident-aa.html) id=test-example-patient-medicare-valid-testident-aa, Expected:Pass

[Patient with valid locally defined identifier](Patient-test-example-patient-medicare-valid-testident-ab.html) id=test-example-patient-medicare-valid-testident-ab, Expected:Pass

[Patient with Medicare Number](Patient-test-example-patient-medicare-valid-testident-ac.html) id=test-example-patient-medicare-valid-testident-ac, Expected:Pass

[Patient with two Medicare Number and two valid locally defined identifiers](Patient-test-example-patient-medicare-valid-testident-ad.html) id=test-example-patient-medicare-valid-testident-ad, Expected:Fail
