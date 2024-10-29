# V1 - Metadata

The **Payerset Metadata API** allows users to retrieve detailed metadata on healthcare providers and billing codes. This endpoint is essential for applications that require accurate and up-to-date information on healthcare providers, taxonomies, billing classifications, and other key reference data used in healthcare.

## Overview

This API endpoint focuses on providing metadata related to:
- **Providers**: Information such as NPI, organization details, taxonomy classifications, and geographic information.
- **Billing Codes**: Details about specific billing codes, including descriptions, categories, and applicable specialties.

### Endpoint

The base URL for the Metadata API is: https://api.payerset.com/v1/metadata


### Authentication

All requests to the Metadata API require an API key. Include your API key in the `x-api-key` header:

`x-api-key: YOUR_API_KEY`


## Key Metadata Endpoints

### `/v1/metadata/npi_detail`
Retrieve detailed metadata on a healthcare provider using the **National Provider Identifier (NPI)**. This endpoint provides comprehensive provider details, including:
- **Taxonomy**: Classification and specialization.
- **Organization**: Name, geographic location, and Medicare enrollment data.
- **Location**: State, city, and county.

#### Query Parameters
- `npi` (required): The National Provider Identifier for the provider you are querying.

#### Sample Request
```javascript
const response = await fetch('https://api.payerset.com/v1/metadata/npi_detail?npi=1730596248', {
    method: 'GET',
    headers: {
      "x-api-key": "YOUR_API_KEY"
    },
});
const data = await response.json();
```

---

### `/v1/metadata/billing_code`
Retrieve metadata associated with a specific billing code. This includes descriptions, category, and subcategory, helping you understand the type of services associated with the code.

#### Query Parameters
- `billing_code` (required): The billing code for the service (e.g., “27447”).
- `code_type` (optional): Type of code (e.g., “CPT” or “MS-DRG”) to specify the code standard.

#### Sample Request
```javascript
const response = await fetch('https://api.payerset.com/v1/metadata/billing_code?billing_code=470&code_type=MS-DRG', {
    method: 'GET',
    headers: {
      "x-api-key": "YOUR_API_KEY"
    },
});
const data = await response.json();
```

## Example Responses

### NPI Detail Response
```json
{
    "items": [
        {
            "npi": "1730596248",
            "taxonomygrouping": "Eye and Vision Services Providers",
            "taxonomyclassification": "Optometrist",
            "organizationname": "EYECARE SPECIALTIES OF MISSOURI LLC",
            "state": "MO",
            "city": "WARRENSBURG",
            "zip": "64093",
            "county": "JOHNSON"
        }
    ]
}
```

### Billing Code Response
```json
{
    "items": [
        {
            "billing_code": "470",
            "name": "(MDC 08) Major hip and knee joint replacement or reattachment of lower extremity without MCC",
            "code_type": "MS-DRG",
            "category": "Surgeries & Procedures",
            "subcategory": "Orthopedic Surgery"
        }
    ]
}
```
