# <a name="delete-permission"></a>Удаление разрешения

Отмена доступа к ресурсу [DriveItem](../resources/driveitem.md).

Удалять можно только те разрешения, которые не были унаследованы. Свойство **inheritedFrom** должно иметь значение `null`.

## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуется одна из указанных **областей**:

  * Files.ReadWrite

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/root:/{path}:/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Тип   | Описание                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-match      | string | Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется. |

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "delete_permission"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/root/items/{item-id}/permissions/{perm-id}
```

##### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a>Заметки

* [Диски](../resources/drive.md), у которых для свойства **driveType** задано значение `personal` (личное хранилище OneDrive), не могут создавать и изменять разрешения в корневом ресурсе DriveItem. 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission"
}-->
