---
title: Перечисление сообщений в каналах
description: 'Получение списка сообщений (без ответов) в канале команды. Чтобы получить ответы на сообщение, вызовите API перечисления ответов на сообщение или получения ответа на сообщение. '
ms.localizationpriority: high
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9312b6d7f5c39b6b3d5480e539686970a1b299d5
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296488"
---
# <a name="list-channel-messages"></a>Перечисление сообщений в каналах

Пространство имен: microsoft.graph

Получение списка [сообщений](../resources/chatmessage.md) (без ответов) в [канале](../resources/channel.md) [команды](../resources/team.md). 

Чтобы получить ответы на сообщение, вызовите API [перечисления ответов на сообщение](chatmessage-list-replies.md) или [получения ответа на сообщение](chatmessage-get.md). 

> **Примечание**. Этот API поддерживает подписку на изменения (создание, обновление и удаление) с использованием [уведомлений об изменениях](../resources/webhooks.md). Это позволяет вызывающим подписаться на изменения и получать их в режиме реального времени. Дополнительные сведения см. в разделе [Получение уведомлений о сообщениях](/graph/teams-changenotifications-chatmessage).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|---------|-------------|
|Делегированные (рабочая или учебная учетная запись)| ChannelMessage.Read.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение| ChannelMessage.Read.Group*, ChannelMessage.Read.All |

