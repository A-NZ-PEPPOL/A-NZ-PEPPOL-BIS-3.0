# A-NZ PEPPOL BIS 3.0
Within this repository is a range of artefacts that will help PEPPOL Service Providers implement and adopt the Australia-New Zealand extension of the PEPPOL BIS 3.0 Specification.
## What's inside
* [A-NZ PEPPOL BIS 3.0 Specifications](https://github.com/A-NZ-PEPPOL/A-NZ-PEPPOL-BIS-3.0/tree/master/Specifications)
* [A-NZ Schematron validation document](https://github.com/A-NZ-PEPPOL/A-NZ-PEPPOL-BIS-3.0/tree/master/Validation%20documents)
* [A-NZ Specification XML message examples](https://github.com/A-NZ-PEPPOL/A-NZ-PEPPOL-BIS-3.0/tree/master/Message%20examples)

## Feedback
Please do not hesitate to get in touch if you have any feedback on ways we can improve this repository.
* The New Zealand PEPPOL Authority - [support@nzpeppol.govt.nz](mailto:support@nzpeppol.govt.nz)
* The Australian Taxation Office - [e-invoicing@ato.gov.au](mailto:e-invoicing@ato.gov.au)


## Release notes

### Version 1.0.4 `17/11/2020`

**Aligns with the Peppol `BIS 3.0.8` November 2020 release.**


Release includes:
* Incorporated changes listed in the BIS Billing 3.0 updates for version 3.0.7 (hotfix in June 2020) and 3.0.8 (November 2020) where applicable, including updated EAS and ICD code lists, and minor correction to the ISO currency code list.   Peppol release notes can be found at: https://docs.peppol.eu/poacc/billing/3.0/release-notes/
* Incorporated updates relating to CEF issues 206, 213, 215, 217, 219, 220, 224, 225, 230, 237. 
These include: 
* New rules: BR-CL-26, UBL-CR-680
* Updated UBL-CR-295, BR-CO-19, BR-E-05, UBL-CR-673, and UBL-CR-412.


### Version 1.0.3 `15/05/2020`

**Aligns with the Peppol `BIS Billing 3.0.6` May 2020 release.**


Release includes:
* Updated specification documents and validation artefacts with bug fixes, editorial corrections and the following minor enhancements:
  - Two new business rules relating to Payment Means
  - Two new business rules relating to Norwegian and Danish organisation number formats (from BIS Billing Nov 2019 release)
  - Two 'fatal' business rules related to Additional Document Reference (one new, one previously a warning)
  - Removal of an irrelevant rule relating to subject codes within the invoice level Note
  - Support for additional codes in UNCL4451 note subject code and ISO 3166-1:Alpha2 Country code
* Refer to Validation documents [README.md]( https://github.com/A-NZ-PEPPOL/A-NZ-PEPPOL-BIS-3.0/blob/master/Validation%20documents/README.md) for further details
* Updated message example files

### Version 1.0.2 `20/03/2020`


Release includes:
* Data element AccountingCustomerParty/Party/PartyTaxScheme/CompanyID to be New Zealand GST number rather than NZBN
* Clarification included on the use of business identifier vs. GST identifier for PartyTaxScheme/CompanyID within AccountingSupplierParty and TaxRepresentativeParty groups
* Minor corrections to rule references in the syntax table


### Version 1.0.1 `20/11/2019`

**Aligns with the Peppol `BIS 3.0.5` November 2019 release.**


Release includes:
* AUNZ rule numbers should be 3 digit: e.g. AUNZ-R-XXX
* Five rules (UBL-SR group) have been changed to GST from VAT.
* BuyerCountry and SupplierCountry parameter fixed (affecting a list of rules for ABN and NZBN checking)
* Fixed error message (with wrong customizationID)
* Fixed right single quotation marks in a few error message texts that may cause encoding issue.
* Removed rule AUNZ-R-003

### Version 1.0.0 `18/10/2019`
No release notes available

