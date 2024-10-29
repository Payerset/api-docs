# GET /v1/metadata/npi_to_tin endpoint

## Headers

- `x-api-key`: **[REQUIRED]** - API key for authorization.

## Parameters

- **npi** (`query`, `string`, required): No description available.

## Responses

- **200**: 200 response
  - Schema: `npiToTin`


{% swagger src="api-datalake-prod-oas30.json" path="/v1/metadata/npi_to_tin" method="get" %}
  headers:
    x-api-key: [REQUIRED]
{% endswagger %}

