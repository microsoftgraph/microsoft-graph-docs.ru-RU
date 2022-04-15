---
title: Расширенные возможности запросов для объектов каталога Azure AD
description: Объекты каталога Azure AD поддерживают расширенные возможности запросов для эффективного доступа к данным.
author: Licantrop0
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: b5eff1cba4f2f8db4e09c5224aaf4b43ff86d513
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2022
ms.locfileid: "64848659"
---
# <a name="advanced-query-capabilities-on-azure-ad-directory-objects"></a>Расширенные возможности запросов для объектов каталога Azure AD

В Azure AD постоянно добавляются новые возможности, повышается стабильность, доступность и производительность этого решения. Одновременно ведется работа и над усовершенствованием Microsoft Graph для масштабирования и эффективного доступа к данным. Одно из направлений этого усовершенствования заключается в усилении поддержки возможностей расширенных запросов для различных объектов Azure AD и их свойств. Например, можно добавлять операторы **Не** (`not`), **Не равно** (`ne`) и **Оканчивается на** (`endsWith`) к параметру запроса `$filter`.

Механизм запросов Microsoft Graph использует хранилище индексов для выполнения запросов. Чтобы добавить поддержку дополнительных возможностей запросов для некоторых свойств, индексирование этих свойств теперь происходит в отдельном хранилище. Благодаря этому отдельному индексированию в Azure Active Directory расширена поддержка и повышена производительность запросов. Однако эти расширенные возможности запросов по умолчанию недоступны. Запросившая сторона также должна установить **ConsistencyLevel** в качестве заголовка, чтобы `eventual` *и*, за исключением `$search`, использовать `$count` параметр запроса. Заголовок **ConsistencyLevel** и `$count` называются *расширенными параметрами запроса*.

Например, если нужно получить только учетные записи неактивных пользователей, можно выполнить любой из этих запросов, использующих параметр запроса `$filter`.

<!-- markdownlint-disable MD023 MD024 MD025 -->
+ Вариант 1. Используйте параметр запроса `$filter` с оператором `eq`. Этот запрос будет работать по умолчанию, то есть этот запрос не требует расширенных параметров запроса.

    # <a name="http"></a>[HTTP](#tab/http)
    <!-- {
      "blockType": "request",
      "name": "get_users_enabled"
    } -->
    ```msgraph-interactive
    GET https://graph.microsoft.com/v1.0/users?$filter=accountEnabled eq false
    ```

    # <a name="c"></a>[C#](#tab/csharp)

    ```csharp
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=CS
    var user = await graphClient.Users.Request()
        .Filter("accountEnabled eq false")
        .GetAsync();
    ```

    # <a name="javascript"></a>[JavaScript](#tab/javascript)

    ```javascript
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Javascript
    let users = await client.api('/users')
      .filter('accountEnabled eq false')
      .get();
    ```

    # <a name="objective-c"></a>[Objective-C](#tab/objc)

    ```objectivec
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Objective-C
    NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users?$filter=accountEnabled eq false"]]];
    [urlRequest setHTTPMethod:@"GET"];

    MSURLSessionDataTask *usersDataTask = [httpClient dataTaskWithRequest:urlRequest
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

      NSError *jsonError = nil;
      MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
      MSGraphUser *user = [[MSGraphUser alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

    }];

    [usersDataTask execute];
    ```

    # <a name="java"></a>[Java](#tab/java)

    ```java
    // See https://docs.microsoft.com/en-us/graph/sdks/create-client?tabs=Java
    UserCollectionPage users = graphClient.users()
        .buildRequest()
        .filter("accountEnabled eq false")
        .get();
    ```

    # <a name="go"></a>[Go](#tab/go)

    ```go
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Go
    requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
        Filter: "accountEnabled eq false",
    }

    options := &msgraphsdk.UsersRequestBuilderGetOptions{
        Q: requestParameters,
    }

    result, err := client.Users().Get(options)
    ```

    # <a name="powershell"></a>[PowerShell](#tab/powershell)

    ```powershell
    Import-Module Microsoft.Graph.Users

    Get-MgUser -Filter "accountEnabled eq false"
    ```

    ---

