# Rates API Endpoints

## `GET /v1/rates`

**Description**: No summary available.

**Endpoint**: `/v1/rates`

**Method**: `GET`

### Authorization

This endpoint requires an `x-api-key` header.

### Query Parameters

- **billing_code** (query, string, Required: Yes): No description available.
- **payer** (query, string, Required: Yes): No description available.
- **npi** (query, string, Required: Yes): No description available.

### Sample Request

```javascript
const response = await fetch('https://api.payerset.com/v1/rates', {
    method: 'GET',
    headers: {
      'x-api-key': '<YOUR_API_KEY>'
    }
});
const data = await response.json();
```

### Response

**Status Code**: 200

**Description**: 200 response

**Schema**:

```json
{
  "title": "Empty Schema",
  "type": "object"
}
```

---

