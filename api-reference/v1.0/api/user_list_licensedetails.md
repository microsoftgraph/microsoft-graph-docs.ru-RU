# <a name="list-licensedetails"></a>Перечисление licenseDetails

Получение списка объектов licenseDetails.

### <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из следующих **областей**: *User.Read*, *User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All или Directory.AccessAsUser.All*.

### <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
### <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод **не** поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters).

### <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Authorization  | Bearer &lt;code&gt;|

### <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.
### <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [licenseDetails](../resources/licensedetails.md) в теле отклика.
### <a name="example"></a>Пример
##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
##### <a name="response"></a>Отклик
Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "value": [
    {
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->