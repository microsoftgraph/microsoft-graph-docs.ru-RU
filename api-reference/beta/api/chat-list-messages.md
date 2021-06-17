---
title: Список сообщений в чате
description: 'Получение списка сообщений в чате. '
localization_priority: Priority
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0acd5466ff17fca1090d491708ce231f37a31f3c
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971295"
---
# <a name="list-messages-in-a-chat"></a><span data-ttu-id="32e40-103">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="32e40-103">List messages in a chat</span></span>

<span data-ttu-id="32e40-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32e40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32e40-105">Получение списка [сообщений](../resources/chatmessage.md) в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="32e40-105">Retrieve the list of [messages](../resources/chatmessage.md) in a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="32e40-106">**Примечание**. Этот API поддерживает подписку на изменения (создание, обновление и удаление) с использованием [уведомлений об изменениях](../resources/webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="32e40-106">**Note**: This API supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="32e40-107">Это позволяет вызывающим подписаться на изменения и получать их в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="32e40-107">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="32e40-108">Дополнительные сведения см. в разделе [Получение уведомлений о сообщениях](/graph/teams-changenotifications-chatmessage).</span><span class="sxs-lookup"><span data-stu-id="32e40-108">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatmessage).</span></span>

## <a name="permissions"></a><span data-ttu-id="32e40-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32e40-109">Permissions</span></span>

<span data-ttu-id="32e40-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32e40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32e40-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32e40-112">Permission type</span></span>      | <span data-ttu-id="32e40-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32e40-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32e40-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32e40-114">Delegated (work or school account)</span></span> | <span data-ttu-id="32e40-115">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32e40-115">Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="32e40-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32e40-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32e40-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32e40-117">Not supported.</span></span>    |
|<span data-ttu-id="32e40-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="32e40-118">Application</span></span> | <span data-ttu-id="32e40-119">ChatMessage.Read.Chat\*, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32e40-119">ChatMessage.Read.Chat\*, Chat.Read.All, Chat.ReadWrite.All</span></span> |

> <span data-ttu-id="32e40-120">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="32e40-120">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="32e40-121">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="32e40-121">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="32e40-122">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="32e40-122">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="32e40-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32e40-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{chat-id}/messages
GET /users/{user-id | user-principal-name}/chats/{chat-id}/messages
GET /chats/{chat-id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="32e40-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="32e40-124">Optional query parameters</span></span>

<span data-ttu-id="32e40-125">Вы можете использовать параметр запроса [$top](/graph/query-parameters#top-parameter) для управления количеством элементов в одном отклике.</span><span class="sxs-lookup"><span data-stu-id="32e40-125">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="32e40-126">Максимальное значение `$top`: 50.</span><span class="sxs-lookup"><span data-stu-id="32e40-126">Maximum allowed `$top` value is 50.</span></span>
<span data-ttu-id="32e40-127">Другие [параметры запроса OData](/graph/query-parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="32e40-127">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="32e40-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32e40-128">Request headers</span></span>

| <span data-ttu-id="32e40-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32e40-129">Header</span></span>       | <span data-ttu-id="32e40-130">Значение</span><span class="sxs-lookup"><span data-stu-id="32e40-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="32e40-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32e40-131">Authorization</span></span>  | <span data-ttu-id="32e40-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32e40-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="32e40-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32e40-134">Request body</span></span>

<span data-ttu-id="32e40-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="32e40-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32e40-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="32e40-136">Response</span></span>

<span data-ttu-id="32e40-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32e40-137">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32e40-138">Пример</span><span class="sxs-lookup"><span data-stu-id="32e40-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="32e40-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="32e40-139">Request</span></span>

<span data-ttu-id="32e40-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32e40-140">The following is an example of the request.</span></span> <span data-ttu-id="32e40-141">`$top=2` передается для получения двух сообщений.</span><span class="sxs-lookup"><span data-stu-id="32e40-141">`$top=2` is passed to retrieve two messages.</span></span>


# <a name="http"></a>[<span data-ttu-id="32e40-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="32e40-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allchatmessages_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages?$top=2
```
# <a name="c"></a>[<span data-ttu-id="32e40-143">C#</span><span class="sxs-lookup"><span data-stu-id="32e40-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allchatmessages-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32e40-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32e40-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allchatmessages-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32e40-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32e40-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allchatmessages-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32e40-146">Java</span><span class="sxs-lookup"><span data-stu-id="32e40-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-allchatmessages-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="32e40-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="32e40-147">Response</span></span>
<span data-ttu-id="32e40-148">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="32e40-148">The following example shows the response.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages?$top=2&$skiptoken=M2UyZDAwMDAwMDMxMzkzYTMyNjQ2MTM0NjMzMjM5NjYzNjY0MzczMDM0MzE2NTYzNjEzNzMwNjIzNjMzMzg2MjM0MzM2NDM0MzUzNDMzMzc0MDc0Njg3MjY1NjE2NDJlNzYzMjAxZThmYjY4M2Y3ODAxMDAwMDg4NjA5ODdhNzgwMTAwMDB8MTYxNjk2NDUwOTgzMg%3d%3d",
    "value": [
        {
            "id": "1616964509832",
            "replyToId": null,
            "etag": "1616964509832",
            "messageType": "message",
            "createdDateTime": "2021-03-28T20:48:29.832Z",
            "lastModifiedDateTime": "2021-03-28T20:48:29.832Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
            "importance": "normal",
            "locale": "en-us",
            "webUrl": null,
            "channelIdentity": null,
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
                "contentType": "text",
                "content": "Hello world"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1615971548136",
            "replyToId": null,
            "etag": "1615971548136",
            "messageType": "message",
            "createdDateTime": "2021-03-17T08:59:08.136Z",
            "lastModifiedDateTime": "2021-03-17T08:59:08.136Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
            "importance": "normal",
            "locale": "en-us",
            "webUrl": null,
            "channelIdentity": null,
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
                "content": "<div><div><div><span><img height=\"63\" src=\"https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents/aWQ9eF8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNix0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1lNTRmNjM1NWYxYmJkNGQ3ZTNmNGJhZmU4NTI5MTBmNi92aWV3cy9pbWdv/$value\" width=\"67\" style=\"vertical-align:bottom; width:67px; height:63px\"></span></div></div></div>"
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
  "description": "Get chat messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

