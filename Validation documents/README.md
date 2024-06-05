# AUNZ-Validation artefacts

This repository contains the validation artefacts for the Australian - New Zealand invoice specification.

The Schematron folder contains three validation artefacts:

* AUNZ-UBL-validation.sch adapts the EN16931 business rules to the Australian - New Zealand requirements. It should be applied to any invoice, credit note or self-billed invoice.
* AUNZ-PEPPOL-validation.sch derived from the OpenPeppol business rules and adapted to AUNZ. It shall be applied to invoices and credit notes.
* AUNZ-PEPPOL-SB-validation.sch derived from the OpenPeppol business rules adapted to AUNZ. It shall be applied to Self-Billing invoices and Self-Billing credit notes.

This repository also contains an xslt folder with the xslt artefacts compiled from the schematron validation artefacts. Any of them can be used for validation of an A-NZ electronic invoice.

## PINT A-NZ Migration
In December 2023 the new Peppol International (PINT) A-NZ Billing specification was published.  The Australian and New Zealand Peppol Authorities have committed to migrating to that specification.  The migration dates are confirmed, the PINT A-NZ Billing specification will become mandatory on 15 November 2024 and after 15 May 2025 the A-NZ Peppol BIS 3.0 extensions will be phased out and no longer available for use.  For more information see the [PINT A-NZ v1.0](https://docs.peppol.eu/poac/aunz/) (current) and [PINT A-NZ v1.0.1](https://docs.peppol.eu/poac/aunz/2024-Q2/) (effective 1 September 2024) specifications.  The validation artefacts are also included in the downloadable resources.

## Validation process

In order to validate a document instance, the following process should be used:

* Use the UBL Invoice.xsd or the UBL CreditNote.xsd version 2.1 for schema validation depending on the document type.
* Validate the syntax boundaries and the derived EN16931 business rules using the AUNZ-UBL-validation.sch for invoice, credit note or self-billing depending on the document type.
* Validate PEPPOL rules and specific AUNZ business rules using the AUNZ-Peppol-validation.sch or AUNZ- Peppol-SB-validation.sch, depending on the type of instance.

To validate the syntax, the UBL 2.1(ISO/IEC 19845:2015) schema shall be used.

[UBL Website](https://www.oasis-open.org/committees/ubl/)

## Release Notes

The A-NZ release notes are available [here](https://github.com/A-NZ-PEPPOL/A-NZ-PEPPOL-BIS-3.0/tree/master/Specifications).

Peppol BIS Billing 3.0 release notes are available [here](https://docs.peppol.eu/poacc/upgrade-3/2024-Q2/release-notes/).