+ Вариант 2. Используйте параметр запроса `$filter` с оператором `ne`. Этот запрос не поддерживается по умолчанию, поскольку оператор `ne` поддерживается только в расширенных запросах. Поэтому необходимо добавить заголовок **ConsistencyLevel**, для которого должно быть указано значение `eventual`*, а также* использовать строку запроса `$count=true`.

    # <a name="http"></a>[HTTP](#tab/http)
    <!-- {
      "blockType": "request",
      "name": "get_users_not_enabled"
    } -->
    ```msgraph-interactive
    GET https://graph.microsoft.com/v1.0/users?$filter=accountEnabled ne true&$count=true
    ConsistencyLevel: eventual
    ```

    # <a name="c"></a>[C#](#tab/csharp)

    ```csharp
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=CS
    var user = await graphClient.Users.Request()
        .Request(new Option[] { new QueryOption("$count", "true")})
        .Header("ConsistencyLevel", "eventual")
        .Filter("accountEnabled ne true")
        .GetAsync();
    ```

    # <a name="javascript"></a>[JavaScript](#tab/javascript)

    ```javascript
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Javascript
    let users = await client.api('/users')
      .header('ConsistencyLevel','eventual')
      .filter('accountEnabled ne true')
      .count(true)
      .get();
    ```

    # <a name="objective-c"></a>[Objective-C](#tab/objc)

    ```objectivec
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Objective-C
    NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users?$filter=accountEnabled ne true&$count=true"]]];
    [urlRequest setHTTPMethod:@"GET"];
    [urlRequest setValue:@"eventual" forHTTPHeaderField:@"ConsistencyLevel"];

    MSURLSessionDataTask *usersDataTask = [httpClient dataTaskWithRequest:urlRequest
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

      NSError *jsonError = nil;
      MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
      MSGraphUser *user = [[MSGraphUser alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

    }];

    [usersDataTask execute];
    ```

    # <a name="java"></a>[Java](#tab/java)

    ```java
    // See https://docs.microsoft.com/en-us/graph/sdks/create-client?tabs=Java
    LinkedList<Option> requestOptions = new LinkedList<Option>();
    requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
    requestOptions.add(new QueryOption("$count", "true"))

    UserCollectionPage users = graphClient.users()
        .buildRequest(requestOptions)
        .filter("accountEnabled ne true")
        .get();
    ```

    # <a name="go"></a>[Go](#tab/go)

    ```go
    // See https://docs.microsoft.com/graph/sdks/create-client?tabs=Go
    requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
        Filter: "accountEnabled ne true",
        Count: true,
    }

    headers := map[string]string{
        "ConsistencyLevel": "eventual"
    }

    options := &msgraphsdk.UsersRequestBuilderGetOptions{
        Q: requestParameters,
        H: headers,
    }

    result, err := client.Users().Get(options)
    ```

    # <a name="powershell"></a>[PowerShell](#tab/powershell)

    ```powershell
    Import-Module Microsoft.Graph.Users

    Get-MgUser -Filter "accountEnabled ne true" -CountVariable CountVar -ConsistencyLevel eventual
    ```

    ---

<!-- markdownlint-enable MD023 MD024 MD025 -->

Эти расширенные возможности запросов поддерживаются только для объектов каталога Azure Active Directory и их взаимосвязей, включая следующие часто используемые объекты:

