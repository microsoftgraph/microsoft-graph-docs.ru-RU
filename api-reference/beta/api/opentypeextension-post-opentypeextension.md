---
title: Создание открытого расширения
description: Создание расширения open (объект openTypeExtension) и Добавление настраиваемых свойств
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: a654d0bc48bc5f4f83be4adaf258fa3186914745
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642711"
---
# <a name="create-open-extension"></a>Создание открытого расширения

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте расширение open (объект[openTypeExtension](../resources/opentypeextension.md) ) и добавьте настраиваемых свойств в новый или существующий экземпляр поддерживаемые ресурсов.

> **Примечание.** Если вы создаете открытые расширения для ресурсов Outlook, см. раздел **Рекомендации, касающиеся Outlook** в статье [Тип ресурса openTypeExtension](../resources/opentypeextension.md#outlook-specific-considerations).

## <a name="permissions"></a>Разрешения

В зависимости от ресурса, в котором создается расширение, и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Поддерживаемый ресурс | Делегированное (рабочая или учебная учетная запись) | Делегированное (личная учетная запись Майкрософт) | Для приложений |
|:-----|:-----|:-----|:-----|
| [device](../resources/device.md) | Directory.AccessAsUser.All | Не поддерживается | Device.ReadWrite.All |
| [event](../resources/event.md) | Calendars.ReadWrite | Calendars.ReadWrite | Calendars.ReadWrite |
| [group](../resources/group.md) | Group.ReadWrite.All | Не поддерживается | Group.ReadWrite.All |
| [event](../resources/event.md) для групп | Group.ReadWrite.All | Не поддерживается | Не поддерживается |
| [post](../resources/post.md) для групп | Group.ReadWrite.All | Не поддерживается | Group.ReadWrite.All |
| [message](../resources/message.md) | Mail.ReadWrite | Mail.ReadWrite | Mail.ReadWrite | 
| [organization](../resources/organization.md) | Directory.AccessAsUser.All | Не поддерживается | Не поддерживается |
| [contact](../resources/contact.md) (личный контакт) | Contacts.ReadWrite | Contacts.ReadWrite | Contacts.ReadWrite |
| [user](../resources/user.md) | User.ReadWrite.All | User.ReadWrite | User.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

### <a name="create-an-extension-in-a-new-resource-instance"></a>Создание расширения в новом экземпляре ресурса

Используйте такой же запрос REST, как для создания экземпляра.

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

>**Примечание.** В этом синтаксисе показаны некоторые распространенные способы создания поддерживаемых экземпляров ресурса. Все другие варианты синтаксиса POST, позволяющие создавать эти экземпляры ресурса, поддерживают создание открытых расширений этих экземпляров подобным образом.

В разделе [Текст запроса](#request-body) показано, как включить свойства нового экземпляра ресурса _и расширение_ в текст запроса.

### <a name="create-an-extension-in-an-existing-resource-instance"></a>Создание расширения в существующем экземпляре ресурса

Идентифицируйте экземпляр ресурса в запросе и выполните операцию `POST` для свойства навигации **extensions**.

<!-- { "blockType": "ignored" } -->
```http
POST /administrativeunits/{id}/extensions
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
```

>**Примечание.** В этом синтаксисе показаны некоторые распространенные способы определения экземпляра ресурса, чье расширение нужно создать. Все другие варианты синтаксиса, позволяющие определить эти экземпляры ресурса, поддерживают создание открытых расширений этих экземпляров подобным образом.

В разделе [Текст запроса](#request-body) показано, как включить _расширение_ в текст запроса.

## <a name="path-parameters"></a>Параметры пути

|**Параметр**|**Тип**|**Описание**|
|:-----|:-----|:-----|
|id|string|Уникальный идентификатор объекта в соответствующей коллекции. Обязательный.|

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Значение |
|:---------------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type | application/json |

## <a name="request-body"></a>Текст запроса

Предоставьте JSON в тексте [openTypeExtension](../resources/opentypeextension.md)следующие обязательные пар имя значение и любые дополнительные пользовательские данные. JSON полезных данных может быть простых типов или массивами простых типов.

| Имя       | Значение |
|:---------------|:----------|
| @odata.type | Microsoft.Graph.OpenTypeExtension |
| extensionName | %уникальная_строка% |

При создании расширения в _новом_ экземпляре ресурса предоставьте не только объект **openTypeExtension**, но и представление JSON соответствующих свойств для создания этого экземпляра ресурса.

## <a name="response"></a>Ответ

### <a name="response-code"></a>Код ответа

В зависимости от операции можно использовать код ответа `201 Created` или `202 Accepted`.

При создании расширения с использованием такой же операции, как для создания экземпляра ресурса, операция возвращает такой же код ответа, что и при создании экземпляра ресурса без расширения.
Изучите соответствующие статьи о создании экземпляров, перечисленные [выше](#create-an-extension-in-a-new-resource-instance).

### <a name="response-body"></a>Текст отклика

| Сценарий       | Ресурс  | Текст отклика |
|:---------------|:----------|:--------------|
| Создание расширения с явным созданием _нового_ экземпляра ресурса | [contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md) | Включает новый экземпляр, дополненный объектом [openTypeExtension](../resources/opentypeextension.md). |
| Создание расширения с неявным созданием экземпляра ресурса | [post](../resources/post.md) | Ответ содержит только код ответа без текста. |
| Создание расширения в _существующем_ экземпляре ресурса | Все поддерживаемые ресурсы | Включает объект **openTypeExtension**. |

## <a name="example"></a>Пример

### <a name="request-1"></a>Запрос 1

В первом примере сообщение и расширение создаются в одном запросе. Текст запроса включает следующие данные:

- Свойства **subject**, **body** и **toRecipients**, характерные для нового сообщения.
- Данные для расширения:

  - Тип `Microsoft.Graph.OpenTypeExtension`.
  - Имя расширения "Com.Contoso.Referral".
  - Дополнительные данные, хранящиеся в виде трех настраиваемых свойств в полезных данных JSON: `companyName`, `expirationDate` и `dealValue`.

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages

{
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "You should be proud!"
  },
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com"
      }
    }
  ],
  "extensions": [
    {
      "@odata.type": "Microsoft.Graph.OpenTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

### <a name="response-1"></a>Отклик 1

Ниже представлен отклик для первого примера. Текст отклика включает свойства нового сообщения и следующие данные для нового расширения:

- Свойство **id** с полным именем `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.
- Стандартное свойство **extensionName**, указанное в запросе.
- Пользовательские данные из запроса, сохраненные в виде 3 настраиваемых свойств.

Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')",
  "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj\"",
  "id": "AAMkAGEbs88AAB84uLuAAA=",
  "createdDateTime": "2015-10-30T03:03:43Z",
  "lastModifiedDateTime": "2015-10-30T03:03:43Z",
  "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj",
  "categories": [ ],
  "receivedDateTime": "2015-10-30T03:03:43Z",
  "sentDateTime": "2015-10-30T03:03:43Z",
  "hasAttachments": false,
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r
\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nYou should be proud!\r\n</body>\r
\n</html>\r\n"
  },
  "bodyPreview": "You should be proud!",
  "importance": "Normal",
  "parentFolderId": "AQMkAGEwAAAIBDwAAAA==",
  "sender": null,
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com",
        "name": "John Doe"
      }
    }
  ],
  "ccRecipients": [ ],
  "bccRecipients": [ ],
  "replyTo": [ ],
  "conversationId": "AAQkAGEFGugh3SVdMzzc=",
  "isDeliveryReceiptRequested": false,
  "isReadReceiptRequested": false,
  "isRead": true,
  "isDraft": true,
  "webLink": "https://outlook.office.com/owa/?
ItemID=AAMkAGEbs88AAB84uLuAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
  "inferenceClassification": "Focused",
  "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
      "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
      "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

****

### <a name="request-2"></a>Запрос 2

Во втором примере показано создание расширения в указанном сообщении. Текст запроса включает следующие данные для расширения:

- Тип `Microsoft.Graph.OpenTypeExtension`.
- Имя расширения "Com.Contoso.Referral".
- Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `dealValue` и `expirationDate`.

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```

### <a name="response-2"></a>Отклик 2

Ниже представлен отклик для второго примера. Текст отклика включает следующие данные для нового расширения:

- Свойство по умолчанию **extensionName**.
- Свойство **id** с полным именем `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.
- Сохраняемые пользовательские данные.

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

### <a name="request-3"></a>Запрос 3

В третьем примере показано создание расширения в указанном событии группы. Текст запроса включает следующие данные для расширения:

- Тип `Microsoft.Graph.OpenTypeExtension`.
- Имя расширения "Com.Contoso.Deal".
- Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `dealValue` и `expirationDate`.

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

### <a name="response-3"></a>Отклик 3

Ниже представлен отклик из третьего примера.

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

### <a name="request-4"></a>Запрос 4

В четвертом примере показано создание расширения в новой записи группы с помощью одного вызова действия **reply** для существующей записи группы. Действие **reply** создает запись и внедряет в нее новое расширение. Текст запроса включает свойство **post**, которое, в свою очередь, содержит свойство **body** новой записи и следующие данные для нового расширения:

- Тип `Microsoft.Graph.OpenTypeExtension`.
- Имя расширения "Com.Contoso.HR".
- Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `expirationDate` и массив строк `topPicks`.

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=')/reply

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
      "extensionName": "Com.Contoso.HR",
      "companyName": "Contoso",
      "expirationDate": "2015-07-03T13:04:00.000Z",
      "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
      ]
    }
  ]
  }
}
```

### <a name="response-4"></a>Отклик 4

Ниже представлен отклик из четвертого примера. При успешном создании расширения в новой записи группы возвращается только код отклика HTTP 202.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Content-type: text/plain
Content-Length: 0
```

****

### <a name="request-5"></a>Запрос 5

В пятом примере показано создание расширения в новой записи группы с помощью той же операции POST, которая создает беседу. Операция POST создает беседу, цепочку и запись, а также внедряет в эту запись новое расширение. Текст отклика включает свойства **Topic** и **Threads**, а также дочерний объект **post** для новой беседы. Объект **post**, в свою очередь, содержит свойство **body** новой записи и следующие данные расширения:

- Тип `Microsoft.Graph.OpenTypeExtension`.
- Имя расширения "Com.Contoso.HR".
- Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `expirationDate` и массив строк `topPicks`.

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations

{
  "Topic": "Does anyone have a second?",
  "Threads": [
    {
      "Posts": [
        {
          "Body": {
            "ContentType": "HTML",
            "Content": "This is urgent!"
          },
          "Extensions": [
            {
              "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
              "extensionName": "Com.Contoso.Benefits",
              "companyName": "Contoso",
              "expirationDate": "2016-08-03T11:00:00.000Z",
              "topPicks": [
                "Employees only",
                "Add spouse or guest",
                "Add family"
              ]
            }
          ]
        }
      ]
    }
  ]
}
```

### <a name="response-5"></a>Отклик 5

Ниже представлен отклик из пятого примера, содержащий новую беседу и идентификатор цепочки. Эта новая цепочка содержит автоматически созданную запись, включающую новое расширение.

Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

Чтобы получить новое расширение, сначала [получите все записи](../api/conversationthread-list-posts.md) из цепочки. Изначально в ней должна быть только одна запись. Затем примените идентификатор записи и имя расширения `Com.Contoso.Benefits`, чтобы [получить расширение](../api/opentypeextension-get.md).

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
    "threads": [
        {
            "id": "AAQkADJDtMUzsf_PdhAAswJOhGVsnkyDtMUzsf_Pdg=="
        }
    ]
}

```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/opentypeextension-post-opentypeextension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
