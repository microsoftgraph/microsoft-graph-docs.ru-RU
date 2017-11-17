# <a name="folder-resource-type"></a>Тип ресурса Folder

Ресурс **Folder** — это единая структура, объединяющая данные элемента, связанные с папками. Ресурсы [**DriveItem**](driveitem.md) с ненулевым аспектом **folder** являются контейнерами для других ресурсов DriveItem.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.folder"
}-->

```json
{
  "childCount": 1024
}
```

## <a name="properties"></a>Свойства

| Свойство       | Тип  | Описание                                                     |
|:---------------|:------|:----------------------------------------------------------------|
| **childCount** | Int64 | Количество дочерних объектов в корне данного контейнера. |

## <a name="remarks"></a>Заметки 

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
