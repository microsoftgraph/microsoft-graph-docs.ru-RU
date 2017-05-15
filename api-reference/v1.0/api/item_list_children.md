# <a name="list-children-of-a-driveitem"></a>Список дочерних элементов ресурса driveItem.

Возвращает коллекцию [DriveItems](../resources/driveitem.md) в **дочерние** элементы ресурса DriveItem.

Ресурсы DriveItem с аспектом **папки** или **пакета**, не равным NULL, могут содержать один или несколько дочерних элементов DriveItems.


## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из указанных **областей**:

  * Files.Read
  * Files.ReadWrite

## <a name="http-request"></a>HTTP-запрос
```http
GET /me/drive/root/children
GET /me/drive/items/{item-id}/children
GET /me/drive/root:/{item-path}:/children
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/root/children
GET /groups/{group-id}/drive/items/{item-id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Тип   | Описание                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | String | Если указан заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то возвращается отклик `HTTP 304 Not Modified`. |

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос
Вот пример запроса на возвращение DriveItems в корневую папку OneDrive текущего пользователя.

<!-- {
  "blockType": "request",
  "name": "get_children"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children
```

## <a name="response"></a>Отклик

Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048, "file": {} },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ],
  "@odata.nextLink": "https://..."
}
```

**Примечание.** Если коллекция превышает размер страницы по умолчанию (200 элементов), свойство **@odata.nextLink** возвращается в отклике, чтобы указать доступность дополнительных элементов и предоставить запрашиваемый URL-адрес для следующей страницы элементов.

Вы можете управлять размером страницы с помощью [необязательных параметров строки запроса](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "OneDrive/DriveItem/List children"
} -->
