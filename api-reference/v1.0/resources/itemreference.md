# <a name="itemreference-resource-type"></a>Тип ресурса ItemReference

Ресурс **ItemReference** предоставляет сведения, необходимые для обращения к ресурсу [DriveItem](driveitem.md) через API.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "id": "string",
  "path": "string"
}
```

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание                                                                   |
|:---------|:-------|:------------------------------------------------------------------------------|
| driveId  | Строка | Уникальный идентификатор экземпляра OneDrive, содержащего элемент. Только для чтения. |
| id       | String | Уникальный идентификатор элемента на диске. Только для чтения.            |
| путь     | String | Путь, по которому можно перейти к элементу. Только для чтения.                     |


## <a name="remarks"></a>Заметки

Чтобы обратиться к элементу из ресурса **ItemReference**, составьте URL-адрес в следующем формате:

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

Значение **path** — это путь к API относительно целевого диска, например: `/drive/root:/Documents/myfile.docx`.

Чтобы получить удобочитаемый путь для навигации, вы можете пропустить все до первого символа `:` в строке пути.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
