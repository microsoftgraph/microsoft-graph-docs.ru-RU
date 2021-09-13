---
title: Вызов API Microsoft Graph
description: 'Для доступа к ресурсу Microsoft Graph и работы с ним необходимо вызвать и указать URL-адреса ресурса, используя одну из указанных ниже операций.   '
ms.localizationpriority: medium
author: ananmishr
ms.prod: cloud-communications
ms.openlocfilehash: 4a09b9b39b41e4f3678abb54fb0de011aa49974d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134089"
---
# <a name="calling-the-microsoft-graph-api"></a>Вызов API Microsoft Graph

Для доступа к ресурсу Microsoft Graph и работы с ним необходимо вызвать и указать URL-адреса ресурса, используя одну из указанных ниже операций.   

- GET
- POST
- PATCH
- PUT
- DELETE 

Во всех запросах API Microsoft Graph используется следующий базовый шаблон URL-адреса:

```
    https://graph.microsoft.com/{version}/{resource}?[query_parameters]
```

В этом URL-адресе:

- `https://graph.microsoft.com` — это конечная точка API Microsoft Graph.
- `{version}` — это целевая версия службы, например `v1.0` или `beta`.
- `{resource}` — это сегмент ресурсов или путь, например:
  - `users`, `groups`, `devices`, `organization`
  - псевдоним `me`, который сопоставляется с вошедшим пользователем;
  - ресурсы, принадлежащие пользователю, такие как `me/events`, `me/drive` или `me/messages`;
  - псевдоним `myOrganization`, который сопоставляется с клиентом организации вошедшего пользователя.
- `[query_parameters]` представляет дополнительные параметры запроса, такие как `$filter` и `$select`.

При желании вы также можете указать клиент в составе запроса. Если используется псевдоним `me`, не указывайте клиент. Список распространенных запросов см. в статье [Обзор Microsoft Graph](overview.md).

## <a name="microsoft-graph-api-metadata"></a>Метаданные API Microsoft Graph
Документ метаданных ($metadata) публикуется в корневом каталоге службы. Например, по указанным ниже URL-адресам можно просмотреть сервисный документ для версии 1.0 и бета-версии.

Метаданные API Microsoft Graph `v1.0`.
```
    https://graph.microsoft.com/v1.0/$metadata
```
Метаданные API Microsoft Graph `beta`.
```
    https://graph.microsoft.com/beta/$metadata
```

Метаданные помогают просматривать и анализировать модель данных Microsoft Graph, в том числе типы и наборы сущностей, сложные типы и перечисления, входящие в состав запроса и пакетов ответа, отправляемых в службу Microsoft Graph и из нее.
С помощью метаданных вы сможете понять связи между сущностями в Microsoft Graph и создать URL-адреса для перехода между ними.
Такая взаимосвязь на основе навигации является уникальной характеристикой Microsoft Graph.

Названия ресурсов URL-адреса пути, параметры запросов, а также параметры и значения действий указываются без учета регистра. Однако назначаемые значения, идентификаторы объектов и другие значения в кодировке base64 указываются с учетом регистра.

В следующих разделах представлено несколько базовых шаблонов программирования вызовов к API Microsoft Graph.

## <a name="navigate-from-a-set-to-a-member"></a>Переход от набора к элементу

Чтобы просмотреть сведения о пользователе, необходимо получить объект `User` из коллекции `users` для конкретного пользователя, на которого указывает идентификатор, используя HTTPS-запрос GET. Для объекта `User` в качестве идентификатора можно использовать свойство `id` или `userPrincipalName`. В следующем примере запроса в качестве идентификатора пользователя используется значение `userPrincipalName`. 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer <access_token>
```

При успешном выполнении действия вы получите ответ 200 OK, содержащий полезные данные с представлением ресурса user, как показано ниже.

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 982

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
    "city": "Redmond",
    "country": "USA",
    "department": "Help Center",
    "displayName": "John Doe",
    "givenName": "John",
    "userPrincipalName": "john.doe@contoso.onmicrosoft.com",

    ... 
}
```


## <a name="project-from-an-entity-to-properties"></a>Проекция из объекта на свойства
Чтобы получить только биографические сведения пользователя, например предоставленное им описание в разделе _Обо мне_ и указанные навыки, вы можете добавить в предыдущий запрос параметр _select_. Например:

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer <access_token>
```

При успешном ответе возвращаются состояние 200 OK и полезные данные в следующем формате:

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 169

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "aboutMe": "A cool and nice guy.",
    "displayName": "John Doe",
    "skills": [
        "n-Lingual",
        "public speaking",
        "doodling"
    ]
}
```

Здесь возвращаются не наборы свойств для объекта `user`, а только свойства `aboutMe`, `displayName` и `skills`.

## <a name="traverse-to-another-resource-via-relationship"></a>Переход к другому ресурсу с помощью отношения
Руководитель состоит в отношении `directReports` со своими подчиненными. Чтобы запросить список подчиненных пользователя, можно использовать приведенный ниже HTTPS-запрос GET для перехода к целевому объекту с помощью отношения. 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer <access_token>
```

При успешном ответе возвращаются состояние 200 OK и полезные данные в следующем формате:

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 152
    
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "c37b074d-fe9d-4e68-83ad-b4401d3be174",
    "department": "Sales & Marketing",
    "displayName": "Bonnie Kearney",

    ...
}
```

