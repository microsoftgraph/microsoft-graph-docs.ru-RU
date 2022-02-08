---
title: 'чаты: getAllMessages'
description: Получение сообщений из всех чатах, в которых пользователь является участником.
author: RamjotSingh
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 34b428e38e36fb1ce8ace217d9daddbc5f898d21
ms.sourcegitcommit: 38e16940da74bda465f890d945f9dc4aa412c6f4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2022
ms.locfileid: "62396977"
---
# <a name="chats-getallmessages"></a>чаты: getAllMessages

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение всех сообщений ото всех [чатов](../resources/chatmessage.md), в которых пользователь является участником, включая чаты с одним участником, групповые чаты и чаты собраний.

[!INCLUDE [teams-model-A-and-B-disclaimer](../../includes/teams-model-A-and-B-disclaimer.md)]

## <a name="permissions"></a>Разрешения

Для вызова этого API требуются указанные ниже разрешения. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись)| Не поддерживается |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается |
|Для приложения | Chat.Read.All, Chat.ReadWrite.All |

> [!NOTE]
> Перед вызовом этого API с разрешениями приложения необходимо запросить доступ. Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | user-principal-name}/chats/getAllMessages
```

## <a name="optional-query-parameters"></a>Необязательные параметры запроса

Вы можете использовать параметр запроса `model`, который поддерживает значения `A` и `B`, в зависимости от предпочитаемой [модели лицензирования и оплаты](/graph/teams-licenses), как показано в следующих примерах.  
Если параметр `model` не указан, будет использоваться [режим оценки](/graph/teams-licenses#evaluation-mode-default-requirements).

```http
GET /users/{id | user-principal-name}/chats/getAllMessages?model=A
GET /users/{id | user-principal-name}/chats/getAllMessages?model=B
```

Эта операция поддерживает [параметры диапазона дат](/graph/query-parameters) для настройки отклика, как показано в следующем примере.

```http
GET /users/{id}/chats/getAllMessages?$top=50&$filter=lastModifiedDateTime gt 2020-06-04T18:03:11.591Z and lastModifiedDateTime lt 2020-06-05T21:00:09.413Z
```

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный. |

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает `200 OK` код отклика и список [chatMessages](../resources/chatmessage.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/getAllMessages
```

### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
   "@odata.count":10,
   "@odata.nextLink":"https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/getAllMessages?$skip=10",
   "value":[
      {
         "@odata.type":"#microsoft.graph.chatMessage",
         "id":"1600457965467",
         "replyToId":null,
         "etag":"1600457965467",
         "messageType":"message",
         "createdDateTime":"2020-09-18T19:39:25.467Z",
         "lastModifiedDateTime":"2020-09-18T19:39:25.467Z",
         "lastEditedDateTime":null,
         "deletedDateTime":null,
         "subject":null,
         "summary":null,
         "chatId":"19:0de69e5e-2da8-4cf2-821f-5e6585b2c65b_5c64e248-3269-4268-a36e-0f80314e9c39@unq.gbl.spaces",
         "importance":"normal",
         "locale":"en-us",
         "webUrl":null,
         "channelIdentity":null,
         "policyViolation":null,
         "eventDetail": null,
         "from":{
            "application":null,
            "device":null,
            "conversation":null,
            "user":{
               "id":"0de69e5e-2da8-4cf2-821f-5e6585b2c65b",
               "displayName":"Richard Wilson",
               "userIdentityType":"aadUser"
            }
         },
         "body":{
            "contentType":"html",
            "content":"<div>\n<blockquote itemscope=\"\" itemtype=\"http://schema.skype.com/Reply\" itemid=\"1600457867820\">\n<strong itemprop=\"mri\" itemid=\"8:orgid:0de69e5e-2da8-4cf2-821f-5e6585b2c65b\">Richard Wilson</strong><span itemprop=\"time\" itemid=\"1600457867820\"></span>\n<p itemprop=\"preview\">1237</p>\n</blockquote>\n<p>this is a reply</p>\n</div>"
         },
         "attachments":[

         ],
         "mentions":[

         ],
         "reactions":[

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
  "description": "chats: getallmessages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
