# <a name="shareddriveitem-resource-type"></a>Тип ресурса SharedDriveItem

Ресурс **sharedDriveItem** возвращается, если для доступа к общему элементу [driveItem](driveitem.md) используется API [Shares](../api/shares_get.md).

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса **sharedDriveItem** в формате JSON.

Ресурс **sharedDriveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
    "id": "string",
    "name": "string",
    "owner": { "@odata.type": "microsoft.graph.identitySet" },

    /* relationships*/
    "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
    "root": { "@odata.type": "microsoft.graph.driveItem" },
    "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
    "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a>Свойства

| Свойство | Тип                          | Описание                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| id       | Строка                        | Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.              |
| name     | Строка                        | Отображаемое имя общего элемента.                             |
| owner    | [IdentitySet](identityset.md) | Сведения о владельце общего элемента, ставшего объектом ссылки. |

## <a name="relationships"></a>Связи

| Связь | Тип                                  | Описание                                                                                                                                                                                                |
| :----------- | :------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| элементы        | Коллекция ([DriveItem](driveitem.md)) | Коллекция общих ресурсов **driveItem**. Эту коллекцию невозможно перечислить, но вы можете получить доступ к элементам по их уникальным идентификаторам.                                                                        |
| root         | [DriveItem](driveitem.md)             | Общий элемент **driveItem** верхнего уровня. Если предоставлен общий доступ к одному файлу, этот элемент будет файлом. Если предоставлен общий доступ к папке, этот элемент будет папкой. Определить, какой вариант используется, можно с помощью аспектов элемента. |
| driveItem    | [driveItem](driveitem.md)             | Элемент **driveItem** для ресурса, к которому предоставлен общий доступ.  Совпадает со свойством **root**.                                                                                                             |
| site         | [site](site.md)                       | Ресурс **site** с элементом, к которому предоставлен общий доступ.                                                                                                                                                |

## <a name="methods"></a>Методы

| Метод                                  | Путь REST                |
| :-------------------------------------- | :----------------------- |
| [Получение общего элемента](../api/shares_get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a>Заметки

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharepointIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->