Meta-data guide
===============

For each entry in org-id.guide, a full meta-data entry is maintained, following the :doc:`schema <schema>`. This meta-data:

* Helps data publishers to understand the nature of an organization identifier list, and how to find the identifiers it contains;
* Helps users to interpret identifiers, and locate additional sources of information linked to each id;
* Drives the quality and relevance rankings used in the org-id.guide frontend;

Assigning a Code
----------------

Each **organisation list** code is made up of two parts: a jurisdiction code, and a list name code.

1) Jurisdiction code
~~~~~~~~~~~~~~~~~~~~

For any list which contains entries only from a given country, the `ISO 2-digit country code should be used <https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2#Officially_assigned_code_elements>`_.

For any list which contains entries only from a given subdivision of a country, the ISO 2-digit country code, followed by underscore, followed by the `subdivision code should be used <https://en.wikipedia.org/wiki/ISO_3166-2>`_. (For example "CA_BC" would be used for British Columbia, Canada.) 

For lists that contain entries from multiple countries, one of the following codes should be used (NOTE:  We rely here on the fact that in ISO 3166-1 the following alpha-2 codes can be user-assigned: AA, QM to QZ, XA to XZ, and ZZ. We avoid any widely used X codes. ).

+--------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Code   | Usage                                                                                                                                                                    |
+--------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| XM     | Multilateral/international agencies. The list contains multilateral or international agencies. These organisations are generally not registered at the national level.   |
+--------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| XI     | International. The list contains organisations based anywhere in the world. The organisations may or may not be registered at the national level.                        |
+--------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| XR     | Regional. The list contains organisations based within a particular region. For example, organisations within the European Union, or within Africa only.                 |
+--------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| ZZ     | Publisher created. This list was created by a publisher, and is maintained by that publisher alone.                                                                      |
+--------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------+


2) List name code
~~~~~~~~~~~~~~~~~

The list name code is manually assigned. In general, list name codes have been designed so that:

1. They are between 2 and 7 characters long;
2. They use a recognisable acronym or contraction of the name of the organisation list;
3. Acronyms should be based on the local language version of the name;
4. Codes should be memorable, allowing users to become familiar with codes.

However, there is no intention that the list name code portion of the prefix will carry any semantics (e.g. type of organisations listed etc.).

Points 1 - 4 are guidance only. Breaking any of these principles shall not be grounds for revision of an existing code.

When a new organisation list is identified, the creator/proposer may suggest a list code.

To confirm a code, the researcher should check:

* The proposed list code is based on a clear understanding of the name of the underlying **organisation list** or list provider.

* Any requirements for multi-lingual codes. For example, in Canada, acronyms should always be given in both their English and French forms. This is achieved using an underscore separator in the list code. (For example  CA-CRA_ACR for the Canadian Revenue Agency / Agence du revenu du Canada)

* The code does not duplicate an existing code, or AKA value.

If a list code is later replaced, the full deprecated prefix should be recorded in the ```formerCodes`` field. This will allow systems to warn about deprecated prefixes and to notify users of their replacements.

Entering meta-data
------------------

Name / Title
~~~~~~~~~~~~

Provide the name of the **identifier list**, or, where the list is the primary list maintained by an organisation, the name of the organisation that maintains the list.

You can enter the name in English, and separately in a local language.

.. hint::

    For example, we use 'Companies House' to identify the owner of the UK Company Register.

URL
~~~

Provide the root URL where information on the list can be found. This does not need to link directly to an interface to search the list.

Description
~~~~~~~~~~~

The description should focus on explaining the way in which organisations end up on the list. If a list covers multiple kinds of organisation, the description may highlight this, using text from the lists own website, or summarised from other relevant documentation.

Descriptions may include Markdown. When including citations, use markdown footnote notation:

.. code-block:: markdown

    This is some text which requires a citation at the end [1].

    [1]: This is the footnote text.

.. hint:: **Example Description - AU-ABN**

  "The Australian Business Number (ABN) enables businesses in Australia to deal with a range of government departments and agencies using a single identification number. The ABN is a public number which does not replace an organisations tax file number."

  "ABN registration details become part of the Australian Business Register (ABR)"

  Each ABN should equate to a single 'business structure', although that structure may be used to carry out a range of business activities.  A range of kinds of entity are issued ABNs, including individuals, corporations, partnerships, unincorporated associations, trusts and superannuation funds. Entities must be carrying on a business in or connection to Australia to receive an ABN.


Geographic coverage
~~~~~~~~~~~~~~~~~~~

Enter each of the jurisdictions this identifier list covers.

If the list is global, use one of the XI (International), XM (Multilateral) or ZZ (Publisher created).

If the list is regional, enter all the countries that the region covers.

Sub-national coverage
~~~~~~~~~~~~~~~~~~~~~

If this list **only** covers one or more sub-national territories, select these.  

(If the schema does not include the required `ISO 3166-2 Subdivision Assigned Codes <https://en.wikipedia.org/wiki/ISO_3166-2#Format>`_, `open a GitHub issue to request these are added <https://github.com/org-id/register/issues/new?title=SCHEMA:%20Geographic%20subdivision%20codes%20for%20[country]&body=>`_)


