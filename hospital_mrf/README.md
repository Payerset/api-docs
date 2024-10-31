# V1 - Hospital MRF

The **Payerset Hospital MRF API** allows users to retrieve detailed metadata on healthcare providers and billing codes. This endpoint is essential for applications that require accurate and up-to-date information on healthcare providers, taxonomies, billing classifications, and other key reference data used in healthcare.

## Overview

This API endpoint focuses on providing metadata related to the Hospital Machine-Readable Files (MRF) dataset. The Hospital MRF dataset contains detailed information about hospitals, including hospital names, locations, and unique identifiers.

### Endpoint

The base URL for the Metadata API is: https://api.payerset.com/v1/hospital_mrf


### Authentication

All requests to the Metadata API require an API key. Include your API key in the `x-api-key` header:

`x-api-key: YOUR_API_KEY`


## Key Metadata Endpoints

### `/v1/hospital_mrf/hospital_list`
Retrieve a list of all hospitals in the Payerset Data Lake. This endpoint will provide the System name, Hospital Name, and Hospital ID, which is used to query other endpoints.


#### Query Parameters
- No query parameters are required for this endpoint.

#### Sample Request
```javascript
const response = await fetch('https://api.payerset.com/v1/hospital_mrf/hospital_list', {
    method: 'GET',
    headers: {
      "x-api-key": "YOUR_API_KEY"
    },
});
const data = await response.json();
```