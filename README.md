# Hotelzify - Wego APIs

### Static API:
- Endpoint: <b> POST </b> `https://dev2-api.hotelzify.com/api/hotel/meta-search/v1/wego/on-demand/static-data`
- Request body:
```
curl --location 'https://dev2-api.hotelzify.com/hotel/meta-search/v1/wego/on-demand/static-data' \
--header 'Content-Type: application/json' \
--data '{
    "id": 10,
    "ln": "en"
}'
```

### Pricing and Inventory (ARI) API:
- Endpoint: <b> POST </b> `https://dev2-api.hotelzify.com/api/hotel/meta-search/v1/wego/on-demand/static-data](https://dev2-api.hotelzify.com/api/hotel/meta-search/v1/wego/on-demand/search`
- Request body:
```
curl --location 'https://dev2-api.hotelzify.com/hotel/meta-search/v1/wego/on-demand/search' \
--header 'Content-Type: application/json' \
--data '{
  "hotelIds": [10, 392],
  "checkInDate": "2024-08-10",
  "checkOutDate": "2024-08-12",
  "rooms": 2,
  "adults": 1,
  "children": 0,
  "infants": 0
}'
```
