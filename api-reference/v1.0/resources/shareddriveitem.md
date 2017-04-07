# <a name="shareddriveitem-resource-type"></a>Тип ресурса SharedDriveItem

Ресурс **SharedDriveItem** возвращается, если для доступа к общему элементу [DriveItem](driveitem.md) используется API [Shares](../api/shares_get.md). Этот ресурс похож на ресурс [Drive](drive.md), но его область ограничена только элементами DriveItem, доступ к которым можно получить с помощью ссылки для совместного доступа или идентификатора shareId.

### <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

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
    "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
    "root": { "@odata.type": "microsoft.graph.driveItem" }
}
```

### <a name="properties"></a>Свойства

| Свойство  | Тип                                  | Описание                                                          |
|:----------|:--------------------------------------|:---------------------------------------------------------------------|
| id        | Строка                                | Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.                  |
| name      | Строка                                | Отображаемое имя общего элемента.                                 |
| owner     | [IdentitySet](identityset.md)         | Сведения о владельце общего элемента, ставшего объектом ссылки.     |
| items     | Collection([DriveItem](driveitem.md)) | Коллекция общих ресурсов DriveItem. Вам не удастся выполнить перечисление этой коллекции, но вы можете получить доступ к элементам по их уникальным идентификаторам. |
| root      | [DriveItem](driveitem.md)             | Общий элемент DriveItem верхнего уровня. Если предоставлен общий доступ к одному файлу, этот элемент будет файлом. Если предоставлен общий доступ к папке, этот элемент будет папкой. Чтобы определить, какой вариант используется, вы можете применять аспекты элемента. |

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