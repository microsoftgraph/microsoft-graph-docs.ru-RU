---
title: Ответ на сообщение в канале
description: Ответ на существующее сообщение в канале.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 02e177ace9c463efa115da531a6d95020820bf72
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987068"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="ce294-103">Ответ на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="ce294-103">Reply to a message in a channel</span></span>

<span data-ttu-id="ce294-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce294-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce294-105">Создание нового ответа на [chatMessage](../resources/chatmessage.md) в указанном [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="ce294-105">Create a new reply to a [chatMessage](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="ce294-106">**Note**: мы не рекомендуем использовать этот API для переноса данных.</span><span class="sxs-lookup"><span data-stu-id="ce294-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="ce294-107">Пропускная способность, необходимая для обычной миграции, отсутствует.</span><span class="sxs-lookup"><span data-stu-id="ce294-107">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="ce294-108">**Note**: нарушение [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) Microsoft Teams в качестве файла журнала.</span><span class="sxs-lookup"><span data-stu-id="ce294-108">**Note**: It is a violation of the [terms of use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="ce294-109">Отправлять только сообщения, которые пользователи смогут читать.</span><span class="sxs-lookup"><span data-stu-id="ce294-109">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce294-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce294-110">Permissions</span></span>
<span data-ttu-id="ce294-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce294-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce294-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce294-113">Permission type</span></span>      | <span data-ttu-id="ce294-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce294-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce294-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce294-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ce294-116">Чаннелмессаже. Send, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ce294-116">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="ce294-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce294-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce294-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce294-118">Not supported.</span></span>    |
|<span data-ttu-id="ce294-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce294-119">Application</span></span> | <span data-ttu-id="ce294-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce294-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce294-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce294-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```
## <a name="request-headers"></a><span data-ttu-id="ce294-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce294-122">Request headers</span></span>
| <span data-ttu-id="ce294-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ce294-123">Name</span></span>       | <span data-ttu-id="ce294-124">Тип</span><span class="sxs-lookup"><span data-stu-id="ce294-124">Type</span></span> | <span data-ttu-id="ce294-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ce294-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ce294-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce294-126">Authorization</span></span>  | <span data-ttu-id="ce294-127">string</span><span class="sxs-lookup"><span data-stu-id="ce294-127">string</span></span>  | <span data-ttu-id="ce294-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce294-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce294-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ce294-130">Request body</span></span>
<span data-ttu-id="ce294-131">В тексте запроса добавьте представление объекта [Message](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce294-131">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="ce294-132">Только свойство Body является обязательным, другие свойства являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="ce294-132">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="ce294-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce294-133">Response</span></span>

<span data-ttu-id="ce294-134">В случае успешного выполнения этот метод возвращает `201 Created` код отклика с созданным [сообщением](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="ce294-134">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="ce294-135">Пример</span><span class="sxs-lookup"><span data-stu-id="ce294-135">Example</span></span>

<span data-ttu-id="ce294-136">Более полный список примеров приведен [в статье Создание chatMessage в канале или чате](chatmessage-post.md).</span><span class="sxs-lookup"><span data-stu-id="ce294-136">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="ce294-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce294-137">Request</span></span>
<span data-ttu-id="ce294-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce294-138">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce294-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce294-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="ce294-140">C#</span><span class="sxs-lookup"><span data-stu-id="ce294-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce294-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce294-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce294-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce294-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reply-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ce294-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce294-143">Response</span></span>

<span data-ttu-id="ce294-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ce294-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages('id-value')/replies/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": null,
    "deleted": false,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create a reply message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


