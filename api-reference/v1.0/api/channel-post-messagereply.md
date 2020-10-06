---
title: Ответ на сообщение в канале
description: Ответ на существующее сообщение в канале.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f1ee31b18c17da5ea038115adb17fd362363030c
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364329"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="20e85-103">Ответ на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="20e85-103">Reply to a message in a channel</span></span>

<span data-ttu-id="20e85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20e85-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="20e85-105">Создание нового ответа на [сообщение](../resources/chatmessage.md) в указанном [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="20e85-105">Create a new reply to a [message](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="20e85-106">**Note**: мы не рекомендуем использовать этот API для переноса данных.</span><span class="sxs-lookup"><span data-stu-id="20e85-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="20e85-107">Пропускная способность, необходимая для обычной миграции, отсутствует.</span><span class="sxs-lookup"><span data-stu-id="20e85-107">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="20e85-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20e85-108">Permissions</span></span>

<span data-ttu-id="20e85-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20e85-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20e85-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20e85-111">Permission type</span></span>      | <span data-ttu-id="20e85-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20e85-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20e85-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20e85-113">Delegated (work or school account)</span></span> | <span data-ttu-id="20e85-114">Чаннелмессаже. Send, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="20e85-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="20e85-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20e85-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20e85-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20e85-116">Not supported.</span></span>    |
| <span data-ttu-id="20e85-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20e85-117">Application</span></span>                           | <span data-ttu-id="20e85-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20e85-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20e85-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20e85-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="20e85-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20e85-120">Request headers</span></span>

| <span data-ttu-id="20e85-121">Имя</span><span class="sxs-lookup"><span data-stu-id="20e85-121">Name</span></span>       | <span data-ttu-id="20e85-122">Тип</span><span class="sxs-lookup"><span data-stu-id="20e85-122">Type</span></span> | <span data-ttu-id="20e85-123">Описание</span><span class="sxs-lookup"><span data-stu-id="20e85-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="20e85-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="20e85-124">Authorization</span></span>  | <span data-ttu-id="20e85-125">string</span><span class="sxs-lookup"><span data-stu-id="20e85-125">string</span></span>  | <span data-ttu-id="20e85-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20e85-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20e85-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20e85-128">Request body</span></span>

<span data-ttu-id="20e85-129">В тексте запроса добавьте представление объекта [Message](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20e85-129">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="20e85-130">Только свойство Body является обязательным, другие свойства являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="20e85-130">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="20e85-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="20e85-131">Response</span></span>

<span data-ttu-id="20e85-132">В случае успешного выполнения этот метод возвращает `201 Created` код отклика с созданным [сообщением](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="20e85-132">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="20e85-133">Пример</span><span class="sxs-lookup"><span data-stu-id="20e85-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="20e85-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="20e85-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="20e85-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="20e85-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="20e85-136">C#</span><span class="sxs-lookup"><span data-stu-id="20e85-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20e85-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20e85-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20e85-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20e85-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reply-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20e85-139">Java</span><span class="sxs-lookup"><span data-stu-id="20e85-139">Java</span></span>](#tab/java) 
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="20e85-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="20e85-140">Response</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages('id-value')/replies/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
    "lastEditedDateTime": null,
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
