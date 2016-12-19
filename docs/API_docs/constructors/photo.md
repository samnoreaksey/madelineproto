## Constructor: photo  

### Attributes:

| Name     |    Type       | Required |
|----------|:-------------:|---------:|
|has\_stickers|[Bool](../types/Bool.md) | Optional|
|id|[long](../types/long.md) | Required|
|access\_hash|[long](../types/long.md) | Required|
|date|[int](../types/int.md) | Required|
|sizes|Array of [PhotoSize](../types/PhotoSize.md) | Required|


### Type: [Photo](../types/Photo.md)

### Example:


```
$photo = ['has_stickers' => Bool, 'id' => long, 'access_hash' => long, 'date' => int, 'sizes' => [PhotoSize], ];
```