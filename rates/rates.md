# GET /v1/rates endpoint

## Headers

- `x-api-key`: **[REQUIRED]** - API key for authorization.

## Parameters

- **billing_code** (`query`, `string`, required): No description available.
- **payer** (`query`, `string`, required): No description available.
- **npi** (`query`, `string`, required): No description available.
- **x-api-key** (`header`, `string`, required): API key for authorization

## Responses

- **200**: 200 response
  - Schema: `Empty`


{% swagger src="../api-datalake-prod-oas30.json" path="/v1/rates" method="get" %}
{% endswagger %}