| Объект                                                         | Связи                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Административная единица](/graph/api/resources/administrativeunit) | <li>[члены](/graph/api/administrativeunit-list-members)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [Приложение](/graph/api/resources/application)                | <li>[владельцы](/graph/api/application-list-owners)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| [Устройство](/graph/api/resources/device)                          | <li>[memberOf](/graph/api/device-list-memberof) <li>[transitiveMemberOf](/graph/api/device-list-transitivememberof) <li>[registeredUsers](/graph/api/device-list-registeredusers) <li>[registeredOwners](/graph/api/device-list-registeredowners)                                                                                                                                                                                                                                                                                                                                                                   |
| [Группа](/graph/api/resources/group)                            | <li>[члены](/graph/api/group-list-members) <li>[transitiveMembers](/graph/api/group-list-transitivemembers) <li>[memberOf](/graph/api/group-list-memberof) <li>[transitiveMemberOf](/graph/api/group-list-transitivememberof) <li>[владельцы](/graph/api/group-list-owners) <li>[appRoleAssignments](/graph/api/group-list-approleassignments)                                                                                                                                                                                                                                                                       |
| [Контакты организации](/graph/api/resources/orgContact)                     | <li>[memberOf](/graph/api/orgcontact-list-memberof) <li>[transitiveMemberOf](/graph/api/orgcontact-list-transitiveMemberOf)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| [Субъект-служба](/graph/api/resources/serviceprincipal)     | <li>[memberOf](/graph/api/serviceprincipal-list-memberof) <li>[transitiveMemberOf](/graph/api/serviceprincipal-list-transitivememberof) <li>[appRoleAssignments](/graph/api/serviceprincipal-list-approleassignments) <li>[appRoleAssignmentsTo](/graph/api/serviceprincipal-list-approleassignedto) <li>[oAuth2PermissionGrant](/graph/api/serviceprincipal-list-oauth2permissiongrants)                                                                                                                                                                                                                           |
| [Пользователь](/graph/api/resources/user)                              | <li>[memberOf](/graph/api/user-list-memberof) <li>[transitiveMemberOf](/graph/api/user-list-transitivememberof)<li>[ownedObjects](/graph/api/user-list-ownedobjects) <li>[registeredDevices](/graph/api/user-list-registereddevices) <li>[ownedDevices](/graph/api/user-list-owneddevices) <li>[transitiveManagers](/graph/api/user-list-manager) <li>[directReports](/graph/api/user-list-directreports) <li>[transitiveReports](/graph/api/user-get-transitivereports) <li>[appRoleAssignments](/graph/api/user-list-approleassignments) <li>[oAuth2PermissionGrant](/graph/api/user-list-oauth2permissiongrants) |

В следующей таблице приведены сценарии запросов для объектов каталога, поддерживаемые только в расширенных запросах:

