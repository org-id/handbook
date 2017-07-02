## Publishing lists and cross-walks

Many of the lists in the org-id.guide register are provided by official registries (company registrars, charity registers etc.).

However, in some cases, data publishers need to use their own **third party** or **local** lists. 

In these cases, data publishers should:

1. Publish these lists, and make sure they are registered with a code in org-id.guide
2. Provide cross-walks to other known primary or secondary identifiers for organisations where available. 


### Simple list format

```eval_rst

.. note:: Under development
    
    This format is under development, and subject to change. 

```

When publishing your own organisation list, provide at least:

* id - Your identifier for each organisation
* name - The common name of the organisation in your list

You are encouraged to include additional information to support organisation identification, including:

* alternateIdentifiers - An array of other known identifiers for the same organisation, constructed using the org-id list codes.
* legalName - The official legally registered name of the organisation (if known)
* address - Any addresses held in your system for this organisation, broken down into:
  * type - e.g. 'registered', 'trading', 'contact'
  * address - A line break or comma separated list of address lines;
  * postalCode - The full or partial postal code
  * country - The ISO 2-Digit country code. When detailed address information can't be provided, giving at least the country code of where the organisation is registered can support disambiguation.
* type - An indication of the legal status of the organisation (e.g. company, government agency etc.)
* country - the country where the organisation is registered
* 