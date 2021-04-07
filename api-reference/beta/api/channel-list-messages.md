---
title: Перечисление сообщений в каналах
description: 'Получение списка сообщений (без ответов) в канале команды. Чтобы получить ответы на сообщение, вызовите API перечисления ответов на сообщение или получения ответа на сообщение. '
localization_priority: Priority
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 74df4282a745fbabf11ccdee4fae7d64aeab5dbe
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610863"
---
# <a name="list-channel-messages"></a><span data-ttu-id="25c7b-104">Перечисление сообщений в каналах</span><span class="sxs-lookup"><span data-stu-id="25c7b-104">List channel messages</span></span>

<span data-ttu-id="25c7b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25c7b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25c7b-106">Получение списка [сообщений](../resources/chatmessage.md) (без ответов) в [канале](../resources/channel.md) [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="25c7b-106">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> 

<span data-ttu-id="25c7b-107">Чтобы получить ответы на сообщение, вызовите API [перечисления ответов на сообщение](chatmessage-list-replies.md) или [получения ответа на сообщение](chatmessage-get.md).</span><span class="sxs-lookup"><span data-stu-id="25c7b-107">To get the replies for a message, call the [list message replies](chatmessage-list-replies.md) or the [get message reply](chatmessage-get.md) API.</span></span> 

> <span data-ttu-id="25c7b-108">**Примечание**. Этот API поддерживает подписку на изменения (создание, обновление и удаление) с использованием [уведомлений об изменениях](../resources/webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="25c7b-108">**Note**: This API supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="25c7b-109">Это позволяет вызывающим подписаться на изменения и получать их в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="25c7b-109">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="25c7b-110">Дополнительные сведения см. в разделе [Получение уведомлений о сообщениях](/graph/teams-changenotifications-chatmessage).</span><span class="sxs-lookup"><span data-stu-id="25c7b-110">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatmessage).</span></span>

## <a name="permissions"></a><span data-ttu-id="25c7b-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25c7b-111">Permissions</span></span>

<span data-ttu-id="25c7b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25c7b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25c7b-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25c7b-114">Permission Type</span></span>|<span data-ttu-id="25c7b-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25c7b-115">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="25c7b-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25c7b-116">Delegated (work or school account)</span></span>| <span data-ttu-id="25c7b-117">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25c7b-117">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="25c7b-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25c7b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25c7b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25c7b-119">Not supported.</span></span>|
|<span data-ttu-id="25c7b-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25c7b-120">Application</span></span>| <span data-ttu-id="25c7b-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25c7b-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="25c7b-122">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="25c7b-122">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="25c7b-123">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="25c7b-123">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="25c7b-124">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="25c7b-124">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="25c7b-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25c7b-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="25c7b-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="25c7b-126">Optional query parameters</span></span>

<span data-ttu-id="25c7b-127">Вы можете использовать параметр запроса [$top](/graph/query-parameters#top-parameter) для управления количеством элементов в одном отклике.</span><span class="sxs-lookup"><span data-stu-id="25c7b-127">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="25c7b-128">Максимальное значение для `$top`: 50.</span><span class="sxs-lookup"><span data-stu-id="25c7b-128">Maximum allowed value for `$top` is 50.</span></span>
<span data-ttu-id="25c7b-129">Другие [параметры запроса OData](/graph/query-parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="25c7b-129">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

> <span data-ttu-id="25c7b-130">**Примечание.** Метод [GET /teams/{team-id}/channels/{channel-id}/messages/delta](chatmessage-delta.md) поддерживает фильтрацию по дате, предоставляя схожие данные с методом GET /teams/{team-id}/channels/{channel-id}/messages.</span><span class="sxs-lookup"><span data-stu-id="25c7b-130">**Note:** [GET /teams/{team-id}/channels/{channel-id}/messages/delta](chatmessage-delta.md) supports filtering by date, which provides similar data to    GET /teams/{team-id}/channels/{channel-id}/messages .</span></span>

## <a name="request-headers"></a><span data-ttu-id="25c7b-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25c7b-131">Request headers</span></span>

| <span data-ttu-id="25c7b-132">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25c7b-132">Header</span></span>       | <span data-ttu-id="25c7b-133">Значение</span><span class="sxs-lookup"><span data-stu-id="25c7b-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="25c7b-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25c7b-134">Authorization</span></span>  | <span data-ttu-id="25c7b-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25c7b-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="25c7b-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25c7b-137">Request body</span></span>

<span data-ttu-id="25c7b-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25c7b-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25c7b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="25c7b-139">Response</span></span>

<span data-ttu-id="25c7b-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="25c7b-140">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25c7b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="25c7b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="25c7b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="25c7b-142">Request</span></span>

<span data-ttu-id="25c7b-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25c7b-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="25c7b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="25c7b-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_listchannelmessages_1"
}-->
```
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages
```
# <a name="c"></a>[<span data-ttu-id="25c7b-145">C#</span><span class="sxs-lookup"><span data-stu-id="25c7b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-listchannelmessages-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25c7b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25c7b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-listchannelmessages-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25c7b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25c7b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-listchannelmessages-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25c7b-148">Java</span><span class="sxs-lookup"><span data-stu-id="25c7b-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-listchannelmessages-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="25c7b-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="25c7b-149">Response</span></span>
<span data-ttu-id="25c7b-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25c7b-150">The following is an example of the request.</span></span> <span data-ttu-id="25c7b-151">`nextLink` в отклике можно использовать для получения следующей страницы сообщений.</span><span class="sxs-lookup"><span data-stu-id="25c7b-151">`nextLink` in the response can be used to get the next page of messages.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages?$skiptoken=%5b%7B%22token%22%3a%22%2bRID%3a~vpsQAJ9uAC047gwAAACcBQ%3d%3d%23RT%3a1%23TRC%3a20%23RTD%3aAyAER1ygxSHVHGAn2S99BTI6OzViOjZnOGU5ZWM1ZDVmOGdiZjk2OGNkZmNmMTczNGY3QXVpc2ZiZS91YmR3MzwyNzIyNDY2OTU0NTg6AA%3d%3d%23ISV%3a2%23IEO%3a65551%23QCF%3a3%23FPC%3aAggEAAAAcBYAABUFAADQKgAABAAAAHAWAAACALu4GwAAAHAWAAACAPSTMwAAAHAWAACaAFWa84BXgQKAEIAMgBaAE4AUgAuAAoAIwAIgACAAAiAACAABACCAAAEVgBSAI4AYgA%2bAGQAEEAAQAAEABACAAAIEEBBAACAYgB%2bAH4AbgBqACoAHwAICCBAEEIAAAgEQAACAIoAZgB2ADoAMgAKAPoAZgB2AJoAXgBIAgiAAQUqLF4AJgALACARAgBCACoAfgB6AIwABgYCQAAFXAAAAcBYAAAYA%2f50ZgGeEXwAAAHAWAAAEAPaBS4V7AAAAcBYAAAIA1aSJAAAAcBYAAAIAtLmbAAAAcBYAAAIAqKXdAAAAcBYAAAQAppUugOMAAABwFgAABADQoAWA6wAAAHAWAAAEABGl94M5AAAA0CoAAAYA6pF7iYOBaQIAANAqAAAcAEUPAMAAMAACAQCBAHQAADDAgCAAQgByAQAzUJDRBAAA0CoAAAQAETwKAA4FAADQKgAAAgBekRUFAADQKgAAHAB2pQCABYAMgJeAH4ATgAGAvIIIgASABIAFgCWA%22%2c%22range%22%3a%7B%22min%22%3a%2205C1D79B33ADE4%22%2c%22max%22%3a%2205C1D7A52F89EC%22%7D%7D%5d",
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
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
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
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div><div><div><span><img height=\"145\" src=\"https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents/aWQ9eF8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZC92aWV3cy9pbWdv/$value\" width=\"131\" style=\"vertical-align:bottom; width:131px; height:145px\"></span><div>&nbsp;</div></div><div><div><span><img height=\"65\" src=\"https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents/aWQ9eF8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNC92aWV3cy9pbWdv/$value\" width=\"79\" style=\"vertical-align:bottom; width:79px; height:65px\"></span></div></div></div></div>"
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

