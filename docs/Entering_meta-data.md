# Entering meta-data

### Confirmed

The confirmed flag should be set once this list entry has been reviewed and accepted.

The process for review is still to be determined.

### Jurisdiction

Enter each of the jurisdictions this identifier list covers using in the ISO 3166-1 two-digit alpha code.

If the list is global, use one of the XI, XM or ZZ.

If the list is regional, enter all the countries for the region.

### Sub-national

If this list only covers one or more sub-national territories, enter the [ISO 3166-2 Subdivision Assigned Code](https://en.wikipedia.org/wiki/ISO_3166-2#Format).

If the sub-division codes you are using are not already in the database, update the Sub-national jurisdictions table with the name of each subdivision.

> ***Example***:
> The UK Charity Commission only covers England and Wales.
>
> As a result, the entry for GB-CHC should have a Jurisdiction of **GB** and then entries in the Sub-national column for **‘GB-WLS’** and **‘GB-ENG’**

### URL

Provide the root URL where this list can be found.

### Name / Title

In the current version of the codelist, the name of the organisation list should be given in English. If a local language name is available, this should be provided after a / separator.

> ***Example: CO-RUE***
>
> "Single Business Register / Al Registro Único Empresarial"


### Description

The description should focus on explaining the way in which organisations end up on the list. If a list covers multiple kinds of organisation, the description may highlight this, using text from the lists own website, or summarised from other relevant documentation.

Descriptions may include Markdown. When including citations, use markdown footnote notation:

```md
This is some text which requires a citation at the end [1].

[1]: This is the footnote text.
```

> ***Example: AU-ABN***

> "The Australian Business Number (ABN) enables businesses in Australia to deal with a range of government departments and agencies using a single identification number. The ABN is a public number which does not replace an organisations tax file number."
>
> "ABN registration details become part of the Australian Business Register (ABR)"
>
> Each ABN should equate to a single 'business structure', although that structure may be used to carry out a range of business activities.  A range of kinds of entity are issued ABNs, including individuals, corporations, partnerships, unincorporated associations, trusts and superannuation funds. Entities must be carrying on a business in or connection to Australia to receive an ABN.



![image alt text](image_2.png)

### Legal structure

Select all the legal structures which this list covers.

Note that legal structures are organised hierarchically in the dataset. So, for example, ‘Sole Trader’ is a kind of company. This is shown in the lookup list under the ‘Parent’ field.

Please consult the research lead if you feel you need to add an extra category to legal structures.

If the list is not specific to a particular kind of legal structure, leave this field blank.

> ***Example: GB-COH***

> UK Companies House registers a number of different kinds of company, including:
>
> * Public limited company (PLC)
> * Private company limited by shares (Ltd, Limited)
> * Private company limited by guarantee, typically a non-commercial membership body such as a charity
> * Private unlimited company (either with or without a share capital)
> * Limited liability partnership (LLP)
> * Limited partnership (LP)
> * Societas Europaea (SE): European Union-wide company structure
> * Companies incorporated by Royal Charter (RC)
> * Community interest company
>
> It is listed against the following specific company types: Partnership, Limited Company, Listed Company, Community Interest Company, and Charity.
>
> **However**, wider research tells us that whilst all Limited Companies, Listed Companies and CIC’s should have a registration in Companies House, not all charities will have a Companies House number. As a result we also need to create a ‘Need to Know’ entry for jurisdiction GB, and organisation type Charity to state this.


### Sector

If this list is specific to a particular sector, you can declare that here.

If the list is not specific to a particular sector, leave this field blank.

> ***Example: GB-UKPRN***
>
> The UK Register of Learning Providers covers only education institutes, so has ‘Education’ set in the sector field.

### List type

This is one of the most important fields in the dataset. You will need to determine if this list is a **primary identifier list** or whether it has secondary, third-party or local status.

Definitions of each category are provided above.

Drawing on your research into how identifiers are created, and looking at a range of example entries in the list, make your determination. You can use the comments feature in AirTable to provide supporting reasons if you require.

The following rule-of-thumb criteria may be useful.

```eval_rst
.. list-table:: Rule of Thumb
   :header-rows: 1

   * - Primary
     - Secondary
     - Third-party
     - Local
   * - Provided by an official registrar

       Organisations were assigned the identifier at the time they were first created.

       Near 100% coverage of the legal type in a jurisdiction (e.g. list contains all companies)
     - Managed by an official source.

       Not all organisations of a given legal type will have these identifiers. Relies upon some other status of the organisation (e.g. VAT registration, being an employer etc.)
     - Maintained independently of the organisations listed.

       May be based on official records, but identifiers are assigned separately from official processes.

     - Maintained by a single organisation for their own business purposes.
```

### Wikipedia page

If you have found a wikipedia page for the organisation, link to that here.

### Finding the identifiers

If users need to follow particular steps in order to carry out a identifier search, detail those here.

This might include:

* Guidance on how to find search features on a complex website;

* Information on charged access to identifiers if no freely available online access is provided;

* Information on how to spot the actual identifier, and how to copy it for re-use;

* Information on formatting the identifiers.

> ***Example: AU-ABN***

> It is possible to search for identifiers at http://abr.business.gov.au/
>
> The Australian Business Number (ABN) is a unique 11 digit identifier issued to all entities registered in the Australian Business Register (ABR). The 11 digit ABN is structured as a 9 digit identifier with two
> leading check digits.
>
> The identifiers are displayed on the website with spaces in the number. All the spaces should be removed when making use of the number within an identifier.

### Example identifiers

Provide 1 - 5 example identifiers, comma separated.

> ***Example: GB-COH

09506232, 07444723
</td>
  </tr>
</table>


### Available online, and Online availability details

Indicate whether this list is available online in any form.

Provide brief details of the information that is available.

### Openly licensed and license details

Look for a license for the contents of the list.

Indicate whether or not an open license can be found, and provide the name of the license (if common) or a short description of the license if it is not a common license.

### Access to data & Data access details

Check for bulk downloads, and API access to the data, and indicate if these are available.

For official registers, check on the national data portal as well as the list website itself. Take note of whether the available data appears to be regularly updated, or only a one-off data dump.

Write brief notes on how the data can be accessed.

Confirm the license information for the data.

### Data features

Select all the features that are apply to **either **of information available through the list’s website, or in APIs or bulk data products.

The goal here is to be aware of all the possible additional available information that could be explored to disambiguate organisations, whether that is available as structured data or not.

### In OpenCorporates?

Tick if this list is available via OpenCorporates

### Languages supported

Using ISO e-digit language codes, indicate which languages this list is available in.

### Mappings

If your register has identified a mapping between this list and another list, you can create a new mapping entry here for outbound and inbound mappings.

### Last updated

Make sure the last updated date reflects the current date.
