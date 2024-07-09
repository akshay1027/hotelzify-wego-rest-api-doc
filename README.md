# Hotelzify - Wego APIs

### 1. Static API:
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
- Payload keys and description
<table>
  <tr>
    <th>Key </th>
    <th>Description </th>
  </tr>
  <tr>
    <td>id</td>
    <td>Hotel ID | This field is mandatory </td>
  </tr>
  <tr>
    <td>ln</td>
    <td>language | This field is not mandatory | Defaults to "en" (english) </td>
  </tr>
</table>  

</br>

### 2. Pricing and Inventory (ARI) API:
- Endpoint: <b> POST </b> `https://dev2-api.hotelzify.com/api/hotel/meta-search/v1/wego/on-demand/static-data`
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
- Payload keys and description
<table>
  <tr>
    <th>Key </th>
    <th>Description </th>
  </tr>
  <tr>
    <td>hotelIds</td>
    <td>Array of Hotel IDs | This field is mandatory </td>
  </tr>
  <tr>
    <td>checkInDate</td>
    <td>Check-in date of the booking | This field is mandatory </td>
  </tr>
  <tr>
    <td>checkOutDate</td>
    <td>Check-out date of the booking | This field is mandatory </td>
  </tr>
  <tr>
    <td>rooms</td>
    <td>Total number of rooms required by the guest for the booking | This field is mandatory | Value cannot be zero </td>
  </tr>
  <tr>
    <td>adults</td>
    <td>Total number of adults required by the guest for the booking | This field is mandatory | Value cannot be zero </td>
  </tr>
  <tr>
    <td>children</td>
    <td>Total number of children required by the guest for the booking | This field is mandatory | Value can be zero </td>
  </tr>
  <tr>
    <td>infants</td>
    <td>Total number of infants required by the guest for the booking | This field is mandatory | Value can be zero </td>
  </tr>
</table>
