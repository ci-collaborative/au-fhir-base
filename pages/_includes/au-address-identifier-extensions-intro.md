**AU Base Address with Identifier Extension** *[[FMM Level 2](guidance.html)]*

_This profile is a prototype design option of AU Base Address. It demonstrates the modelling and inclusion of address identifiers via a single identifier extension on the Address data type._

This profile is provided for use in an Australian context where some constraint on content is desirable to guarantee the quality of an Australian address whilst still supporting
other uses such as unstructured addresses. 

#### Identifiers
These definitions, defined as profiles of [Identifier](http://hl7.org/fhir/R4/datatypes.html#Identifier), represent common identifiers that may be sent using the [Address Identifier](StructureDefinition-address-identifier.html) extension:
* [Delivery Point Identifier](StructureDefinition-au-deliverypointidentifier.html)
* [G-NAF Identifier](StructureDefinition-au-gnafidentifier.html)


#### Extensions
Extensions used in this profile:
* Address: [Address Identifier](StructureDefinition-address-identifier.html)
* Address: [No Fixed Address](StructureDefinition-no-fixed-address.html)


#### Usage Notes
* Is for use when representing an Australian (location) address so country is fixed to AU.
* Is not bound to any elements in this implementation guide directly.
* Overseas addresses can be represented using the core Address data type.
* May be used as needed in implementation guide by use cases.
* Is provided as the best practice guidance on Australian address representation.


Standard extensions for address are available [here](http://hl7.org/fhir/R4/datatypes-extras.html#address)

For example can consider the following for address parts support:
* [Unit](http://hl7.org/fhir/R4/extension-iso21090-adxp-unitid.html)
* [House Number](http://hl7.org/fhir/R4/extension-iso21090-adxp-housenumber.html)
* [Street Name](http://hl7.org/fhir/R4/extension-iso21090-adxp-streetname.html)
* [Street Name Type](http://hl7.org/fhir/R4/extension-iso21090-adxp-streetnametype.html)
* [Street Name Base](http://hl7.org/fhir/R4/extension-iso21090-adxp-streetnamebase.html)

See more info at : [ISO 21090 Data Type Extensions](http://hl7.org/fhir/R4/iso-21090.html)


**Examples**

[Postal address (with DPID and G-NAF Identifier) and work address in Darwin, NT](Patient-address-example0-identifiers.html)

[Level 1, 300 George St, Brisbane, QLD 4000](Patient-address-example1.html)

[No fixed address in Melbourne, VIC](Patient-address-example2.html)