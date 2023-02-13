# Comparing Generated OSCAL Scheams from Java and XSLT-M4

## Methodology

- `develop` from usnistgov/OSCAL with metaschema submodule @ ``
- `oscal-cli` version `0.3.1` was used at this time with current metaschemas from `develop` branch of usnistgov/OSCAL.


## JSON Schema
- Object names for sub-schemas (i.e. xslt-M4: `oscal-complete-oscal-catalog:catalog:` vs. metaschema-java: `OscalCatalogCatalogAssemblyType`)
- XSLT-M4 schema generation prefixes the schema "strategy" as a prefix whereas metaschema-java does not (i.e. `oscal-complete-oscal-catalog:catalog:` vs. metaschema-java: `OscalCatalogCatalogAssemblyType`)
- `$ref` structures are different (i.e. in xslt-M4: `"$ref": "#/definitions/UUIDDatatype"` versus the same with metaschema-java is `"#/definitions/OscalCatalogCatalogUuidFlagType"`)

## XML Schema