Legal structure
~~~~~~~~~~~~~~~

Select all the legal structures which this list covers.

Note that legal structures are organised hierarchically in the dataset. So, for example, ‘Sole Trader’ is a kind of company. This is shown in the lookup list under the ‘Parent’ field.

Please consult the research lead if you feel you need to add an extra category to legal structures.

If the list is not specific to a particular kind of legal structure, leave this field blank.

.. hint:: **Example: GB-COH**

  UK Companies House registers a number of different kinds of company, including:

  * Public limited company (PLC)
  * Private company limited by shares (Ltd, Limited)
  * Private company limited by guarantee, typically a non-commercial  embership body such as a charity
  * Private unlimited company (either with or without a share capital)
  * Limited liability partnership (LLP)
  * Limited partnership (LP)
  * Societas Europaea (SE): European Union-wide company structure
  * Companies incorporated by Royal Charter (RC)
  * Community interest company

  It is listed against the following specific company types: Partnership,  Limited Company, Listed Company, Community Interest Company, and Charity.

  **However**, wider research tells us that whilst all Limited Companies, Listed Companies and CIC’s should have a registration in Companies House, not all charities will have a Companies House number.

Sector
~~~~~~

If this list is specific to a particular sector, you can declare that here.

If the list is not specific to a particular sector, leave this field blank.

.. hint:: **Example: GB-UKPRN**

 The UK Register of Learning Providers covers only education institutes, so has ‘Education’ set in the sector field.

List type
~~~~~~~~~

This is one of the most important fields in the dataset. You will need to determine if this list is a **primary identifier list** or whether it has secondary, third-party or local status.

Definitions of each category are provided above.

Drawing on your research into how identifiers are created, and looking at a range of example entries in the list, make your determination. You can use the comments feature in AirTable to provide supporting reasons if you require.

The following rule-of-thumb criteria may be useful.

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

Access information
~~~~~~~~~~~~~~~~~~

Available online, and online availability details
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Indicate whether this list is available online in **any form**, including only partial search.

Provide the URL that users should visit to access this list and a description of how to find identifiers.

How to locate identifiers
~~~~~~~~~~~~~~~~~~~~~~~~~

If users need to follow particular steps in order to carry out a identifier search, detail those here.

This might include:

* Guidance on how to find search features on a complex website;

* Information on charged access to identifiers if no freely available online access is provided;

* Information on how to spot the actual identifier, and how to copy it for re-use;

* Information on formatting the identifiers.


.. hint:: **Example: AU-ABN**

   It is possible to search for identifiers at http://abr.business.gov.au/

   The Australian Business Number (ABN) is a unique 11 digit identifier issued to all entities registered in the Australian Business Register (ABR). The 11 digit ABN is structured as a 9 digit identifier with two leading check digits.

   The identifiers are displayed on the website with spaces in the number. All the spaces should be removed when making use of the number within an identifier.


Example identifiers
~~~~~~~~~~~~~~~~~~~

Provide 1 - 5 example identifiers, comma separated.

.. hint:: **Example: GB-COH**

  09506232, 07444723


Access to data & Data access details
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Check for bulk downloads, and API access to the data, and indicate if these are available.

For official registers, check on the national data portal as well as the list website itself. Take note of whether the available data appears to be regularly updated, or only a one-off data dump.

Write brief notes on how the data can be accessed.

Confirm the license information for the data.

Data features
~~~~~~~~~~~~~

Select all the features that are apply to **either** of information available through the list’s website, or in APIs or bulk data products.

The goal here is to be aware of all the possible additional available information that could be explored to disambiguate organisations, whether that is available as structured data or not.

Openly licensed and license details
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Look for a license for the contents of the list.

Indicate whether or not an open license can be found, and provide the name of the license (if common) or a short description of the license if it is not a common license.

Wikipedia page
~~~~~~~~~~~~~~

If you have found a wikipedia page for the organisation, link to that here.

In OpenCorporates?
~~~~~~~~~~~~~~~~~~

If OpenCorporates has data for this list, include a link to the open corporates page here.

Languages supported
~~~~~~~~~~~~~~~~~~~

Using ISO e-digit language codes, indicate which languages this list is available in.



Last updated
~~~~~~~~~~~~

Make sure the last updated date reflects the current date.

Confirmed
~~~~~~~~~

The confirmed flag should be set once this list entry has been reviewed and accepted.
