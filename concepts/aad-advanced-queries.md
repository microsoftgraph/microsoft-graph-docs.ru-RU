---
title: Расширенные возможности запросов для объектов каталога Azure AD
description: Объекты каталога Azure AD поддерживают расширенные возможности запросов для эффективного доступа к данным.
author: Licantrop0
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: e8a6c4a3a2d37eafeaee85f7778baa68bad97357
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351293"
---
# <a name="advanced-query-capabilities-on-azure-ad-directory-objects"></a>Расширенные возможности запросов для объектов каталога Azure AD

В Azure AD постоянно добавляются новые возможности, повышается стабильность, доступность и производительность этого решения. Одновременно ведется работа и над усовершенствованием Microsoft Graph для масштабирования и эффективного доступа к данным. Одно из направлений этого усовершенствования заключается в усилении поддержки возможностей расширенных запросов для различных объектов Azure AD и их свойств. Например, добавление операторов **Not** (`NOT`), **Not equals** (`ne`) и **Ends with** (`endsWith`) к параметру запроса `$filter` в октябре 2020 г.

Механизм запросов Microsoft Graph использует хранилище индексов для выполнения запросов. Чтобы добавить поддержку дополнительных возможностей запросов для некоторых свойств, индексирование этих свойств теперь происходит на отдельном сервере. Благодаря этому отдельному индексированию в Azure AD расширена поддержка и повышена производительность запросов. Тем не менее, эти расширенные возможности запросов по умолчанию недоступны. Запрашивающий должен установить для заголовка **ConsistencyLevel** значение `eventual`, *а также*, за исключением `$search`, использовать параметр запроса `$count` (в виде [сегмента URL-адреса](/graph/query-parameters#other-odata-url-capabilities) или строки запроса `$count=true`). Заголовок **ConsistencyLevel** и `$count` называются *расширенными параметрами запроса*.

Например, если нужно получить только учетные записи неактивных пользователей, можно выполнить любой из этих запросов, использующих параметр запроса `$filter`.

+ Используйте параметр запроса `$filter` с оператором `eq`. Этот запрос будет работать по умолчанию, то есть этот запрос не требует расширенных параметров запроса.

<!-- {
  "blockType": "ignored",
  "name": "get_users_enabled"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=accountEnabled eq false
```

+ Используйте параметр запроса `$filter` с оператором `ne`. Этот запрос не поддерживается по умолчанию, поскольку оператор `ne` поддерживается только в расширенных запросах. Поэтому необходимо добавить заголовок **ConsistencyLevel**, для которого должно быть указано значение `eventual`*, а также* использовать строку запроса `$count=true`.

<!-- {
  "blockType": "ignored",
  "name": "get_users_not_enabled"
} -->
```msgraph-interactive
https://graph.microsoft.com/v1.0/users?$filter=accountEnabled ne true&$count=true
ConsistencyLevel: eventual
```

Эти расширенные возможности запросов поддерживаются только для объектов Azure AD, то есть для следующих ресурсов и их взаимосвязей, производных от [directoryObject](/graph/api/resources/directoryobject):

- [application](/graph/api/resources/application)
- [orgContact](/graph/api/resources/orgcontact)
- [device](/graph/api/resources/device)
- [group](/graph/api/resources/group)
- [servicePrincipal](/graph/api/resources/serviceprincipal)
- [user](/graph/api/resources/user)

В следующей таблицы приведены сценарии запросов для объектов каталога, поддерживаемые только в расширенных запросах.

| Описание                                                              | Пример                                                                                                                                                                                                                                                                                                                                                                                                                              |
|:-------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Использование `$count` в качестве сегмента URL-адреса                                         | [GET](https://developer.microsoft.com/graph/graph-explorer?request=groups%2F%24count&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups/$count`                                                                                                                                                                                       |
| Использование `$count` в качестве параметра строки запроса                              | [GET](https://developer.microsoft.com/graph/graph-explorer?request=servicePrincipals%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../servicePrincipals?$count=true`                                                                                                                                                     |
| Использование `$search`                                                         | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24search%3D%22displayName%3ABrowser%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$search="displayName:Browser"`                                                                                                                     |
| Использование `$orderby` для выбранных свойств                                   | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$count=true`                                                                                                               |
| Использование `$filter` с оператором `endsWith`                            | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40outlook.com')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@outlook.com')`                                                                                       |
| Использование `$filter` и `$orderby` в одном и том же запросе                        | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24filter%3DstartsWith(displayName%2C%20'Box')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$filter=startsWith(displayName, 'Box')&$count=true`                       |
| Использование `$filter` с операторами `startsWith` для определенных свойств | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DstartsWith(mobilePhone%2C%20'25478')%20OR%20startsWith(mobilePhone%2C%20'25473')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=startsWith(mobilePhone, '25478') OR startsWith(mobilePhone, '25473')&$count=true` |
| Использование `$filter` с операторами `ne` и `NOT`                           | 
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`                     |
| Использование `$filter` с операторами `NOT` и `startsWith`                   | 
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=%2Fusers%3F%24filter%3DNOT%20startsWith(displayName%2C%20'Conf')%26%24count%3Dtrue&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=NOT startsWith(displayName, 'Conf')&$count=true`                                                                |
| Использование функции OData cast с другим параметром запроса                           | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true`                                                                                             |

> [!NOTE]
> Эти расширенные возможности запросов недоступны в клиентах Azure AD B2C.

## <a name="support-for-filter-on-properties-of-azure-ad-directory-objects"></a>Поддержка фильтрации по свойствам объектов каталога Azure AD

Свойства объектов каталога ведут себя по-разному в отношении поддержки параметров запросов. Ниже приведены распространенные сценарии для объектов каталога:

+ Если не указано иное, свойства с одинаковыми именами в ресурсах каталога поддерживают одинаковые операторы `$filter`. Например, свойство **createdDateTime**, доступное в ресурсах **application**, **group**, **organization** и **user**. Это свойство по умолчанию поддерживает операторы `eq`, `ge` и `le`; при этом оно поддерживает операторы `in`, `ne` и `NOT` только в расширенных запросах.
+ Оператор `endsWith` поддерживается только для свойств **mail** и **userPrincipalName**.
+ Запросы, поддерживаемые по умолчанию, поддерживаются в расширенных запросах.
+ Операторы отрицания `NOT` и `ne` поддерживаются только в расширенных запросах. 
  + Все свойства, поддерживающие оператор `eq`, также поддерживают операторы `ne` или `NOT`.
  + Оператор `ne` задействует отрицание в случаях, когда оператор `eq` выдал бы значение `true`. Для запросов, использующих лямбда-оператор `any`, используйте оператор `NOT`. См. [Фильтрация с помощью лямбда-операторов](/graph/query-parameters#filter-using-lambda-operators)..

В следующей таблице перечислена поддержка операторов `$filter` свойствами объекта каталога [users](/graph/api/resources/user).

- ![Работает по умолчанию. Не требуются расширенные параметры запроса.](/graph/images/advanced-query-parameters/default.png) Это свойство поддерживает `$filter` с оператором по умолчанию.
- ![Требуются расширенные параметры запроса.](/graph/images/advanced-query-parameters/advanced.png) Для конкретного оператора `$filter` требуются *расширенные параметры запроса.*
  - Заголовок `ConsistencyLevel=eventual`
  - Строка запроса `$count=true`
- Пустые ячейки указывают, что это свойство не поддерживает использование `$filter` с оператором.
- Столбец **Значения null** указывает, что для этого свойства поддерживается фильтрация по значениям `null`.
- Свойства, не указанные здесь, не поддерживают `$filter`.

[!INCLUDE [filter-directory-objects](../includes/filter-directory-objects.md)]


## <a name="error-handling-for-advanced-queries-on-directory-objects"></a>Обработка ошибок расширенных запросов к объектам каталога

Подсчет объектов каталога поддерживается только с использованием расширенных параметров запросов. Если заголовок `ConsistencyLevel=eventual` не указан, запрос возвращает ошибку, когда используется сегмент URL-адреса `$count`, или автоматически игнорирует параметр запроса `$count` (`?$count=true`), если он используется.

```http
https://graph.microsoft.com/v1.0/users/$count
```

```json
{
    "error": {
        "code": "Request_BadRequest",
        "message": "$count is not currently supported.",
        "innerError": {
            "date": "2021-05-18T19:03:10",
            "request-id": "d9bbd4d8-bb2d-44e6-99a1-71a9516da744",
            "client-request-id": "539da3bd-942f-25db-636b-27f6f6e8eae4"
        }
    }
}
```

`$search` для ресурсов Azure AD, производных от [directoryObject](/graph/api/resources/directoryobject), работает только в расширенных запросах. Если заголовок **ConsistencyLevel** не указан, запрос возвращает ошибку.

```http
https://graph.microsoft.com/v1.0/applications?$search="displayName:Browser"
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "Request with $search query parameter only works through MSGraph with a special request header: 'ConsistencyLevel: eventual'",
        "innerError": {
            "date": "2021-05-27T14:26:47",
            "request-id": "9b600954-ba11-4899-8ce9-6abad341f299",
            "client-request-id": "7964ef27-13a3-6ca4-ed7b-73c271110867"
        }
    }
}
```

Если свойство или параметр запроса в URL-адресе поддерживаются только в расширенных запросах, но отсутствует заголовок **ConsistencyLevel** или строка запроса `$count=true`, то запрос возвращает ошибку.

```http
https://graph.microsoft.com/beta/users?$filter=endsWith(mail,'@outlook.com')
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "Unsupported Query.",
        "innerError": {
            "date": "2021-05-18T19:12:36",
            "request-id": "63f2093c-399c-4350-9609-3ce9b62abe3c",
            "client-request-id": "e60ed0ba-df5d-e190-f056-f9c0318456d7"
        }
    }
}
```

Если свойство не проиндексировано для поддержки параметра запроса, даже если указаны расширенные параметры запроса, то запрос возвращает ошибку.

```http
https://graph.microsoft.com/v1.0/users?$filter=id ge '398164b1-5196-49dd-ada2-364b49f99b27'&$count=true
ConsistencyLevel: eventual
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "The request uses a filter property that is not indexed",
        "innerError": {
            "date": "2021-06-10T19:32:01",
            "request-id": "5625ba13-0c9f-4fce-a853-4b52f3e0bd09",
            "client-request-id": "76fe4cd8-df3a-f8c3-659b-594274b6bb31"
        }
    }
}
```

При этом необходимо отметить, что указанные в запросе параметры могут просто не сработать. Это может произойти, если не поддерживаются либо сами параметры, либо их сочетание. В таких случаях необходимо проверить возвращенные запросом данные и определить, дали ли указанные параметры запроса желаемый результат. В следующем примере параметр `@odata.count` отсутствует, даже если запрос успешно выполняется.

```http
https://graph.microsoft.com/v1.0/users?$count=true
```

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "value":[
    {
      "displayName":"Oscar Ward",
      "mail":"oscarward@contoso.com",
      "userPrincipalName":"oscarward@contoso.com"
    },
  ]
}
```

## <a name="see-also"></a>См. также

- [Настройка откликов с помощью параметров запроса](/graph/query-parameters)
- [Ограничения параметров запроса](known-issues.md#query-parameter-limitations)
- [Использование параметра запроса $search для сопоставления с условием поиска](/graph/aad-advanced-queries)
