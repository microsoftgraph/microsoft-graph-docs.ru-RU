# <a name="get-singlevaluelegacyextendedproperty"></a>Получение объекта singleValueLegacyExtendedProperty

Получение экземпляров ресурса, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`.

С помощью параметра запроса `$expand` вы можете получить указанный экземпляр, дополненный указанным расширенным свойством. На данный момент это единственный способ получить объект [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md), представляющий расширенное свойство.

С помощью параметра запроса `$filter` вы можете получить все экземпляры указанного ресурса, которые содержат расширенное свойство, соответствующее фильтру для свойств **id** и **value**. Фильтр применяется ко всем экземплярам ресурса в почтовом ящике вошедшего пользователя.

Поддерживаются следующие ресурсы пользователей:

- [message](../resources/message.md);
- [mailFolder](../resources/mailfolder.md);
- [event](../resources/event.md);
- [calendar](../resources/calendar.md);
- [contact](../resources/contact.md);
- [contactFolder](../resources/contactfolder.md). 

Кроме того, поддерживаются следующие ресурсы групп:

- [event](../resources/event.md) для групп;
- [calendar](../resources/calendar.md) для групп;
- [post](../resources/post.md) для групп. 

Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).

## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуется одна из указанных ниже **областей** (в зависимости от ресурса, который требуется получить).

- _Mail.Read_
- _Calendars.Read_
- _Contacts.Read_
- _Group.Read.All_ 

## <a name="http-request"></a>HTTP-запрос

#### <a name="get-a-resource-instance-using-expand"></a>Запрос GET на получение экземпляра ресурса с помощью параметра `$expand`
Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое соответствует фильтру по свойству **id**. Убедитесь, что вы применяете [кодировку URL](http://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.

Получение экземпляра объекта **message**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Получение экземпляра объекта **mailFolder**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

Получение экземпляра объекта **event**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Получение экземпляра объекта **calendar**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Получение экземпляра объекта **contact**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Получение экземпляра объекта **contactFolder**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Получение экземпляра объекта **event** для группы:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

Получение экземпляра объекта **post** для группы:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-using-filter"></a>Запрос GET на получение экземпляров ресурсов с помощью параметра `$filter`

Получение экземпляров поддерживаемого ресурса с расширенным свойством, соответствующим фильтру для свойств **id** и **value**. Убедитесь, что вы применяете [кодировку URL](http://www.w3schools.com/tags/ref_urlencode.asp) для символов косой черты и пробела в строке фильтра.


Получение экземпляров объекта **message**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Получение экземпляров объекта **mailFolder**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

Список экземпляров объекта **event**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Получение экземпляров объекта **calendar**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Получение экземпляров объекта **contact**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Получение экземпляров объекта **contactFolder**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Получение экземпляров объекта **event** для группы:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

Получение экземпляров объекта **post** для группы:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

## <a name="parameters"></a>Параметры
|**Параметр**|**Тип**|**Описание**|
|:-----|:-----|:-----|
|_Параметры URL-адреса_|
|id_value|String|Идентификатор сопоставляемого расширенного свойства. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.|
|property_value|String|Значение сопоставляемого расширенного свойства. Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос** выше.|

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |


## <a name="request-body"></a>Основной текст запросов
Не указывайте тело запроса для этого метода.
## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `200 OK`.

#### <a name="get-resource-instance-using-expand"></a>Запрос GET на получение экземпляра ресурса с помощью `$expand`
Текст отклика содержит объект, который представляет запрашиваемый экземпляр ресурса, дополненный соответствующим объектом [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md).
  
#### <a name="get-resource-instances-using-filter"></a>Запрос GET на получение экземпляров ресурсов с помощью параметра `$filter`
Текст отклика содержит один или несколько объектов, представляющих экземпляры ресурсов, которые содержат соответствующее расширенное свойство. Текст отклика не включает расширенное свойство.

## <a name="example"></a>Пример
#### <a name="request-1"></a>Запрос 1

В первом примере показано, как получить указанное сообщение и дополнить его расширенным свойством с одним значением. Фильтр возвращает расширенное свойство, значение **id** которого совпадает со строкой `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL).

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
##### <a name="response-1"></a>Отклик 1
Текст отклика включает все свойства указанного сообщения и расширенное свойство, возвращенное из фильтра.

Примечание. Показанный здесь объект **message** усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AACbyS4H\"",
    "id": "AAMkAGE1M2_bs88AACHsLqWAAA=",
    "subject": "RE: Talk about emergency prep",
    "sender": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "from": null,
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Christine Irwin",
                "address": "christine@contoso.com"
            }
        }
    ],
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

****

#### <a name="request-2"></a>Запрос 2

Во втором примере показано, как получить сообщения, у которых есть расширенное свойство с одним значением, указанное в фильтре. Фильтр возвращает расширенное свойство со следующими параметрами:
- Параметр **id** совпадает со строкой `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL).
- Для параметра **value** задано значение `Green`.

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/api/v1.0/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

##### <a name="response-2"></a>Отклик 2

В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а текст отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру. Текст отклика аналогичен отклику при [получении коллекции сообщений](../api/user_list_messages.md). Отклик не включает соответствующее расширенное свойство.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->