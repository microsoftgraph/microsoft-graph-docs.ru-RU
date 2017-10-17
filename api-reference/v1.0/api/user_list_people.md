# <a name="list-people"></a>Получение списка людей

Вы можете получить коллекцию объектов [person](../resources/person.md), упорядоченных по их релевантности для [пользователя](../resources/user.md), которая определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями.

Вы можете получить эти сведения с помощью API People. Примеры см. в разделе [Примеры](#examples) и статье о том, как [получить релевантную информацию о людях](../../../concepts/people_example.md).

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
GET /me/people
GET /users/{id | userPrincipalName}/people
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
|Имя|Значение|Описание|
|:---------------|:--------|:-------|
|$filter|string|Позволяет возвращать в отклике только тех людей, чьи записи содержат указанные критерии.|
|$orderby|string|По умолчанию люди в отклике отсортированы по их релевантности вашему запросу. Вы можете изменить порядок людей в отклике, используя параметр *$orderby*.|
|$search|string|Поиск пользователей по имени или псевдониму. Поддерживается функция нечеткого соответствия.|
|$select|string|Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.|
|$skip|int|Пропуск первых n результатов; эту функцию удобно использовать при разбиении результатов на страницы. Эта возможность не поддерживается при использовании параметра *$search*.|
|$top|int|Количество возвращаемых результатов.|

## <a name="request-headers"></a>Заголовки запроса
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Accept | application/json |

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [person](../resources/person.md) в тексте ответа. Отклик может содержать один объект person либо коллекцию объектов person. 
## <a name="examples"></a>Примеры

### <a name="get-a-collection-of-relevant-people"></a>Получение коллекции релевантных людей 

С помощью указанного ниже запроса можно получить людей, наиболее релевантных для пользователя, выполнившего вход в систему (`/me`), на основании его шаблонов общения и совместной работы, а также бизнес-отношений. 
<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

В примере ниже показан отклик. По умолчанию в каждом отклике возвращается 10 записей. Вы можете изменить количество возвращаемых записей с помощью параметра запроса *$top*. В этом примере показано, как использовать параметр запроса *$top* для ограничения количества записей (до 3 шт.) в отклике.
<!-- {
  "blockType": "response",
  "name": "get_person_collection",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye",
            "givenName": "Lorrie",
            "surname": "Frye",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Paralegal",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "20/1109",
            "profession": "",
            "userPrincipalName": "Lorrief@contoso.onmicrosoft.com",
            "imAddress": "sip:Lorrief@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 980 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        },
        {
            "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
            "displayName": "Maynard Denman",
            "givenName": "Maynard",
            "surname": "Denman",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "userPrincipalName": "Maynardd@contoso.onmicrosoft.com",
            "imAddress": "sip:Maynardd@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Maynardd@contoso.onmicrosoft.com",
                    "relevanceScore": 8.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        },
        {
            "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
            "displayName": "Darrel Halsey",
            "givenName": "Darrel",
            "surname": "Halsey",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Attorney",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "14/1102",
            "profession": "",
            "userPrincipalName": "Darrelh@contoso.onmicrosoft.com",
            "imAddress": "sip:Darrelh@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Darrelh@contoso.onmicrosoft.com",
                    "relevanceScore": 8.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 205 555 0103"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        }
    ]
}
```
### <a name="search-other-users-relevant-people"></a>Поиск людей, релевантных для другого пользователя

Указанный ниже запрос возвращает людей, наиболее релевантных для другого пользователя в организации пользователя, выполнившего вход в систему. Для выполнения этого запроса требуется разрешение People.Read.All. В этом примере отображаются люди, релевантные для пользователя Roscoe Seidel.

<!-- {
  "blockType": "request",
  "name": "get_other_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

В примере ниже показан отклик. По умолчанию в каждом отклике возвращается 10 записей. Вы можете изменить количество возвращаемых записей с помощью параметра *$top*. В этом примере показано, как использовать параметр запроса *$top* для ограничения количества записей (до 3 шт.) в отклике.

<!-- {
  "blockType": "response",
  "name": "get_other_person",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
     "value": [
        {
            "id": "56155636-703F-47F2-B657-C83F01F49BBC",
            "displayName": "Clifton Clemente",
            "givenName": "Clifton",
            "surname": "Clemente",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Director",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "19/2106",
            "profession": "",
            "userPrincipalName": "Cliftonc@contoso.onmicrosoft.com",
            "imAddress": "sip:Cliftonc@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Cliftonc@contoso.onmicrosoft.com",
                    "relevanceScore": 20.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 309 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        },
        {
            "id": "6BF27D5A-AB4F-4C43-BED0-7DAD9EB0C1C4",
            "displayName": "Sheree Mitchell",
            "givenName": "Sheree",
            "surname": "Mitchell",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Product Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/2107",
            "profession": "",
            "userPrincipalName": "Shereem@contoso.onmicrosoft.com",
            "imAddress": "sip:shereem@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Shereem@contoso.onmicrosoft.com",
                    "relevanceScore": 10.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 918 555 0107"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        },
        {
            "id": "B3E5302D-EAF0-4E8B-8C6C-A2AE64B4B163",
            "displayName": "Vincent Matney",
            "givenName": "Vincent",
            "surname": "Matney",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "CVP Engineering",
            "companyName": null,
            "yomiCompany": "",
            "department": "Engineering",
            "officeLocation": "23/2102",
            "profession": "",
            "userPrincipalName": "Vincentm@contoso.onmicrosoft.com",
            "imAddress": "sip:vincentm@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Vincentm@contoso.onmicrosoft.com",
                    "relevanceScore": 10.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 502 555 0102"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
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
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
