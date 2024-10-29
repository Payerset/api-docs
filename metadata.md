# Metadata API Endpoints

## `GET /v1/metadata/npi_to_parent`

**Description**: No summary available.

**Endpoint**: `/v1/metadata/npi_to_parent`

**Method**: `GET`

### Authorization

This endpoint requires an `x-api-key` header.

### Query Parameters

- **npi** (query, string, Required: Yes): No description available.

### Sample Request

```javascript
const response = await fetch('https://api.payerset.com/v1/metadata/npi_to_parent', {
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

## `GET /v1/metadata/billing_code`

**Description**: No summary available.

**Endpoint**: `/v1/metadata/billing_code`

**Method**: `GET`

### Authorization

This endpoint requires an `x-api-key` header.

### Query Parameters

- **billing_code** (query, string, Required: Yes): No description available.
- **code_type** (query, string, Required: Yes): No description available.

### Sample Request

```javascript
const response = await fetch('https://api.payerset.com/v1/metadata/billing_code', {
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

## `GET /v1/metadata/npi_detail`

**Description**: No summary available.

**Endpoint**: `/v1/metadata/npi_detail`

**Method**: `GET`

### Authorization

This endpoint requires an `x-api-key` header.

### Query Parameters

- **npi** (query, string, Required: Yes): No description available.

### Sample Request

```javascript
const response = await fetch('https://api.payerset.com/v1/metadata/npi_detail', {
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

## `GET /v1/metadata/tin_to_npi`

**Description**: No summary available.

**Endpoint**: `/v1/metadata/tin_to_npi`

**Method**: `GET`

### Authorization

This endpoint requires an `x-api-key` header.

### Query Parameters

- **tin_value** (query, string, Required: Yes): No description available.

### Sample Request

```javascript
const response = await fetch('https://api.payerset.com/v1/metadata/tin_to_npi', {
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

## `GET /v1/metadata/npi_to_tin`

**Description**: No summary available.

**Endpoint**: `/v1/metadata/npi_to_tin`

**Method**: `GET`

### Authorization

This endpoint requires an `x-api-key` header.

### Query Parameters

- **npi** (query, string, Required: Yes): No description available.

### Sample Request

```javascript
const response = await fetch('https://api.payerset.com/v1/metadata/npi_to_tin', {
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

## `GET /v1/metadata/npi_parent`

**Description**: No summary available.

**Endpoint**: `/v1/metadata/npi_parent`

**Method**: `GET`

### Authorization

This endpoint requires an `x-api-key` header.

### Query Parameters

- **npi_parent** (query, string, Required: Yes): No description available.

### Sample Request

```javascript
const response = await fetch('https://api.payerset.com/v1/metadata/npi_parent', {
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

