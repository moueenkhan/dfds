
# Order

## Structure

`Order`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `Long` | Optional | - | Long getId() | setId(Long id) |
| `PetId` | `Long` | Optional | - | Long getPetId() | setPetId(Long petId) |
| `Quantity` | `Integer` | Optional | - | Integer getQuantity() | setQuantity(Integer quantity) |
| `ShipDate` | `LocalDateTime` | Optional | - | LocalDateTime getShipDate() | setShipDate(LocalDateTime shipDate) |
| `Status` | [`Status1Enum`](../../doc/models/status-1-enum.md) | Optional | Order Status | Status1Enum getStatus() | setStatus(Status1Enum status) |
| `Complete` | `Boolean` | Optional | - | Boolean getComplete() | setComplete(Boolean complete) |

## Example (as JSON)

```json
{
  "id": null,
  "petId": null,
  "quantity": null,
  "shipDate": null,
  "status": null,
  "complete": null
}
```