> **Примечание**. Разрешения, помеченные звездочкой (*), используют [согласие для конкретных ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

> [!NOTE]
> Перед вызовом этого API с разрешениями приложения необходимо запросить доступ. Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает указанные ниже [параметры запросов OData](/graph/query-parameters).

| Имя      | Описание          |
|:----------|:---------------------|
| [$top](/graph/query-parameters#top-parameter)| Примените `$top`, чтобы указать количество сообщений канала, возвращаемых на страницу в отклике. Размер страницы по умолчанию — 20 сообщений. Вы можете расширить до 50 сообщений канала на страницу. |
| [$expand](/graph/query-parameters#expand)  | Примените `$expand`, чтобы получить свойства сообщений канала, которые являются ответами. По умолчанию отклик может включать до 1000 ответов. Для операции, которая расширяет сообщения канала с более чем 1000 ответов, используйте URL-адрес запроса, возвращенный в `replies@odata.nextLink`, чтобы получить следующую страницу ответов. |

Другие [параметры запроса OData](/graph/query-parameters) в настоящее время не поддерживаются.

> **Примечание.** Метод [GET /teams/{team-id}/channels/{channel-id}/messages/delta](chatmessage-delta.md) поддерживает фильтрацию по дате, предоставляя схожие данные с методом GET /teams/{team-id}/channels/{channel-id}/messages.

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-request-with-top-query-parameter-and-without-optional-prefer-header"></a>Пример 1: Запрос с параметром запроса $top и без необязательного заголовка Prefer

#### <a name="request"></a>Запрос

Ниже приведен пример запроса с опцией запроса $top и без необязательного заголовка Prefer.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_listchannelmessages_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages?top=3
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-listchannelmessages-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-listchannelmessages-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-listchannelmessages-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-listchannelmessages-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-listchannelmessages-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-listchannelmessages-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
Ниже приведен пример запроса. `@odata.nextLink` в отклике можно использовать для получения следующей страницы сообщений.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages",
    "@odata.count": 3,
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages?$skiptoken=%5b%7B%22token%22%3a%22%2bRID%3a~vpsQAJ9uAC047gwAAACcBQ%3d%3d%23RT%3a1%23TRC%3a20%23RTD%3aAyAER1ygxSHVHGAn2S99BTI6OzViOjZnOGU5ZWM1ZDVmOGdiZjk2OGNkZmNmMTczNGY3QXVpc2ZiZS91YmR3MzwyNzIyNDY2OTU0NTg6AA%3d%3d%23ISV%3a2%23IEO%3a65551%23QCF%3a3%23FPC%3aAggEAAAAcBYAABUFAADQKgAABAAAAHAWAAACALu4GwAAAHAWAAACAPSTMwAAAHAWAACaAFWa84BXgQKAEIAMgBaAE4AUgAuAAoAIwAIgACAAAiAACAABACCAAAEVgBSAI4AYgA%2bAGQAEEAAQAAEABACAAAIEEBBAACAYgB%2bAH4AbgBqACoAHwAICCBAEEIAAAgEQAACAIoAZgB2ADoAMgAKAPoAZgB2AJoAXgBIAgiAAQUqLF4AJgALACARAgBCACoAfgB6AIwABgYCQAAFXAAAAcBYAAAYA%2f50ZgGeEXwAAAHAWAAAEAPaBS4V7AAAAcBYAAAIA1aSJAAAAcBYAAAIAtLmbAAAAcBYAAAIAqKXdAAAAcBYAAAQAppUugOMAAABwFgAABADQoAWA6wAAAHAWAAAEABGl94M5AAAA0CoAAAYA6pF7iYOBaQIAANAqAAAcAEUPAMAAMAACAQCBAHQAADDAgCAAQgByAQAzUJDRBAAA0CoAAAQAETwKAA4FAADQKgAAAgBekRUFAADQKgAAHAB2pQCABYAMgJeAH4ATgAGAvIIIgASABIAFgCWA%22%2c%22range%22%3a%7B%22min%22%3a%2205C1D79B33ADE4%22%2c%22max%22%3a%2205C1D7A52F89EC%22%7D%7D%5d",
    "value": [
        {
            "id": "1616965872395",
            "replyToId": null,
            "etag": "1616965872395",
            "messageType": "message",
            "createdDateTime": "2021-03-28T21:11:12.395Z",
            "lastModifiedDateTime": "2021-03-28T21:11:12.395Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616965872395?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616965872395&parentMessageId=1616965872395",
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "Hello World <at id=\"0\">Jane Smith</at>"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Jane Smith",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
                            "displayName": "Jane Smith",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
            "reactions": []
        },
        {
            "id": "1616963377068",
            "replyToId": null,
            "etag": "1616963377068",
            "messageType": "message",
            "createdDateTime": "2021-03-28T20:29:37.068Z",
            "lastModifiedDateTime": "2021-03-28T20:29:37.068Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616963377068?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616963377068&parentMessageId=1616963377068",
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div><div><div><span><img height=\"145\" src=\"https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents/aWQ9eF8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZC92aWV3cy9pbWdv/$value\" width=\"131\" style=\"vertical-align:bottom; width:131px; height:145px\"></span><div>&nbsp;</div></div><div><div><span><img height=\"65\" src=\"https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents/aWQ9eF8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNC92aWV3cy9pbWdv/$value\" width=\"79\" style=\"vertical-align:bottom; width:79px; height:65px\"></span></div></div></div></div>"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1616883610266",
            "replyToId": null,
            "etag": "1616883610266",
            "messageType": "unknownFutureValue",
            "createdDateTime": "2021-03-28T03:50:10.266Z",
            "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
            "policyViolation": null,
            "from": null,
            "body": {
                "contentType": "html",
                "content": "<systemEventMessage/>"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": [],
            "eventDetail": {
                "@odata.type": "#microsoft.graph.teamDescriptionUpdatedEventMessageDetail",
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "teamDescription": "Team for Microsoft Teams members",
                "initiator": {
                    "application": null,
                    "device": null,
                    "user": {
                        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
                        "displayName": null,
                        "userIdentityType": "aadUser"
                    }
                }
            }
        }
    ]
}
```

### <a name="example-2-request-with-optional-prefer-header"></a>Пример 2. Запрос с необязательным заголовком Prefer

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "get_listchannelmessages_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages?top=3

Prefer: include-unknown-enum-members
```


#### <a name="response"></a>Отклик
Ниже приведен пример отклика, когда `Prefer: include-unknown-enum-members` указывается в заголовке запроса.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages",
    "@odata.count": 3,
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages?$skiptoken=%5b%7B%22token%22%3a%22%2bRID%3a~vpsQAJ9uAC047gwAAACcBQ%3d%3d%23RT%3a1%23TRC%3a20%23RTD%3aAyAER1ygxSHVHGAn2S99BTI6OzViOjZnOGU5ZWM1ZDVmOGdiZjk2OGNkZmNmMTczNGY3QXVpc2ZiZS91YmR3MzwyNzIyNDY2OTU0NTg6AA%3d%3d%23ISV%3a2%23IEO%3a65551%23QCF%3a3%23FPC%3aAggEAAAAcBYAABUFAADQKgAABAAAAHAWAAACALu4GwAAAHAWAAACAPSTMwAAAHAWAACaAFWa84BXgQKAEIAMgBaAE4AUgAuAAoAIwAIgACAAAiAACAABACCAAAEVgBSAI4AYgA%2bAGQAEEAAQAAEABACAAAIEEBBAACAYgB%2bAH4AbgBqACoAHwAICCBAEEIAAAgEQAACAIoAZgB2ADoAMgAKAPoAZgB2AJoAXgBIAgiAAQUqLF4AJgALACARAgBCACoAfgB6AIwABgYCQAAFXAAAAcBYAAAYA%2f50ZgGeEXwAAAHAWAAAEAPaBS4V7AAAAcBYAAAIA1aSJAAAAcBYAAAIAtLmbAAAAcBYAAAIAqKXdAAAAcBYAAAQAppUugOMAAABwFgAABADQoAWA6wAAAHAWAAAEABGl94M5AAAA0CoAAAYA6pF7iYOBaQIAANAqAAAcAEUPAMAAMAACAQCBAHQAADDAgCAAQgByAQAzUJDRBAAA0CoAAAQAETwKAA4FAADQKgAAAgBekRUFAADQKgAAHAB2pQCABYAMgJeAH4ATgAGAvIIIgASABIAFgCWA%22%2c%22range%22%3a%7B%22min%22%3a%2205C1D79B33ADE4%22%2c%22max%22%3a%2205C1D7A52F89EC%22%7D%7D%5d",
    "value": [
        {
            "id": "1616965872395",
            "replyToId": null,
            "etag": "1616965872395",
            "messageType": "message",
            "createdDateTime": "2021-03-28T21:11:12.395Z",
            "lastModifiedDateTime": "2021-03-28T21:11:12.395Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616965872395?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616965872395&parentMessageId=1616965872395",
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "Hello World <at id=\"0\">Jane Smith</at>"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Jane Smith",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
                            "displayName": "Jane Smith",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
            "reactions": []
        },
        {
            "id": "1616963377068",
            "replyToId": null,
            "etag": "1616963377068",
            "messageType": "message",
            "createdDateTime": "2021-03-28T20:29:37.068Z",
            "lastModifiedDateTime": "2021-03-28T20:29:37.068Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616963377068?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616963377068&parentMessageId=1616963377068",
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div><div><div><span><img height=\"145\" src=\"https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents/aWQ9eF8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZC92aWV3cy9pbWdv/$value\" width=\"131\" style=\"vertical-align:bottom; width:131px; height:145px\"></span><div>&nbsp;</div></div><div><div><span><img height=\"65\" src=\"https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents/aWQ9eF8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNC92aWV3cy9pbWdv/$value\" width=\"79\" style=\"vertical-align:bottom; width:79px; height:65px\"></span></div></div></div></div>"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1616883610266",
            "replyToId": null,
            "etag": "1616883610266",
            "messageType": "systemEventMessage",
            "createdDateTime": "2021-03-28T03:50:10.266Z",
            "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
            "policyViolation": null,
            "from": null,
            "body": {
                "contentType": "html",
                "content": "<systemEventMessage/>"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": [],
            "eventDetail": {
                "@odata.type": "#microsoft.graph.teamDescriptionUpdatedEventMessageDetail",
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "teamDescription": "Team for Microsoft Teams members",
                "initiator": {
                    "application": null,
                    "device": null,
                    "user": {
                        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
                        "displayName": null,
                        "userIdentityType": "aadUser"
                    }
                }
            }
        }
    ]
}
```

### <a name="example-3-request-with-top-and-expand-query-options-on-replies"></a>Пример 3. Запрос с параметрами запроса $top и $expand в ответах

#### <a name="request"></a>Запрос

Следующий запрос использует `$top` для возврата одного сообщения канала на страницу и `$expand` для включения ответов на это сообщение канала.

<!-- {
  "blockType": "request",
  "name": "get_listchannelmessages_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages?$top=1&$expand=replies
```

#### <a name="response"></a>Отклик
Следующий отклик показывает одно сообщение канала на странице и включает URL-адрес в `@odata.nextLink` для последующей операции, чтобы получить следующее сообщение в этом канале. 

Отклик включает в себя ответы на это сообщение канала. На практике эта операция может вернуть до 1000 ответов на сообщение канала и включает URL-адрес в `replies@odata.nextLink`, чтобы получить любые дополнительные ответы, превышающие размер страницы 1000. В этом примере предполагается более 1000 ответов в этом сообщении канала, но для удобочитаемости следующий отклик показывает только 3 ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages",
    "@odata.count": 1,
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages?$skiptoken=%5b%7B%22token%22%3a%22%2bRID%3a~vpsQAJ9uAC047gwAAACcBQ%3d%3d%23RT%3a1%23TRC%3a20%23RTD%3aAyAER1ygxSHVHGAn2S99BTI6OzViOjZnOGU5ZWM1ZDVmOGdiZjk2OGNkZmNmMTczNGY3QXVpc2ZiZS91YmR3MzwyNzIyNDY2OTU0NTg6AA%3d%3d%23ISV%3a2%23IEO%3a65551%23QCF%3a3%23FPC%3aAggEAAAAcBYAABUFAADQKgAABAAAAHAWAAACALu4GwAAAHAWAAACAPSTMwAAAHAWAACaAFWa84BXgQKAEIAMgBaAE4AUgAuAAoAIwAIgACAAAiAACAABACCAAAEVgBSAI4AYgA%2bAGQAEEAAQAAEABACAAAIEEBBAACAYgB%2bAH4AbgBqACoAHwAICCBAEEIAAAgEQAACAIoAZgB2ADoAMgAKAPoAZgB2AJoAXgBIAgiAAQUqLF4AJgALACARAgBCACoAfgB6AIwABgYCQAAFXAAAAcBYAAAYA%2f50ZgGeEXwAAAHAWAAAEAPaBS4V7AAAAcBYAAAIA1aSJAAAAcBYAAAIAtLmbAAAAcBYAAAIAqKXdAAAAcBYAAAQAppUugOMAAABwFgAABADQoAWA6wAAAHAWAAAEABGl94M5AAAA0CoAAAYA6pF7iYOBaQIAANAqAAAcAEUPAMAAMAACAQCBAHQAADDAgCAAQgByAQAzUJDRBAAA0CoAAAQAETwKAA4FAADQKgAAAgBekRUFAADQKgAAHAB2pQCABYAMgJeAH4ATgAGAvIIIgASABIAFgCWA%22%2c%22range%22%3a%7B%22min%22%3a%2205C1D79B33ADE4%22%2c%22max%22%3a%2205C1D7A52F89EC%22%7D%7D%5d",
    "value": [
        {
            "id": "1616963377068",
            "replyToId": null,
            "etag": "1616963377068",
            "messageType": "message",
            "createdDateTime": "2021-03-28T20:29:37.068Z",
            "lastModifiedDateTime": "2021-03-28T20:29:37.068Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616963377068?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616963377068&parentMessageId=1616963377068",
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div><div><div><span><img height=\"145\" src=\"https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents/aWQ9eF8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZC92aWV3cy9pbWdv/$value\" width=\"131\" style=\"vertical-align:bottom; width:131px; height:145px\"></span><div>&nbsp;</div></div><div><div><span><img height=\"65\" src=\"https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents/aWQ9eF8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNC92aWV3cy9pbWdv/$value\" width=\"79\" style=\"vertical-align:bottom; width:79px; height:65px\"></span></div></div></div></div>"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": [],
            "replies@odata.count": 3,
            "replies@odata.nextLink": "https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/replies?$skiptoken=MSwwLDE2NDQ0MzkzODAxNDU",
            "replies": [
                {
                    "id": "1616989753153",
                    "replyToId": "1616963377068",
                    "etag": "1616989753153",
                    "messageType": "message",
                    "createdDateTime": "2021-03-29T03:49:13.153Z",
                    "lastModifiedDateTime": "2021-03-29T03:49:13.153Z",
                    "lastEditedDateTime": null,
                    "deletedDateTime": null,
                    "subject": null,
                    "summary": null,
                    "chatId": null,
                    "importance": "normal",
                    "locale": "en-us",
                    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616989753153?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616989753153&parentMessageId=1616989510408",
                    "policyViolation": null,
                    "eventDetail": null,
                    "from": {
                        "application": null,
                        "device": null,
                        "user": {
                            "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                            "displayName": "Robin Kline",
                            "userIdentityType": "aadUser"
                        }
                    },
                    "body": {
                        "contentType": "text",
                        "content": "Reply3"
                    },
                    "channelIdentity": {
                        "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                        "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
                    },
                    "attachments": [],
                    "mentions": [],
                    "reactions": []
                },
                {
                    "id": "1616989750004",
                    "replyToId": "1616963377068",
                    "etag": "1616989750004",
                    "messageType": "message",
                    "createdDateTime": "2021-03-29T03:49:10.004Z",
                    "lastModifiedDateTime": "2021-03-29T03:49:10.004Z",
                    "lastEditedDateTime": null,
                    "deletedDateTime": null,
                    "subject": null,
                    "summary": null,
                    "chatId": null,
                    "importance": "normal",
                    "locale": "en-us",
                    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616989750004?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616989750004&parentMessageId=1616989510408",
                    "policyViolation": null,
                    "eventDetail": null,
                    "from": {
                        "application": null,
                        "device": null,
                        "user": {
                            "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                            "displayName": "Robin Kline",
                            "userIdentityType": "aadUser"
                        }
                    },
                    "body": {
                        "contentType": "text",
                        "content": "Reply2"
                    },
                    "channelIdentity": {
                        "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                        "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
                    },
                    "attachments": [],
                    "mentions": [],
                    "reactions": []
                },
                {
                    "id": "1616989747416",
                    "replyToId": "1616963377068",
                    "etag": "1616989747416",
                    "messageType": "message",
                    "createdDateTime": "2021-03-29T03:49:07.416Z",
                    "lastModifiedDateTime": "2021-03-29T03:49:07.416Z",
                    "lastEditedDateTime": null,
                    "deletedDateTime": null,
                    "subject": null,
                    "summary": null,
                    "chatId": null,
                    "importance": "normal",
                    "locale": "en-us",
                    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616989747416?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616989747416&parentMessageId=1616989510408",
                    "policyViolation": null,
                    "eventDetail": null,
                    "from": {
                        "application": null,
                        "device": null,
                        "user": {
                            "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                            "displayName": "Robin Kline",
                            "userIdentityType": "aadUser"
                        }
                    },
                    "body": {
                        "contentType": "text",
                        "content": "Reply1"
                    },
                    "channelIdentity": {
                        "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                        "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
                    },
                    "attachments": [],
                    "mentions": [],
                    "reactions": []
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
  "description": "List channel messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

