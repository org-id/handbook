# Assigning a prefix

Each **organisation list** prefix is made up of two parts: a jurisdiction code, and a list code.

##### 1) Jurisdiction code

For any list which contains entries only from a given country, the ISO 2-digit country code should be used.

For lists that contain entries from multiple countries, one of the following codes should be used (NOTE:  We rely here on the fact that in ISO 3166-1 the following alpha-2 codes can be user-assigned: AA, QM to QZ, XA to XZ, and ZZ. We avoid any widely used X codes. ).

```eval_rst
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
```


### 2) List code

The list code is manually assigned. In general, list codes have been designed so that:

1. They are between 2 and 7 characters long;

2. They use a recognisable acronym or contraction of the name of the organisation list;

3. Acronyms should be based on the local language version of the name (NOTE:  It is not clear how far this principle has been followed in the past. );

4. Codes should be memorable, allowing users to become familiar with codes.

However, there is no intention that the list code portion of the prefix will carry any semantics (e.g. type of organisations listed etc.).

Points 1 - 4 are guidance only. Breaking any of these principles shall not be grounds for revision of an existing code.

When a new organisation list is identified, the creator/proposer may suggest a list code.

There will be a short window for proposed prefixes to be reviewed before they are confirmed.

To confirm a code, the researcher should check:

* The proposed list code is based on a clear understanding of the name of the underlying **organisation list** or list provider.

* Any requirements for multi-lingual codes. For example, in Canada, acronyms should always be given in both their English and French forms. This is achieved using an underscore separator in the list code. E.g.

CA-CRA_ACR for the Canadian Revenue Agency / Agence du revenu du Canada

* The code does not duplicate an existing code, or AKA value.

If a list code is later replaced, the full deprecated prefix should be recorded in the **AKA** field. This will allow systems to warn about deprecated prefixes and to notify users of their replacements.
