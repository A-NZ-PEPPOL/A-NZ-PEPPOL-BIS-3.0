# AUNZ-Validation artefacts

This repository contains the validation artefacts for the Australian - New Zealand electronic invoice specification.

The AUNZ Validation Artefacts are based on two validation artefacts:
* European Norm validation artefacts v1.2.3 https://github.com/ConnectingEurope/eInvoicing-EN16931/releases/tag/validation-1.2.3 
* PEPPOL electronic invoice Spring Release https://github.com/OpenPEPPOL/peppol-bis-invoice-3/releases/tag/3.0.4

# Release Notes
   
* Release 1.0.4 (17 November 2020)
  
  - Incorporated changes listed in the BIS Billing 3.0 updates for version 3.0.7 (hotfix in June 2020) and 3.0.8 (November 2020) where applicable, including updated EAS and ICD code lists, and minor correction to the ISO currency code list.   Peppol release notes can be found at: https://docs.peppol.eu/poacc/billing/3.0/release-notes/
  - Incorporated updates relating to CEF issues 206, 213, 215, 217, 219, 220, 224, 225, 230, 237. 
These include: 
- New rules: BR-CL-26, UBL-CR-680
- Updated UBL-CR-295, BR-CO-19, BR-E-05, UBL-CR-673, and UBL-CR-412.
   
* Release 1.0.3 (15 May 2020)
  - New rules: BR-66, BR-67, UBL-CR-673, UBL-CR-674, UBL-CR-675, UBL-CR-676, UBL-CR-677, UBL-CR-678 and UBL-CR-679 
  - New rules: PEPPOL-COMMON-R041 and PEPPOL-COMMON-R042 (algorithm check for Norwegian and Danish organisation numbers)
  - Updated BR-CL-14 and BR-CL-15 to reflect updated country code list 3166
  - Updated BR-CL-16 to reflect updated payment means code list 4461
  - Bug fix for BR-17
  - Updated severity from 'warning' to 'fatal' for UBL-CR-666 
  - Updated error message for PEPPOL-EN16931-R044
  - Removed rule BR-S-08 to support decimals in tax rate
  - Removed BR-CL-08 which is related to EN and does not improve automation for A-NZ. 
  - Updated BR-CL-25 with additional codes, which is however further restricted by PEPPOL-EN16931-CL008. Schematron update only and no impact on effective business use of EAS codes.
 
* Release 1.0.2 (January 2020)
 
* Correction of the profile identifier in AUNZ-PEPPOL-SB-validation

* Release 1.0.1 (November 2019)
 
**Aligns with the Peppol `BIS 3.0.5` November 2019 release.**

* Release 1.0.0 (October 2019)
 
**Initial release.**

There are three validation artefacts that should be applied to validate an AUNZ electronic invoice instance:

* AUNZ-UBL-validation.sch adapts the EN16931 business rules to the Australian - New Zealand requirements. It should be applied to any invoice, credit note or selfbilled invoice.
 
* AUNZ-PEPPOL-validation.sch derived from the OpenPEPPOL business rules and adapted to AUNZ. It shall be applied to invoices and credit notes.
* AUNZ-PEPPOL-SB-validation.sch derived from the OpenPEPPOL business rules adapted to AUNZ. It shall be applied the selfbilling invoices and selfbilling credit notes.


To validate the syntax, the UBL 2.1 schema shall be used:
* `ubl` - UBL 2.1 (ISO/IEC 19845:2015) 
  * UBL Website: https://www.oasis-open.org/committees/ubl/

   
# Validation process

In order to validate a document instance, the following process should be used:

* Use the UBL Invoice.xsd or the UBL CreditNote.xsd version 2.1 for schema validation depending on the document type
* Validate the syntax boundaries and the derived EN16931 business rules using the AUNZ-UBL-validation.sch
* Validate PEPPOL rules and specific AUNZ business rules using the AUNZ-PEPPOL-validation.sch or AUNZ-PEPPOL-SB-validation.sch depending on the type of instance 

This repository contains an xslt folder with the xslt artefacts compiled from the schematron validation artefacts. Any of them can be used for validation of an AUNZ electronic invoice.
