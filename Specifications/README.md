# A-NZ Specifications

This repository contains; 

   * A-NZ Invoice specification

   * A-NZ Self-Billing specification

Guidance notes related to specifications are available [here](https://github.com/A-NZ-PEPPOL/Guidance-documents).

## A-NZ Release Notes:

Peppol BIS Billing release notes are available [here](https://docs.peppol.eu/poacc/billing/3.0/release-notes/).

### May 2022 – Invoice and Self-Billing specification v1.0.7
Effective date 30 May 2022, Mandatory from 12:00PM AEST/2:00PM NZST 27 June 2022.

Aligns with the Peppol BIS 3.0.13 May 2022 release.

Release includes:

* Adopted changes as appropriate, as per [BIS Billing release 3.0.13]( https://docs.peppol.eu/poacc/billing/3.0/release-notes/#_version_3_0_13), code list and validation artefact updates:

  -	New PEPPOL-COMMON-R050 rule to validate the format of ABNs, replacing A-NZ rule AUNZ-R-006. The severity of this rule is warning (consistent with AUNZ-R-006), expected to be updated to ‘fatal’ in the November 2022 release.
Note - There is no change to the validation of NZBNs, which are GLNs and so are validated under Peppol rule PEPPOL-COMMON-R040.

  -	Change PEPPOL-COMMON-R043 rule severity from ‘warning’ to ‘fatal’.
  -	New PEPPOL-COMMON-R049 rule to validate the format of Swedish organization number. 
    The severity of this rule is warning, expected to be updated to ‘fatal’ in the November 2022 release.
  - New rules UBL-CR-681 and UBL-CR-682, both with ‘warning’ severity to check for elements PaymentMeans/InstructionNote and Delivery/DeliveryAddress.
  - Change to PEPPOL-EN16931-R080 to apply rule to Credit Note only. 
  - Change BR-51 from ‘fatal’ to ‘warning’.
  - Corrections/improvements to warnings UBL-CR-414, UBL-CR-487, UBL-CR-512, UBL-CR-607, UBL-CR-665.

  - New invoice type codes added (see [updated code list UNCL 1001](https://docs.peppol.eu/poacc/billing/3.0/codelist/UNCL1001-inv/)). Please note:
    - A number of new codes are added to EN16931 (implemented through BR-CL-01). 
      The available codes are restricted by PEPPOL-EN16931-P0100.
      New codes supported are: 71, 102, 218, 219, 331, 382, 553, 817, 870, 875, 876, 877.
      - The advice from Peppol indicates that code 388 will be supported where a government tax/revenue authority issues invoices for tax (only).
    - Added to BIS instructions that these additional invoice type codes shall be handled as synonyms to the 380 code and thus do not require change in   processing.
 
  - New codes added to multiple code lists (ICD, EAS, Allowance Reason):
    - ICD code list: 0214, 0215, 0216 which affects rules BR-CL-10, BR-CL-11, BR-CL-21, BR-CL-25, BR-CL-26.
    - EAS code list: 0147, 0170, 0188, 0215, 0216 which affects rule BR-CL-25.
    - Allowance Reason Code list: 105 which affects rule BR-CL-19.

### November 2021 - Invoice and Self-Billing Specification v1.0.6
Publication date 15 November 2021, Mandatory from 12:00PM AEST/2:00PM NZST 29 November 2021.

Aligns with the Peppol BIS 3.0.12 November 2021 release.

Release includes:

* Adopted changes as appropriate, as per [BIS Billing release 3.0.12]( https://docs.peppol.eu/poacc/billing/3.0/release-notes/#_version_3_0_12) and validation artefacts:

  - Included six new rules PEPPOL-COMMON-R043 to PEPPOL-COMMON-R048 confirming the format of Belgium and Italian organisation identifiers. These have been implemented as Warnings in this release, and will become ‘fatal’ errors in the May 2021 release.

  - Incorporated schematron updates relating to [CEF issues](https://github.com/ConnectingEurope/eInvoicing-EN16931/issues?q=is%3Aissue+) 219, 234, 257, 286, 287, 293:
    - Minor correction to BR-CO-19 to align with BIS Billing
    - Include versioning in schematron validation artefacts
    - BR-CO-15 schematron code changed (removed //) and UBL-SR-06
    - Re-include the corrected UBL-SR-27 to prevent multiple PaymentMeansCodes within each PaymentMeans (multiple PaymentMeans continue to be allowed within the A-NZ specification)
    - Minor corrections for the following UBL-CR-nnn rules: UBL-CR-022, UBL-CR-028, UBL-CR-051, UBL-CR-067, UBL-CR-084, UBL-CR-100, UBL-CR-115, UBL-CR-183, UBL-CR-247, UBL-CR-282, UBL-CR-358, UBL-CR-384, UBL-CR-414, UBL-CR-419, UBL-CR-512, UBL-CR-538, UBL-CR-572, UBL-CR-577, UBL-CR-583, UBL-CR-607, and UBL-CR-625 to UBL-CR-644
* Added BT identifiers to syntax table.
* Minor editorial updates.

### May 2021 - Invoice and Self-Billing Specification v1.0.5 
Publication date 14 May 2021, Mandatory from 12:00PM AEST/2:00PM NZST 31 May 2021.

Aligns with the Peppol BIS 3.0.10 May 2021 release.

Release includes:

* Adopted changes as appropriate, as per [BIS Billing release 3.0.10](https://docs.peppol.eu/poacc/billing/3.0/release-notes/), including updated [code lists](https://docs.peppol.eu/poacc/billing/3.0/codelist/):
   - Electronic Address Scheme (EAS)
   - ISO 6523 ICD list
   - ISO 4217 Currency code
   - ISO 3166-1:Alpha2 Country codes
   - Units of measure – UN/ECE Recommendation 20 and 21 code
   - Item type identification code (UNCL7143)
   - Charge reason code (UNCL7161)

   Note: updates made under BIS Billing Hotfix v3.0.9 relate to country-specific rules and are not applicable in A-NZ.

* Adopted selected changes to UBL-SR rule severity (to become ‘fatal’) made in BIS Billing release 3.0.8 from [CEF #214](https://github.com/ConnectingEurope/eInvoicing-EN16931/issues/214) that were not applied to A-NZ specifications at the time:
   - UBL-SR-01 to UBL-SR-26, UBL-SR-28, UBL-SR-30 to UBL-SR-37, UBL-SR-39 to UBL-SR-43, UBL-SR-48 to UBL-SR-50.
* Removed as a result of review of UBL-SR-nn rules: 
   - UBL-SR-29 (SEPA doesn’t apply in AU-NZ).
   - UBL-SR-27, UBL-SR-38 (reference elements that do not occur in syntax)
* The following will remain as warnings (no change) to support common business practice in A-NZ by allowing multiple (different) Payment Means to be included in an invoice:
   - UBL-SR-44 
   - UBL-SR-45 
   - UBL-SR-46 
   - UBL-SR-47
* Clarified that rules BR-B-01 and BR-B-02, introduced with BIS Billing release 3.0.8 to support Italian domestic invoices, are not applicable for A-NZ.
* Editorial changes for clarification
   - Updated NZIRD link for credit note.
   - Updated NZ GST number example (removal of hyphens and, where the number is 8 digits long, it should lead with a zero).
   - Updated description of cbc:Note field.
   - Included clarification for including NZ bank account number.
* Minor corrections to rules table, and rules referenced from syntax table and minor editorial updates.

### November 2020 - Invoice and Self-Billing Specification v1.0.4 
Release date 17/11/2020, Mandatory from 07/12/2020.
Aligns with the Peppol BIS 3.0.8 November 2020 release.

Release includes:

* Incorporated changes listed in the BIS Billing 3.0 updates for version 3.0.7 (hotfix in June 2020) and 3.0.8 (November 2020) where applicable, including updated EAS and ICD code lists, and minor correction to the ISO currency code list. The change of severity from ‘warning’ to ‘fatal’ for UBL-SR-nn rules was not applied.
* Incorporated updates relating to [CEF issues](https://github.com/ConnectingEurope/eInvoicing-EN16931/issues?q=is%3Aissue+) 206, 213, 214, 215, 217, 219, 220, 224, 225, 230, 237.
* New rules: BR-CL-26, UBL-CR-680.
* Updated UBL-CR-295, BR-CO-19, BR-E-05, UBL-CR-673, and UBL-CR-412.

### May 2020 - Invoice and Self-Billing Specification v1.0.3
Release date 15/05/2020, Mandatory from 30/05/2020.
Aligns with Peppol BIS Billing 3.0.6 May 2020 release.

Release includes:

* Updated specification documents and validation artefacts with bug fixes, editorial corrections and the following minor enhancements:
   - Two new business rules relating to Payment Means.
   - Two new business rules relating to Norwegian and Danish organisation number formats (from BIS Billing Nov 2019 release).
   - Two 'fatal' business rules related to Additional Document Reference (one new, one previously a warning).
   - Removal of an irrelevant rule relating to subject codes within the invoice level Note.
   - Support for additional codes in UNCL4451 note subject code and ISO 3166-1: Alpha2 Country code.
* Updated message example files.

### March 2020 - Invoice and Self-Billing Specification v1.0.2
Release date 20/03/2020.

Release includes:

* Data element AccountingCustomerParty/Party/PartyTaxScheme/CompanyID to be New Zealand GST number rather than NZBN.
* Clarification included on the use of business identifier vs. GST identifier for PartyTaxScheme/CompanyID within AccountingSupplierParty and TaxRepresentativeParty groups.
* Minor corrections to rule references in the syntax table.

### November 2019 - Invoice and Self-Billing Specification v1.0.1 
Release date 15/11/2019.
Aligns with the Peppol BIS 3.0.5 November 2019 release.

Release includes:

* AUNZ rule numbers should be 3 digit: e.g. AUNZ-R-XXX.
* Five rules (UBL-SR group) have been changed to GST from VAT.
* BuyerCountry and SupplierCountry parameter fixed (affecting a list of rules for ABN and NZBN checking).
* Fixed error message (with wrong customizationID).
* Fixed right single quotation marks in a few error message texts that may cause encoding issue.
* Removed rule AUNZ-R-003.

### October 2019 - Invoice and Self-Billing Specification v1.0.0 
Release date 15/11/2019.
* Initial release.
