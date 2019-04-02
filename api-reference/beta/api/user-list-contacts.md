---
title: Список контактов
description: Получение контактов в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a1eaeac682f511bf9b895e06e6a19b3bc728a38c
ms.sourcegitcommit: e6168b868660ad0078d460424d4e6f987d2684a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2019
ms.locfileid: "31026012"
---
# <a name="list-contacts"></a>Список контактов

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение контактов в почтовом ящике пользователя.

Существует два сценария, в которых приложение может получать контакты в папке контактов другого пользователя:

* если у приложения есть разрешения для приложений;
* Если приложение имеет соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь предоставил доступ к папке контактов для этого пользователя или предоставил ему делегированный доступ. См. [подробные сведения и пример](/graph/outlook-get-shared-contacts-folders).


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Contacts.Read, Contacts.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Contacts.Read, Contacts.ReadWrite    |
|Для приложений | Contacts.Read, Contacts.ReadWrite |

## <a name="http-request"></a>HTTP-запрос

Для получения всех контактов в почтовом ящике пользователя:

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

Для получения контактов, которые хранятся в определенной папке в почтовом ящике пользователя:

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
С помощью параметра `$filter` запроса можно фильтровать контакты на основе их адресов электронной почты:

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

Обратите внимание, что `$filter`вы `any`можете использовать, `eq` и оператор, только для вложенного свойства **Address** экземпляров в коллекции **EmailAddresses** . То есть невозможно выполнить фильтрацию по **имени** или другому подсвойству экземпляра **EmailAddresses**, а также к любому другому оператору или функции с `filter`помощью, например `ne`, `le`, и. `startswith()`

Общие сведения о параметре `$filter` запроса можно узнать в разделе [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В следующем примере возвращаются свойства **DisplayName** и **EmailAddresses** для контактов вошедшего пользователя.
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```


##### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts(displayName,emailAddresses)",
    "value":[
        {
            "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7f6\"",
            "id":"AAMkADh6v5AAAvgTCFAAA=",
            "displayName":"Elvis Blank",
            "emailAddresses":[
                {
                    "type":"personal",
                    "name":"Elvis Blank",
                    "address":"elvisb@relecloud.onmicrosoft.com"
                },
                {
                    "type":"other",
                    "otherLabel":"Volunteer work",
                    "name":"Elvis Blank",
                    "address":"elvisb@fabrikam.onmicrosoft.com"
                }
            ]
        },
        {
            "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fn\"",
            "id":"AAMkADh6v5AAAvgTCEAAA=",
            "displayName":"Pavel Bansky",
            "emailAddresses":[
                {
                    "type":"personal",
                    "name":"Pavel Bansky",
                    "address":"pavelb@contoso.onmicrosoft.com"
                },
                {
                    "type":"other",
                    "otherLabel":"Volunteer work",
                    "name":"Pavel Bansky",
                    "address":"pavelb@fabrikam.onmicrosoft.com"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-contacts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
