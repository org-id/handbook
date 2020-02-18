List research
=============

## Populating new entries

For list requests, the research team should seek to identify a potential source of organization identifiers.

The research process may involve:

* Online desk research;
* Consultation with the wider standards community;
* Consultation with local experts;

Once you have identified a good candidate list to meet a particular need, assign it a prefix as detailed below, and then fill in the detailed [metadata](metadata.md).

## Validating an existing entry

For stub entries or proposals with incomplete information, researcher sshould: 

1. **Check the list title** - and make sure it follows the [rules for multilingual titles](metadata.md)

2. **Write a clear description of the identifier list** describing the way in which organisations end up on the list. This should be 1 - 2 paragraphs maximum. You may use content quoted from the registers own website, or wikipedia pages.

3. **Fill in the list [metadata](metadata.md)**

## Research sources

When carrying out research the following resources may be useful. All researchers are encouraged to familiarise themselves with these resources.

### Useful websites

* **Investigative dashboard** - https://investigativedashboard.org/databases/topics/business list of company registers

* **Wikipedia.** Primary and secondary identifier lists are usually notable enough to have a Wikipedia page, at least in the language of the country concerned. For official registers - look for information about the legislation that created the register in order to understand the organisation types it covers. See in particular [List_of_company_registers](https://en.wikipedia.org/wiki/List_of_company_registers) and [Types_of_business_entity](https://en.wikipedia.org/wiki/Types_of_business_entity)

* The [World Bank Doing Business](http://www.doingbusiness.org/) country profile give detailed information on company registration processes - and can provide useful hints as to the official company register and identifiers in a country.

* [OpenCorporates Open Company Index](http://registries.opencorporates.com/)

* [European Commission list of Business registers in Member States](https://e-justice.europa.eu/content_business_registers_in_member_states-106-en.do)

* [Wiki Procedure](https://www.wikiprocedure.com)

* [Open Corporates policy paper on handling company number problems](https://docs.google.com/document/d/1cQ626bFP-66LtXX4oJ_nEoyDjBtGtJ8RITbdK6W6nOk/edit)

* [European Business Register list of worldwide registers](https://ebra.be/worldwide-registers/)


### Existing use

For codes taken from the IATI Codelist, you can search for records that currently use this code via OIPA.

For example, the following query returns a list of activities (in JSON format) with reporting or participating organisation identifiers that start with ‘ET-MFA’

[https://oipa.nl/api/activities/?format=json&q_fields=reporting_org,participating_org&q_lookup=startswith&q=ET-MFA](https://oipa.nl/api/activities/?format=json&q_fields=reporting_org,participating_org&q_lookup=startswith&q=ET-MFA)

Checking each of the linked activities can give an indication of the kinds of identifier in use.

Current usage in IATI is no guarantee of a correct identifier, but, it can give clues as to the kinds of identifiers you are looking for, and can help validate organisation list information.
