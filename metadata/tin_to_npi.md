# GET /v1/metadata/tin_to_npi endpoint

## Headers

- `x-api-key`: **[REQUIRED]** - API key for authorization.

## Parameters

- **tin_value** (`query`, `string`, required): No description available.

## Responses

- **200**: 200 response
  - Schema: `tinToNpi`


{% swagger src="./api-datalake-prod-oas30.json" path="/v1/metadata/tin_to_npi" method="get" %}
  headers:
    x-api-key: [REQUIRED]
{% endswagger %}
