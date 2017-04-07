# <a name="sharepointids-resource-type"></a>Тип ресурса SharePointIds

Ресурс **SharePointIds** — это единая структура, объединяющая различные идентификаторы элемента, хранящегося на сайте SharePoint или в OneDrive для бизнеса.

**Примечание.** Элементы, возвращаемые из личного хранилища OneDrive, не включают аспект **SharePointIds**.

### <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->
```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "webId": "string"
}
```

### <a name="properties"></a>Свойства

| Свойство          | Тип    | Описание                                                          |
|:------------------|:--------|:---------------------------------------------------------------------|
| listId            | string  | Уникальный идентификатор списка элементов в SharePoint.                          |
| listItemId        | string  | Целочисленный идентификатор элемента в списке.                    |
| listItemUniqueId  | string  | Уникальный идентификатор элемента в OneDrive для бизнеса или на сайте SharePoint. |
| siteId            | string  | Уникальный идентификатор семейства веб-сайтов, в котором хранится элемент. |
| webId             | string  | Уникальный идентификатор сайта, на котором хранится элемент.                          |

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
