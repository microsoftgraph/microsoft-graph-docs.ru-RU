# <a name="list-contracts"></a>Перечисление contract

Получение списка объектов [contract](../resources/contract.md), сопоставленных с клиентом партнера.

### <a name="prerequisites"></a>Необходимые условия

Для применения этого API требуется одна из следующих **областей**: *Directory.Read.All*, *Directory.ReadWrite.All* или *Directory.AccessAsUser.All*.

### <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

### <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки отклика. 

> Для свойств customerId, defaultDomainName и displayName поддерживается фильтрация.

### <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |

### <a name="request-body"></a>Основной текст запросов

Не указывайте тело запроса для этого метода.

### <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contract](../resources/contract.md) в теле отклика.

### <a name="example"></a>Пример
##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts
```

##### <a name="response"></a>Отклик

Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
      "contractType": "contractType-value",
      "customerId": "customerId-value",
      "defaultDomainName": "defaultDomainName-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->