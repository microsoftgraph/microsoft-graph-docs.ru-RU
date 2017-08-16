# <a name="update-driveitem-properties"></a>Обновление свойств DriveItem

Обновление метаданных ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути.

Путем обновления также можно [переместить элемент](item_move.md) в другой родительский объект, изменив значение свойства **parentReference**.

## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуется одна из указанных **областей**:

* Files.ReadWrite.
* Files.ReadWrite.All
* Sites.ReadWrite.All

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Тип   | Описание                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-match      | String | Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом eTag папки, то возвращается отклик `412 Precondition Failed`. |

## <a name="request-body"></a>Текст запроса
Укажите в тексте запроса значения обновляемых свойств. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств. Для достижения максимальной оптимальной производительности в приложении не следует указывать свойства, которые не были изменены.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.

## <a name="example"></a>Пример
В этом примере переименовывается ресурс driveItem.

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-file-name.docx"
}
```

##### <a name="response"></a>Отклик

Ниже приводится пример отклика. Для наглядности этот отклик сокращен.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
    "name": "new-file-name.docx",
    "file": { }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update item"
}-->
