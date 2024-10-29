# GET /v1/metadata/npi_to_parent endpoint

## Headers

- `x-api-key`: **[REQUIRED]** - API key for authorization.

## Parameters

- **npi** (`query`, `string`, required): No description available.
- **x-api-key** (`header`, `string`, required): API key for authorization

## Responses

- **200**: 200 response
  - Schema: `npiToParent`


{% swagger src="../api-datalake-prod-oas30.json" path="/v1/metadata/npi_to_parent" method="get" %}
{% endswagger %}

