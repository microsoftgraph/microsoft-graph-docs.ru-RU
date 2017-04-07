# <a name="get-device"></a>Получение устройства

Получение свойств и связей объекта устройства.
## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуется одна из указанных ниже **областей**. *Directory.Read.All*, *Directory.ReadWrite.All*, *Directory.AccessAsUser.All* или *Device.ReadWrite.All*

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | строка  | Bearer <token>. Обязательный параметр. |

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.
## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200 OK` и объект [device](../resources/device.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type": 2,
      "key":"Y3YxN2E1MWFlYw==",
      "identityProvider": null
    }
  ],
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "id": "id-value",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
