# Metadata API Endpoints

{% swagger src="api-datalake-prod-oas30.json" path="/v1/metadata/npi_to_parent" method="get" %}
No description available.

  headers:
    x-api-key: [REQUIRED]
  parameters:
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

{% swagger src="api-datalake-prod-oas30.json" path="/v1/metadata/billing_code" method="get" %}
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
    - name: code_type
      in: query
      required: True
      schema:
        type: string
      description: No description available.
  responses:
    200:
      description: 200 response
{% endswagger %}

{% swagger src="api-datalake-prod-oas30.json" path="/v1/metadata/npi_detail" method="get" %}
No description available.

  headers:
    x-api-key: [REQUIRED]
  parameters:
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

{% swagger src="api-datalake-prod-oas30.json" path="/v1/metadata/tin_to_npi" method="get" %}
No description available.

  headers:
    x-api-key: [REQUIRED]
  parameters:
    - name: tin_value
      in: query
      required: True
      schema:
        type: string
      description: No description available.
  responses:
    200:
      description: 200 response
{% endswagger %}

{% swagger src="api-datalake-prod-oas30.json" path="/v1/metadata/npi_to_tin" method="get" %}
No description available.

  headers:
    x-api-key: [REQUIRED]
  parameters:
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

{% swagger src="api-datalake-prod-oas30.json" path="/v1/metadata/npi_parent" method="get" %}
No description available.

  headers:
    x-api-key: [REQUIRED]
  parameters:
    - name: npi_parent
      in: query
      required: True
      schema:
        type: string
      description: No description available.
  responses:
    200:
      description: 200 response
{% endswagger %}

