# V1 - Rates

The **Payerset Rates API** provides detailed information on negotiated rates for healthcare services across various providers and billing codes. This endpoint is essential for applications needing transparency into negotiated healthcare rates, enabling users to make cost-informed decisions.

## Overview

This API endpoint focuses on retrieving negotiated rate data for:
- **Healthcare Providers**: Information on the rates associated with individual providers, based on their National Provider Identifier (NPI).
- **Billing Codes**: Rates for specific healthcare services, identified by unique billing codes and their modifiers.
- **Payers**: Rates negotiated with specific insurance payers, ensuring access to payer-specific pricing.

### Endpoint

The base URL for the Rates API is: https://api.payerset.com/v1/rates

### Authentication

All requests to the Rates API require an API key. Include your API key in the `x-api-key` header:
`x-api-key: YOUR_API_KEY`


## Rates Endpoint

### `/v1/rates`
Retrieve negotiated rates for healthcare services provided by specific healthcare providers, identified by NPI and payer. The endpoint returns all associated rate information for the given criteria.

#### Query Parameters
- `npi` (required): National Provider Identifier for the healthcare provider.
- `payer` (required): Name of the insurance payer (e.g., “aetna”).
- `billing_code` (required): The billing code for the healthcare service (e.g., “27447”).

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

---

## Example Responses

### Rates Response
The response provides detailed information on the negotiated rates, including billing codes, modifiers, rate type, and arrangement.

```json
[
    {
        "npi": "1003936113",
        "tin_type": "ein",
        "tin_value": "223468528",
        "billing_code": "27447",
        "billing_code_name": "TOTAL KNEE ARTHROPLASTY",
        "billing_code_modifier": "30",
        "billing_code_type": "CPT",
        "billing_code_type_version": "2022",
        "billing_class": "professional",
        "expiration_date": "9999-12-31",
        "negotiated_rate": 30.0,
        "negotiated_type": "fee schedule",
        "service_codes": "01,02,03,04,05,06,07,08,10,11,12,13,14,15,17,18,19,20,21,22,23,24,25,26,27,31,32,33,34,41,42,49,50,51,52,53,54,55,56,57,58,60,61,62,65,71,72,81,99",
        "negotiation_arrangement": "ffs",
        "additional_information": ""
    },
    {
        "npi": "1003936113",
        "tin_type": "ein",
        "tin_value": "223468528",
        "billing_code": "27447",
        "billing_code_name": "TOTAL KNEE ARTHROPLASTY",
        "billing_code_modifier": "54",
        "billing_code_type": "CPT",
        "billing_code_type_version": "2022",
        "billing_class": "professional",
        "expiration_date": "9999-12-31",
        "negotiated_rate": 1049.18,
        "negotiated_type": "fee schedule",
        "service_codes": "01,02,03,04,05,06,07,08,10,11,12,13,14,15,17,18,19,20,21,22,23,24,25,26,27,31,32,33,34,41,42,49,50,51,52,53,54,55,56,57,58,60,61,62,65,71,72,81,99",
        "negotiation_arrangement": "ffs",
        "additional_information": ""
    }
]
```

