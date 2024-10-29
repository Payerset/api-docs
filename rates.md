# Rates API Endpoints

{% swagger src="api-datalake-prod-oas30.json" path="/v1/rates" method="get" %}
No description available.

  headers:
    x-api-key: [REQUIRED]
  parameters:
    - name: billing_code
      in: query
      required: True
      schema:
        type: string
      description: No description available.
    - name: payer
      in: query
      required: True
      schema:
        type: string
      description: No description available.
    - name: npi
      in: query
      required: True
      schema:
        type: string
      description: No description available.
  responses:
    200:
      description: 200 response
{% endswagger %}

