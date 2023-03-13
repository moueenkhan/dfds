
# Pet

## Structure

`Pet`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `Long` | Optional | - | Long getId() | setId(Long id) |
| `Category` | [`Category`](../../doc/models/category.md) | Optional | - | Category getCategory() | setCategory(Category category) |
| `Name` | `String` | Required | - | String getName() | setName(String name) |
| `PhotoUrls` | `List<String>` | Required | - | List<String> getPhotoUrls() | setPhotoUrls(List<String> photoUrls) |
| `Tags` | [`List<Tag>`](../../doc/models/tag.md) | Optional | - | List<Tag> getTags() | setTags(List<Tag> tags) |
| `Status` | [`StatusEnum`](../../doc/models/status-enum.md) | Optional | pet status in the store | StatusEnum getStatus() | setStatus(StatusEnum status) |

## Example (as JSON)

```json
{
  "id": null,
  "category": null,
  "name": "name0",
  "photoUrls": [
    "photoUrls5",
    "photoUrls6",
    "photoUrls7"
  ],
  "tags": null,
  "status": null
}
```

