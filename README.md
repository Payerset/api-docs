# Payerset API Documentation

Welcome to the **Payerset API** documentation. This API provides a comprehensive solution for accessing healthcare data, including provider and billing code metadata, healthcare rates, and other critical reference information that supports data transparency and price comparison for health services.

## Overview

Payerset’s API is designed to facilitate streamlined access to healthcare-related data. It’s built with a focus on **price transparency**, **rate benchmarking**, and **contract negotiation** across healthcare services. The API enables healthcare consulting firms, insurance companies, and other stakeholders to retrieve and leverage various data points efficiently.

### Key Capabilities
- **Provider Metadata**: Access detailed information about healthcare providers, including National Provider Identifier (NPI) details, organization names, taxonomies, geographic data, and Medicare-specific classifications.
- **Billing Codes**: Retrieve metadata associated with healthcare billing codes (e.g., CPT codes) including code descriptions, categories, and specialties.
- **Healthcare Rates**: Retrieve negotiated healthcare rates by provider, payer, and billing code, supporting use cases in benchmarking and price transparency efforts.

## Base URL
The API is hosted at:
https://api.payerset.com/v1/

vbnet
Copy code

### Authentication
This API requires an API key for authentication. Include your API key in the `x-api-key` header with every request:
`x-api-key: YOUR_API_KEY`

## Key Endpoints

### Provider Metadata
#### `/v1/metadata/npi_detail`
Get detailed metadata about a provider based on NPI.

#### `/v1/metadata/billing_code`
Retrieve metadata about specific billing codes, including category, subcategory, and description.

### Healthcare Rates
#### `/v1/rates`
Retrieve negotiated rates for healthcare services based on provider NPI, payer, and billing code. Each response includes the negotiated rate, billing code details, billing class, and service codes.

## Usage Example

### Fetching Rates

#### Endpoint
`GET /v1/rates`

#### Query Parameters
npi (required): National Provider Identifier.
payer (required): Name of the payer (e.g., “Aetna”).
billing_code (required): Billing code of the service (e.g., “27447” for Total Knee Arthroplasty).

#### Sample Request
```javascript
const response = await fetch('https://api.payerset.com/v1/rates?npi=1003936113&payer=aetna&billing_code=27447', {
    method: 'GET',
    headers: {
      "x-api-key": "YOUR_API_KEY"
    },
});
const data = await response.json();
```

### Additional Resources
For comprehensive usage guidelines, examples, and parameter details, visit the full documentation at:
https://api-docs.payerset.com

## Contact Us
If you have any questions or need assistance, please reach out to our support team at support@payerset.com.

Ths API documentation is a part of Payerset’s commitment to advancing healthcare price transparency and supporting data-driven decisions across the industry.
