# A-NZ PEPPOL BIS 3.0
Within this repository is a range of artefacts that will help Peppol Service Providers to implement and adopt the Australia-New Zealand extension of the [Peppol BIS Billing](https://docs.peppol.eu/poacc/billing/3.0/2023-Q4/) and should be read in conjunction with that specification. 

In December 2023 the new Peppol International (PINT) A-NZ Billing specification was published.  The Australian and New Zealand Peppol Authorities have committed to migrating to that specification.  The migration dates are confirmed, the PINT A-NZ Billing specification will become mandatory on 15 November 2024 and after 15 May 2025 the A-NZ Peppol BIS 3.0 extensions will be phased out and no longer available for use.  You can view the new PINT A-NZ specification [here](https://docs.peppol.eu/poac/aunz/).

No localised versions of other Procure to Pay (P2P) specifications are required. See Procure to Pay section below for further details.

## What's inside
* [A-NZ Peppol BIS 3.0 Specifications](https://github.com/A-NZ-PEPPOL/A-NZ-PEPPOL-BIS-3.0/tree/master/Specifications)
* [A-NZ Schematron validation documents](https://github.com/A-NZ-PEPPOL/A-NZ-PEPPOL-BIS-3.0/tree/master/Validation%20documents)
* [A-NZ Specification XML message examples](https://github.com/A-NZ-PEPPOL/A-NZ-PEPPOL-BIS-3.0/tree/master/Message%20examples)

## Specification and Schematron release process

### A-NZ Invoicing and Self-Billing

The A-NZ release notes are available [here](https://github.com/A-NZ-PEPPOL/A-NZ-PEPPOL-BIS-3.0/tree/master/Specifications).

The A-NZ Invoice and Self-Billing specifications are substantially the same as Peppol BIS Billing with minor differences e.g. to accommodate GST rather than VAT.

With each Peppol release, changes to BIS Billing are reflected in the A-NZ specifications which are generally published approximately two weeks after the Peppol BIS release.

In the rare event of potentially significant changes being to BIS Billing made at short notice, the changes may be reflected in the A-NZ extension in the following biannual release.

### Peppol Biannual Release Process

The Peppol BIS Billing release notes are available [here](https://docs.peppol.eu/poacc/upgrade-3/2023-Q4/release-notes/).

Peppol standards for business processes and transactions are updated biannually in May and November. Releases typically contain minor corrections and/or enhancements proposed by Peppol members (service providers or Peppol Authorities). 

Key dates for Peppol releases are available [here](https://peppol.eu/downloads/post-award/). 

The specifications provide message syntax, business rules, code lists and implementation guidance, and are supported by centrally maintained validation artefacts to assist service providers to implement services that comply with the standards.

## Procure to Pay (Peppol eProcurement)

### Localisation

While BIS Billing is constrained to comply with European standards (EN16931), including using the term ‘VAT’ in the definition of a number of terms and business rules, no such constraint exists for the other Peppol eProcurement documents.

Peppol eProcurement specifications were updated in May 2020 to support non-VAT tax schemes including GST, and that allowed A-NZ providers to implement Peppol eProcurement documents ‘as-is’ without localisation.

Therefore the normal Peppol release processes apply to those documents without the need to subsequently issue localised specifications.

### Procure to Pay documents supported by Peppol

Peppol supports a suite of eProcurement business documents that can be used in Australia and New Zealand including;
* **Invoice Response**: enables status notification for an invoice or credit note, e.g. an invoice is accepted, being processed, rejected, or under query. Specific message responses improve the efficiency for both parties to address exceptions.
* **Catalogue (and Catalogue Response)**: enables the automated exchange of catalogue information including the seller providing a new, updated or deleted catalogue, and the buyer advising whether the information (new or updates) is accepted in the buyers’ ERP system.
* **Punch Out**: enables integration between the seller’s web catalogue and buyer’s procurement system to create a product or service list for the buyer, which can later be used as the basis for an order or item comparison list.
* **Order (and Order Response)**: enables order automation in line with catalogue and invoice. A buyer creates an order and the seller either accepts the order, accepts the order with changes or rejects the order and responds with the required information. Invoices containing an order reference can be matched automatically.
* **Despatch Advice**: enables communication between Seller and Consignee regarding transport details including packing and delivery, ordering details including what was sent, quantity of goods sent and items outstanding, and receiving goods including delivery time and address details.

The Peppol specifications and technical artefacts are available [here](https://docs.peppol.eu/poacc/upgrade-3/2023-Q4/).

## Feedback
If you have any questions or feedback, please contact your relevant Peppol authority:

* The New Zealand Peppol Authority - [support@nzpeppol.govt.nz](mailto:support@nzpeppol.govt.nz)
* The Australian Peppol Authority - [eInvoicing@ato.gov.au](mailto:eInvoicing@ato.gov.au)

