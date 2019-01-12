---
title: Просмотр ресурсов в Microsoft Graph
description: Помимо чтения и записи данных с помощью API Microsoft Graph, вы можете использовать шаблоны запросов для просмотра ресурсов в Microsoft Graph. Документ метаданных поможет вам разобраться в модели данных ресурсов и отношений в Microsoft Graph.
localization_priority: Priority
ms.openlocfilehash: dc4cafc00516f4222ba6ec860dd45ff96d608dd8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863835"
---
# <a name="traverse-microsoft-graph"></a>Просмотр ресурсов в Microsoft Graph

Помимо чтения и записи данных с помощью API Microsoft Graph, вы можете использовать шаблоны запросов для просмотра ресурсов в Microsoft Graph. Документ метаданных поможет вам разобраться в модели данных ресурсов и отношений в Microsoft Graph.

## <a name="microsoft-graph-api-metadata"></a>Метаданные API Microsoft Graph

Документ метаданных ($metadata) публикуется в корневом каталоге службы. По указанным ниже URL-адресам можно просмотреть сервисный документ для версии 1.0 и бета-версии API Microsoft Graph.

**Метаданные API Microsoft Graph 1.0**
```
    https://graph.microsoft.com/v1.0/$metadata
```

**Метаданные API Microsoft Graph (бета-версия)**

```
    https://graph.microsoft.com/beta/$metadata
```

Метаданные позволяют разобраться в модели данных Microsoft Graph, в том числе типах объектов, сложных типах и перечислениях, из которых состоят ресурсы, представленные в пакетах запросов и откликов.

С помощью метаданных можно узнать о связях между объектами в Microsoft Graph и создать URL-адреса для перехода между ними.

Имена ресурсов URL-адреса пути, параметры запросов, а также параметры и значения действий указываются без учета регистра. Но назначаемые значения, идентификаторы объектов и другие значения в кодировке Base64 указываются с учетом регистра.

## <a name="view-a-collection-of-resources"></a>Просмотр коллекции ресурсов

Microsoft Graph позволяет просматривать ресурсы в клиенте с помощью HTTP-запросов GET. Отклик на запрос включает свойства каждого ресурса, при этом каждый ресурс определяется по соответствующему идентификатору. ИД ресурса может быть GUID, его формат обычно разнится в зависимости от типа ресурса. 

Например, можно получить коллекцию объектов user, определенных в клиенте:

```no-highlight 
GET https://graph.microsoft.com/v1.0/users HTTP/1.1
Authorization : Bearer {access_token}
```

При успешном выполнении запроса будет получен отклик 200 OK, который содержит полезные данные с коллекцией ресурсов [user](/graph/api/resources/user?view=graph-rest-1.0). Каждый объект user идентифицируется по свойству **id** и сопровождается свойствами по умолчанию. Полезные данные, показанные ниже, усечены для краткости.

```no-highlight 
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "value":[
    {
      "id":"f71f1f74-bf1f-4e6b-b266-c777ea76e2c7",
      "businessPhones":[

      ],
      "displayName":"CIE Administrator",
      "givenName":"CIE",
      "jobTitle":null,
      "mail":"admin@contoso.onmicrosoft.com",
      "mobilePhone":"+1 3528700812",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Administrator",
      "userPrincipalName":"admin@contoso.onmicrosoft.com"
    },
    {
      "id":"d66f2902-9d12-4ff8-ab01-21ec6706079f",
      "businessPhones":[

      ],
      "displayName":"Alan Steiner",
      "givenName":"Alan",
      "jobTitle":"VP Corporate Marketing",
      "mail":"alans@contoso.onmicrosoft.com",
      "mobilePhone":null,
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Steiner",
      "userPrincipalName":"alans@contoso.onmicrosoft.com"
    }
  ]
}
```

