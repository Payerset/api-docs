# GET /v1/metadata/billing_code endpoint

## Headers

- `x-api-key`: **[REQUIRED]** - API key for authorization.

## Parameters

- **billing_code** (`query`, `string`, required): No description available.
- **code_type** (`query`, `string`, required): No description available.
- **x-api-key** (`header`, `string`, required): API key for authorization

## Responses

- **200**: 200 response

{% swagger src="../api-datalake-prod-oas30.json" path="/v1/metadata/billing_code" method="get" %}
{% endswagger %}

