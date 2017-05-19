# <a name="sharepointids-resource-type"></a>Тип ресурса SharePointIds

Ресурс **SharePointIds** — это единая структура, объединяющая различные идентификаторы элемента, хранящегося на сайте SharePoint или в OneDrive для бизнеса.

**Примечание.** Элементы, возвращаемые из личного хранилища OneDrive, не включают аспект **SharePointIds**.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "listId", "listItemId", "listItemUniqueId", "siteId", "siteUrl", "webId" ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->

```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "siteUrl": "url",
    "webId": "string"
}
```

## <a name="properties"></a>Свойства

| Свойство         | Тип         | Описание                                                                                  |
| :--------------- | :----------- | :------------------------------------------------------------------------------------------- |
| listId           | string       | Уникальный идентификатор (GUID) списка, содержащего элемент, в SharePoint.                              |
| listItemId       | string       | Целочисленный идентификатор элемента в списке.                               |
| listItemUniqueId | string       | Уникальный идентификатор (GUID) элемента в OneDrive для бизнеса или на сайте SharePoint. |
| siteId           | string       | Уникальный идентификатор (GUID) семейства веб-сайтов (SPSite), содержащего элемент.                        |
| siteUrl          | string (url) | URL-адрес SharePoint для сайта, содержащего элемент.                                      |
| webId            | string       | Уникальный идентификатор (GUID) семейства веб-сайтов (SPWeb), содержащего элемент.                                    |

## <a name="remarks"></a>Заметки

Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharepointIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