Microsoft Graph позволяет также просматривать коллекции, переходя к нужному отношению, которым связаны ресурсы. Например, применяя свойство навигации **mailFolders** объекта user, вы можете запрашивать коллекцию ресурсов [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) в почтовом ящике пользователя:

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/mailfolders HTTP/1.1
Authorization : Bearer {access_token}
```

При успешном выполнении запроса будет получен отклик 200 OK, который содержит полезные данные с коллекцией ресурсов [mailFolder](/graph/api/resources/user?view=graph-rest-1.0). Каждый объект **mailFolder** определяется по его свойству **id** и сопровождается другими свойствами. Полезные данные, показанные ниже, усечены для краткости.

```no-highlight 
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('16f5a7b6-5a15-4568-aa5a-31bb117e9967')/mailFolders",
  "value":[
    {
      "id":"AAMkADRm9AABDGisXAAA=",
      "displayName":"Archive",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AQMkADRm0AAAIBXAAAAA==",
      "displayName":"Sales reports",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AAMkADRCxI9AAAT6CAIAAA=",
      "displayName":"Conversation History",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":1,
      "unreadItemCount":0,
      "totalItemCount":0
    }
  ]
}
```




## <a name="view-a-specific-resource-from-a-collection-by-id"></a>Просмотр ресурса из коллекции по идентификатору

Еще раз приведем ресурс **user** в качестве примера. Чтобы просмотреть сведения об определенном пользователе, отправьте HTTPS-запрос GET, указав идентификатор объекта user. Для объекта **user** в качестве идентификатора можно использовать свойство **id** или **userPrincipalName**. В следующем примере запроса указано значение **userPrincipalName** как идентификатор user. 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer {access_token}
```

При успешном выполнении запроса будет получен отклик 200 OK, содержащий полезные данные с представлением ресурса user, как показано ниже.

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

## <a name="read-specific-properties-of-a-resource"></a>Чтение определенных свойств ресурса
Чтобы получить только биографические данные пользователя, например предоставленное им описание в разделе _Обо мне_ и набор квалификационных навыков, в предыдущий запрос можно добавить параметр [$select](query-parameters.md), как показано в следующем примере. 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer {access_token}
```

При успешном выполнении запроса в отклике возвращаются полезные данные и состояние 200 OK, как показано ниже.

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
Здесь возвращаются не полные наборы свойств для объекта **user**, а только основные свойства **aboutMe**, **displayName** и **skills**.

## <a name="read-specific-properties-of-the-resources-in-a-collection"></a>Чтение отдельных свойств ресурсов в коллекции
Вы можете не только просматривать отдельные свойства одного ресурса, но и получить все ее ресурсы только с указанными свойствами, применив к коллекции аналогичный параметр запроса [$select](query-parameters.md). Например, чтобы запросить имена элементов на диске вошедшего пользователя, можно отправить следующий HTTPS-запрос GET.

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer {access_token}
```

При успешном ответе возвращаются код состояния 200 OK и полезные данные, содержащие только имена общих файлов, как показано в следующем примере.

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

## <a name="traverse-from-one-resource-to-another-via-relationship"></a>Переход от одного ресурса к другому с помощью отношения
Руководитель состоит в отношении **directReports** со своими подчиненными. Чтобы запросить список подчиненных пользователя, можно использовать приведенный ниже HTTPS-запрос GET для перехода к целевому объекту с помощью отношения. 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer {access_token}
```

При успешном выполнении запроса в отклике возвращаются полезные данные и состояние 200 OK, как показано ниже.

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

Аналогичным образом можно переходить к ресурсам, используя их отношения. Например, отношение user-messages позволяет перейти от пользователя Azure Active Directory (AD) к набору сообщений Outlook. В приведенном ниже примере показано, как это сделать в вызове REST API.


```no-highlight 
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer {access_token}
```

    
При успешном выполнении запроса в отклике возвращаются полезные данные и состояние 200 OK, как показано ниже.


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
Чтобы просмотреть все отношения для ресурса, откройте метаданные, найдите нужный EntityType и просмотрите все его свойства NavigationProperties.

## <a name="call-functions"></a>Вызов функций
Microsoft Graph также поддерживает _функции_ для выполнения с ресурсами действий, отличных от простых операций CRUD (создание, чтение, обновление и удаление). Они часто имеют форму HTTPS-запросов POST, принимающих аргументы. Например, с помощью указанной ниже функции вошедший пользователь (`me`) может отправить сообщение электронной почты.

```no-highlight 
POST https://graph.microsoft.com/v1.0/me/sendMail HTTP/1.1
authorization: bearer {access_token}
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

Вы можете просмотреть все доступные функции в метаданных. Они отображаются как функции или действия.

## <a name="use-the-microsoft-graph-sdks"></a>Использование пакетов SDK Microsoft Graph

Вам нравятся возможности и удобство пакетов SDK? Вы всегда можете вызывать Microsoft Graph с помощью REST API, но мы также предоставляем пакеты SDK для многих популярных платформ. Обзор доступных пакетов SDK см. в разделе [Примеры кода и пакеты SDK](https://developer.microsoft.com/graph/code-samples-and-sdks).

## <a name="see-also"></a>См. также

- [Использование API Microsoft Graph](use-the-api.md)
- [Получение токенов аутентификации](auth-overview.md)
