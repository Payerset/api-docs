# GET /v1/metadata/billing_codes/code_detail

## Metadata

        - **Possible Values:** `CPT`, `HCPCS`, `MS-DRG`, `RC`
        - **Description:** Possible values for the `code_type` parameter.
        - **You must include both the billing_code and code_type parameters.**

{% swagger src="../../api-datalake-prod-oas30.json" path="/v1/metadata/billing_codes/code_detail" method="get" %}
{% endswagger %}

