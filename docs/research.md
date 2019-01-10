List research
=============

## Populating new entries

For list requests, the research team should seek to identify a potential source of organization identifiers.

The research process may involve:

* Online desk research;
* Consultation with the wider standards community;
* Consultation with local experts;

Once you have identified a good candidate list to meet a particular need, assign it a prefix as detailed below, and then fill in the detailed [metadata](metadata.md).

### Evaluating Candidate Registration Agencies

There is sometimes uncertainty whether a registration agency is suitable for inclusion in org-id. The following criteria can be used to determine when a registration agency or list can be included.

If the researcher **has** established a negative answer, or **cannot** establish a positive answer to any combination of the following, a registration agency or list is not suitable for inclusion into org-id.guide:

* Does the registration agency or list provide identifiers which will **uniquely refer** to one and only one organisation or entity within their jurisdiction?
* Does it provide identifiers which are **stable**? I.e. if an organisation has been given an identifier, are we sure that it will not change in the event of a change in the organisation’s structure, legal status, name, or location? There may be edge case scenarios in which identifiers change or duplicate identifiers are issued, but these cases should generally be rare and understood by the issuing authority and **documented by the researcher**, or historical in nature.
* Does it provide identifiers which *don’t change over time*? This is linked to the condition above, but is more specifically to do with predictable, mostly temporal changes. For instance, is the researcher sure that numerical values in an identifier do **not** refer to part of a process, a date, or something which looks like an organisation but is in fact a time bound object such as a licence? (If they are, the identifier could be subject to change over time). As with the point above, exceptions may be possible, but must be acknowledged by the agency and documented by the researcher.

> N.B. this section is still under development

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


### Existing use

For codes taken from the IATI Codelist, you can search for records that currently use this code via OIPA.

For example, the following query returns a list of activities (in JSON format) with reporting or participating organisation identifiers that start with ‘ET-MFA’

[https://oipa.nl/api/activities/?format=json&q_fields=reporting_org,participating_org&q_lookup=startswith&q=ET-MFA](https://oipa.nl/api/activities/?format=json&q_fields=reporting_org,participating_org&q_lookup=startswith&q=ET-MFA)

Checking each of the linked activities can give an indication of the kinds of identifier in use.

Current usage in IATI is no guarantee of a correct identifier, but, it can give clues as to the kinds of identifiers you are looking for, and can help validate organisation list information.
