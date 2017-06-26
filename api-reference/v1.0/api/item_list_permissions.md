# <a name="list-permissions-on-a-driveitem"></a>Создание списка разрешений для доступа к ресурсу DriveItem

Создание списка действующих разрешений для доступа к ресурсу [DriveItem](../resources/driveitem.md).

Связи между **разрешениями** ресурса DriveItem невозможно развернуть как часть запроса на [получение DriveItem](item_get.md) или коллекции DriveItems. Необходимо открыть доступ непосредственно к свойству разрешений.

## <a name="access-to-permissions"></a>Доступ к разрешениям

Коллекция разрешений включает потенциально конфиденциальные данные и может быть недоступна для каждого абонента.

* Все разрешения будут возвращены владельцу элемента. Включает совладельцев.
* Абоненту, который не является владельцем, возвращаются только применяемые к нему разрешения.
* Свойства разрешений, которые содержат секретную информацию (например, `shareId` и `webUrl`) возвращаются только абонентам, которые могут создать разрешение.

## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из указанных **областей**:

* Files.Read
* Files.ReadWrite.
* Files.Read.All
* Files.ReadWrite.All
* Sites.Read.All
* Sites.ReadWrite.All

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Тип   | Описание                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | string | Если указан заголовок запроса, а предоставленный тег etag совпадает с текущим тегом etag элемента, то возвращается отклик `HTTP 304 Not Modified`. |


## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию ресурсов [Permission](../resources/permission.md) в тексте отклика.

Действующие разрешения элемента могут поступать из двух источников:

* разрешения, которые были применены непосредственно к самому элементу;
* разрешения, унаследованные от предшествующих элементов.

Абоненты могут распознать унаследованное разрешение, проверив свойство **inheritedFrom**. Это свойство — ресурс [**itemReference**](../resources/itemreference.md), отсылающий к предшествующему элементу, от которого унаследовано разрешение.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_permissions"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions
```


##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "TimeTravelPlus"
        }
      }
    }
  ]
}
```

Дополнительные сведения о том, как получить единый ресурс разрешения см. в статье [Получение разрешения](permission_get.md).


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List permissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List permissions"
}-->