Аналогичным образом вы можете воспользоваться отношением, чтобы перейти к связанным ресурсам. Например, отношение `user => messages` позволяет перейти от пользователя Azure AD к набору сообщений Outlook. В приведенном ниже примере показано, как это сделать в вызове API REST:


```no-highlight 
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer <access_token>
```

    
При успешном ответе возвращаются состояние 200 OK и полезные данные в следующем формате:


```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
odata-version: 4.0
content-length: 147
    
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/Messages",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$top=1&$skip=1",
  "value": [
    {
      "@odata.etag": "W/\"FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej\"",
      "id": "<id-value>",
      "createdDateTime": "2015-11-14T00:24:42Z",
      "lastModifiedDateTime": "2015-11-14T00:24:42Z",
      "changeKey": "FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej",
      "categories": [],
      "receivedDateTime": "2015-11-14T00:24:42Z",
      "sentDateTime": "2015-11-14T00:24:28Z",
      "hasAttachments": false,
      "subject": "Did you see last night's game?",
      "body": {
        "ContentType": "HTML",
        "Content": "<content>"
      },
      "BodyPreview": "it was great!",
      "Importance": "Normal",
            
       ...
    }
  ]
}
```

## <a name="project-from-entities-to-properties"></a>Проекция из объектов на свойства
Помимо проекции из одного объекта на его свойства, вы также можете применить такой же параметр запроса `select` к коллекции объектов, чтобы спроецировать их на коллекцию некоторых их свойств. Например, чтобы запросить имена элементов на диске вошедшего пользователя, вы можете отправить следующий HTTPS-запрос GET:

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer <access_token>
```

При успешном ответе возвращается код состояния 200 OK и полезные данные, содержащие имена и типы общих файлов, как показано в следующем примере:

```no-highlight 
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/drive/root/children(name,type)",
  "value": [
    {
      "@odata.etag": "\"{896A8E4D-27BF-424B-A0DA-F073AE6570E2},2\"",
      "name": "Shared with Everyone"
    },
    {
      "@odata.etag": "\"{B39D5D2E-E968-491A-B0EB-D5D0431CB423},1\"",
      "name": "Documents"
    },
    {
      "@odata.etag": "\"{9B51EA38-3EE6-4DC1-96A6-230E325EF054},2\"",
      "name": "newFile.txt"
    }
  ]
}
```

## <a name="query-a-subset-of-users-with-the-filtering-query-option"></a>Запрос подмножества пользователей с помощью параметра фильтрации
Чтобы найти сотрудников, занимающих определенную должность в организации, можно перейти из коллекции пользователей, а затем указать параметр запроса _filter_. Пример:

    
```no-highlight 
GET https://graph.microsoft.com/v1.0/users/?$filter=jobTitle+eq+%27Helper%27 HTTP/1.1
Authorization : Bearer <access_token>
```

При успешном ответе возвращаются код состояния 200 OK и список пользователей, занимающих указанную должность (`'Helper'`), как показано в следующем примере:

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
odata-version: 4.0
content-length: 986

{
    "@odata.context": "https://graph.microsoft.com/v1.0/contoso.onmicrosoft.com/$metadata#users",
    "value": [
        {
            "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
            "city": "Redmond",
            "country": "USA",
            "department": "Help Center",
            "displayName": "Jane Doe",
            "givenName": "Jane",
            "jobTitle": "Helper",
            ......
            "mailNickname": "Jane",
            "mobile": null,
            "otherMails": [
                "jane.doe@contoso.onmicrosoft.com"
            ],
            ......
            "surname": "Doe",
            "usageLocation": "US",
            "userPrincipalName": "help@contoso.onmicrosoft.com",
            "userType": "Member"
        },
        
        ...
    ]
}
```

## <a name="call-actions-or-functions"></a>Вызов действий и функций
Microsoft Graph также поддерживает _действия_ и _функции_ для управления ресурсами с использованием методов, которые сложно совмещать со стандартными методами HTTP. Например, с помощью приведенного ниже HTTPS-запроса POST вошедший пользователь (`me`) может отправить электронное сообщение.
```no-highlight 
POST https://graph.microsoft.com/v1.0/me/sendMail HTTP/1.1
authorization: bearer <access_token>
content-type: application/json
content-length: 96

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "garthf@a830edad9050849NDA1.onmicrosoft.com"
        }
      }
    ],
    "attachments": [
      {
        "@odata.type": "microsoft.graph.fileAttachment",
        "name": "menu.txt",
        "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
      }
    ]
  },
  "saveToSentItems": "false"
}
```

Полезные данные запроса содержат входные данные для действия `sendMail`, которые также определены в документе $metadata.

## <a name="use-microsoft-graph-client-libraries"></a>Использование клиентских библиотек Microsoft Graph
Вам нравятся возможности и удобство пакетов SDK? Вы всегда можете вызывать Microsoft Graph с помощью REST API, но мы также предоставляем пакеты SDK для многих популярных платформ.

Изучите наши [примеры кода и пакеты SDK](https://developer.microsoft.com/graph/code-samples-and-sdks).
