# <a name="get-person"></a>Вывод сведений о человеке

Получение свойств и связей объекта [person](../resources/person.md).

Для получения этих сведений используйте API службы "Люди". Примеры представлены в разделе [Примеры](#examples) и статье [Получение релевантных сведений о людях](../../../concepts/people_example.md).

## <a name="prerequisites"></a>Необходимые условия
Для применения фрагментов этого API требуются следующие **разрешения**: *People.Read*; *People.Read.All*
 
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/?$search='{property_value}'
GET /me/people/?$filter={person_property} eq '{property_value}'
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
|Имя|Значение|Описание|
|:---------------|:--------|:-------|
|$filter|string|Ограничивает отклик данными тех людей, чьи записи содержат указанные условия.|
|$orderby|string|По умолчанию данные о людях в отклике сортируются по степени соответствия запросу. Этот порядок можно изменить с помощью параметра *$orderby*.|
|$search|string|Поиск пользователей по имени или псевдониму. Поддерживается функция нечеткого соответствия.|
|$select|string|Разделенный запятыми список свойств, включаемых в ответ. Для оптимальной производительности требуется выбрать подмножество нужных свойств.|
|$skip|int|Пропуск первых n результатов. Эта функция полезна при разбиении на страницы. Не поддерживается, если используется параметр *$search*.|
|$top|int|Число возвращаемых результатов.|

## <a name="parameters"></a>Параметры
| Параметр |Тип       |Описание|
|:----------|:----------|:----------|
|property_value|String     |Значение сопоставляемого расширенного свойства. Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос**.|
|person_property|String    |Соответствие свойству person. Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос**.|

## <a name="request-headers"></a>Заголовки запросов
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
Можно объединить параметры *$select* и *$filter*, чтобы создать настраиваемый список людей, имеющих отношение к данному пользователю, при этом возвращаются только поля, которые требуются приложению. 

В примере ниже возвращаются данные **displayName** и **scoredEmailAddresses** для людей, чье отображаемое имя соответствует указанному. В этом примере возвращаются сведения только о людях, чье отображаемое имя соответствует имени Lorrie Frye. 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
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