| Описание                                                              | Пример                                                                                                                                                                                                                                                                                                                                                                                                                              |
| :----------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Использование `$count` в качестве сегмента URL-адреса                                         | [GET](https://developer.microsoft.com/graph/graph-explorer?request=groups%2F%24count&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups/$count`                                                                                                                                                                                       |
| Использование `$count` в качестве параметра строки запроса                              | [GET](https://developer.microsoft.com/graph/graph-explorer?request=servicePrincipals%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../servicePrincipals?$count=true`                                                                                                                                                     |
| Использование `$search`                                                         | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24search%3D%22displayName%3ABrowser%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$search="displayName:Browser"`                                                                                                                     |
| Использование `$orderby` для выбранных свойств                                   | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$count=true`                                                                                                               |
| Использование `$filter` с оператором `endsWith`                            | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40outlook.com')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@outlook.com')`                                                                                       |
| Использование `$filter` и `$orderby` в одном и том же запросе                        | [GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24filter%3DstartsWith(displayName%2C%20'Box')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$filter=startsWith(displayName, 'Box')&$count=true`                       |
| Использование `$filter` с операторами `startsWith` для определенных свойств | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DstartsWith(mobilePhone%2C%20'25478')%20OR%20startsWith(mobilePhone%2C%20'25473')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=startsWith(mobilePhone, '25478') OR startsWith(mobilePhone, '25473')&$count=true` |
| Использование `$filter` с операторами `ne` и `not`                           | 
  [GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`                           |
| Использование `$filter` с операторами `not` и `startsWith`                   | 
  [GET](https://developer.microsoft.com/graph/graph-explorer?request=%2Fusers%3F%24filter%3DNOT%20startsWith(displayName%2C%20'Conf')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=NOT startsWith(displayName, 'Conf')&$count=true`                                                                      |
| Использование функции OData cast с другим параметром запроса                           | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true`                                                                                             |

> [!NOTE]
>
> + Совместное использование `$filter` и `$orderBy` поддерживается только в расширенных запросах.
> + `$expand` в настоящее время не поддерживается в расширенных запросах.
> + Расширенные возможности запросов в настоящее время недоступны для клиентов Azure AD B2C.

## <a name="support-for-filter-on-properties-of-azure-ad-directory-objects"></a>Поддержка фильтрации по свойствам объектов каталога Azure AD

Свойства объектов каталога ведут себя по-разному в отношении поддержки параметров запросов. Ниже приведены распространенные сценарии для объектов каталога:

+ Запросы, поддерживаемые по умолчанию, также поддерживаются в расширенных запросах, но в конечном итоге ответ будет согласованным.
+ Оператор `in` поддерживается по умолчанию, когда `eq` оператор поддерживается по умолчанию.
+ Оператор `endsWith` поддерживается только расширенными запросами и свойствами `mail` и `userPrincipalName`.
+ Операторы отрицания `not` и `ne` поддерживаются только расширенными запросами.
  + Все свойства, поддерживающие оператор `eq`, также поддерживают операторы `ne` или `not`.
  + Для запросов, использующих лямбда-оператор `any`, используйте оператор `not`. См. [Фильтрация с помощью лямбда-операторов](/graph/query-parameters#filter-using-lambda-operators)..

В следующих таблицах обобщается поддержка `$filter` операторов по свойствам объектов каталога, поддерживаемых расширенными возможностями запросов.

### <a name="legend"></a>Условные обозначения

+ ![Работает по умолчанию. Не требуются расширенные параметры запроса.](../concepts/images/yesandnosymbols/greencheck.svg) Оператор `$filter` по умолчанию работает для этого свойства.
+ ![Требуются расширенные параметры запроса.](../concepts/images/yesandnosymbols/whitecheck-in-greencircle.svg) Оператору `$filter` **требуются** *расширенные параметры запроса,* которые:
  + Заголовок `ConsistencyLevel=eventual`
  + Строка запроса `$count=true`
+ ![Не поддерживаются.](../concepts/images/yesandnosymbols/no.svg) Оператор `$filter` не поддерживается для этого свойства. [Отправьте свой отзыв,](https://aka.ms/MsGraphAADSurveyDocs) чтобы запросить поддержку этого свойства `$filter` для сценариев.
+ Пустые ячейки указывают, что запрос является недействительным для этого свойства.
+ Столбец **значение null** указывает, что свойство является недействительным и фильтруемым с помощью `null`.
+ Свойства, не указанные здесь, совсем не `$filter` поддерживаются.

[!INCLUDE [filter-directory-objects](../includes/filter-directory-objects.md)]

## <a name="error-handling-for-advanced-queries-on-directory-objects"></a>Обработка ошибок расширенных запросов к объектам каталога

Подсчет объектов каталога поддерживается только с использованием расширенных параметров запросов. Если заголовок `ConsistencyLevel=eventual` не указан, запрос возвращает ошибку, когда используется сегмент URL-адреса `$count`, или автоматически игнорирует параметр запроса `$count` (`?$count=true`), если он используется.

<!-- {
  "blockType": "request",
  "name": "get_users_count_bad"
} -->
```http
https://graph.microsoft.com/v1.0/users/$count
```

<!-- {
  "blockType": "response",
  "@odata.type": "odata.error",
  "expectError": true
} -->
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

Для объектов каталога `$search` поддерживается только в расширенных запросах. Если заголовок **ConsistencyLevel** не указан, запрос возвращает ошибку.

<!-- {
  "blockType": "request",
  "name": "get_applications_search_displayName"
} -->
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

<!-- {
  "blockType": "request",
  "name": "get_users_filer_endsWith"
} -->
```http
https://graph.microsoft.com/v1.0/users?$filter=endsWith(mail,'@outlook.com')
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

<!-- {
  "blockType": "request",
  "name": "get_groups_unindexed_bad"
} -->
```http
https://graph.microsoft.com/beta/groups?$filter=createdDateTime ge 2021-11-01&$count=true
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

При этом необходимо отметить, что указанные в запросе параметры могут просто не сработать.
Это может произойти, если не поддерживаются либо сами параметры, либо их сочетание.
В таких случаях необходимо проверить возвращенные запросом данные и определить, дали ли указанные параметры запроса желаемый результат. В следующем примере параметр `@odata.count` отсутствует, даже если запрос успешно выполняется.

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

+ [Настройка откликов с помощью параметров запроса](/graph/query-parameters)
+ [Ограничения параметров запроса](known-issues.md#some-limitations-apply-to-query-parameters)
+ [Использование параметра запроса $search для сопоставления с условием поиска](/graph/search-query-parameter#using-search-on-directory-object-collections)
+ [Обзор расширенных возможностей запроса для объектов каталога Azure AD с помощью SDK .NET](https://github.com/microsoftgraph/dotnet-aad-query-sample/)
