# GET /v1/rates endpoint

## Headers

- `x-api-key`: **[REQUIRED]** - API key for authorization.

## Parameters

- **billing_code** (`query`, `string`, required): No description available.
- **payer** (`query`, `string`, required): No description available.
- **npi** (`query`, `string`, required): No description available.

## Responses

- **200**: 200 response
  - Schema: `Empty`


{% swagger src="../api-datalake-prod-oas30.json" path="/v1/rates" method="get" %}
  headers:
    x-api-key: [REQUIRED]
{% endswagger %}

