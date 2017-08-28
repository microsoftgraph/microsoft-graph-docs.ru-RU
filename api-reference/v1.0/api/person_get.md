# <a name="get-person"></a>Вывод сведений о человеке

Получение свойств и связей объекта [person](../resources/person.md).

Для получения этих сведений используйте API службы "Люди". Примеры см. в разделе [Примеры](#examples) и статье о том, как [получить релевантную информацию о людях](../../../concepts/people_example.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).
 

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | People.Read, People.Read.All    |
|Делегированные (личная учетная запись Майкрософт) | People.Read    |
|Для приложений | People.Read.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/?$search='{property_value}'
GET /me/people/?$filter={person_property} eq '{property_value}'
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
|Имя|Значение|Описание|
|:---------------|:--------|:-------|
|$filter|string|Позволяет возвращать в отклике только тех людей, чьи записи содержат указанные критерии.|
|$orderby|string|По умолчанию данные о людях в отклике сортируются по степени соответствия запросу. Этот порядок можно изменить с помощью параметра *$orderby*.|
|$search|string|Поиск пользователей по имени или псевдониму. Поддерживается функция нечеткого соответствия.|
|$select|string|Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.|
|$skip|int|Пропуск первых n результатов; эту функцию удобно использовать при разбиении результатов на страницы. Эта возможность не поддерживается при использовании параметра *$search*.|
|$top|int|Число возвращаемых результатов.|

## <a name="parameters"></a>Параметры
| Параметр |Тип       |Описание|
|:----------|:----------|:----------|
|property_value|String     |Значение сопоставляемого расширенного свойства. Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос**.|
|person_property|String    |Соответствие свойству person. Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос**.|

## <a name="request-headers"></a>Заголовки запроса
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [person](../resources/person.md) в тексте отклика. Отклик может содержать как один, так и коллекцию экземпляров person. 
## <a name="examples"></a>Примеры
### <a name="perform-a-search"></a>Выполнение поиска 
В приведенном ниже запросе выполняется поиск пользователя по имени Irene McGowan. 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowan"
```

Ниже приводится пример отклика. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```
### <a name="select-the-fields-to-return-in-a-filtered-response"></a>Выбор полей, которые возвращаются в отфильтрованном отклике 
Сочетая параметры *$select* и *$filter*, вы можете создать настраиваемый список людей, релевантных для пользователя, и получать только те поля, которые необходимы вашему приложению. 

В примере ниже показано, как получить значения полей **displayName** и **scoredEmailAddresses** для людей, чьи отображаемые имена совпадают с заданными. В этом примере показано, как возвратить людей c отображаемыми именами Lorrie Frye. 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

В примере ниже показан отклик. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get person",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
