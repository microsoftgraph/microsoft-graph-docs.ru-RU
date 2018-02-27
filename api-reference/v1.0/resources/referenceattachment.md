# <a name="referenceattachment-resource-type"></a>Тип ресурса referenceAttachment

Ссылка на файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или в других поддерживаемых местах хранения, вложенный в событие, сообщение или запись.

Производный от типа [attachment](attachment.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Get](../api/attachment_get.md) | [referenceAttachment](referenceattachment.md) |Чтение свойств и связей объекта referenceAttachment.|
|[Delete](../api/attachment_delete.md) | Нет |Удаление объекта referenceAttachment. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contentType|String|Тип контента этого вложения.|
|id|String|Идентификатор вложения.  Только для чтения.|
|isInline|Boolean|Значение true указывает, что вложение встроено в содержимое объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения вложения. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|имя|String|Текст, который отображается под значком, представляет внедренное вложение. Он может не быть фактическим именем файла.|
|size|Int32|Объем метаданных, которые хранятся в сообщении с вложением (в байтах). Это значение не отображает фактический размер файла.|

## <a name="relationships"></a>Связи
Нет



## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
