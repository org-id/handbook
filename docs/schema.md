# List Schema

Entries in the org-id.guide platform MUST be provided as JSON data following the latest version of the list schema, [available here](https://raw.githubusercontent.com/org-id/register/master/schema/list-schema.json). 

The schema structure is documented below. More details on how to populate schema elements are found in the [research guidance](research.md)

### Additional schema information

The schema is [compiled from a number of source files](https://github.com/org-id/register/tree/master/schema) that contain codelists embedded within the schema. These codelist files also contain weighting used to calculate quality scores. 

The schema includes some additional properties to aid interface creation:

* [Property ordering](https://github.com/jdorn/json-editor#property-ordering)
* [enum_titles](https://github.com/jdorn/json-editor#editor-options) - a list matching the order of an enum list to provide titles for elements. 

### Schema overview

```eval_rst
.. jsonschema:: assets/list-schema.json
    :include: 
    :collapse: 
```

