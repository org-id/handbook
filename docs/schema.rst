List Schema
===========

Entries in the org-id.guide platform MUST be provided as JSON data following the latest version of the list schema, `available here <https://raw.githubusercontent.com/org-id/register/main/schema/list-schema.json>`_.

The schema structure is documented below. More details on how to populate schema elements are found in the :doc:`research guidance <research>`

Additional schema information
-----------------------------

The schema is `compiled from a number of source files <https://github.com/org-id/register/tree/master/schema>`_ that contain codelists embedded within the schema. These codelist files also contain weighting used to calculate quality scores.

The schema includes some additional properties to aid interface creation:

* `Property ordering <https://github.com/jdorn/json-editor#property-ordering>`_
* `enum_titles <https://github.com/jdorn/json-editor#editor-options>`_ - a list matching the order of an enum list to provide titles for elements.

Schema overview
---------------

.. jsonschema:: assets/list-schema.json
    :include: 
    :collapse: 


