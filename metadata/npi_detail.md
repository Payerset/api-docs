# GET /v1/metadata/npi_detail endpoint

## Headers

- `x-api-key`: **[REQUIRED]** - API key for authorization.

## Parameters

- **npi** (`query`, `string`, required): No description available.
- **x-api-key** (`header`, `string`, required): API key for authorization

## Responses

- **200**: 200 response
  - Schema: `npiDetail`


{% swagger src="../api-datalake-prod-oas30.json" path="/v1/metadata/npi_detail" method="get" %}
{% endswagger %}

