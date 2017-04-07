# <a name="identityset-resource-type"></a>Тип ресурса IdentitySet

Ресурс **IdentitySet** представляет собой коллекцию ресурсов [identity](identity.md) с ключами. Он представляет набор удостоверений, связанных с различными событиями для элемента, например _созданием_ или _последним изменением_.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "user", "device", "application" ],
  "@odata.type": "microsoft.graph.identitySet"
}-->

```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a>Свойства

| Свойство    | Тип                    | Описание                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| application | [Identity](identity.md) | Необязательный. Приложение, связанное с данным действием. |
| Устройство
      | [Identity](identity.md) | Необязательный. Устройство, связанное с данным действием.      |
| ПОЛЬЗОВАТЕЛЬ        | [Identity](identity.md) | Необязательный. Пользователь, связанный с данным действием.        |

## <a name="remarks"></a>Заметки 

Сведения об использовании ресурсов **IdentitySet** см. в описании типа [DriveItem](driveitem.md).


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
