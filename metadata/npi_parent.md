# GET /v1/metadata/npi_parent endpoint

## Headers

- `x-api-key`: **[REQUIRED]** - API key for authorization.

## Parameters

- **npi_parent** (`query`, `string`, required): No description available.

## Responses

- **200**: 200 response
  - Schema: `npiParent`


{% swagger src="./api-datalake-prod-oas30.json" path="/v1/metadata/npi_parent" method="get" %}
  headers:
    x-api-key: [REQUIRED]
{% endswagger %}

