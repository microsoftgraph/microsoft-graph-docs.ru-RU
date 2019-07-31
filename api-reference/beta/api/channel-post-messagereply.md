---
title: Ответ на сообщение в канале
description: Ответ на существующее сообщение в канале.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2fad5650e530f494a0f9a5bbb91d820340dc2a9e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944228"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="0591a-103">Ответ на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="0591a-103">Reply to a message in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0591a-104">Создание нового ответа на [сообщение](../resources/chatmessage.md) в указанном канале [](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="0591a-104">Create a new reply to a [message](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="0591a-105">**Note**: мы не рекомендуем использовать этот API для переноса данных.</span><span class="sxs-lookup"><span data-stu-id="0591a-105">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="0591a-106">Пропускная способность, необходимая для обычной миграции, отсутствует.</span><span class="sxs-lookup"><span data-stu-id="0591a-106">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="0591a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0591a-107">Permissions</span></span>
<span data-ttu-id="0591a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0591a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0591a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0591a-110">Permission type</span></span>      | <span data-ttu-id="0591a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0591a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0591a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0591a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0591a-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0591a-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0591a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0591a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0591a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0591a-115">Not supported.</span></span>    |
|<span data-ttu-id="0591a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0591a-116">Application</span></span> | <span data-ttu-id="0591a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0591a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0591a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0591a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```
## <a name="request-headers"></a><span data-ttu-id="0591a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0591a-119">Request headers</span></span>
| <span data-ttu-id="0591a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0591a-120">Name</span></span>       | <span data-ttu-id="0591a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0591a-121">Type</span></span> | <span data-ttu-id="0591a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0591a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0591a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0591a-123">Authorization</span></span>  | <span data-ttu-id="0591a-124">string</span><span class="sxs-lookup"><span data-stu-id="0591a-124">string</span></span>  | <span data-ttu-id="0591a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0591a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0591a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0591a-127">Request body</span></span>
<span data-ttu-id="0591a-128">В тексте запроса добавьте представление объекта [Message](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0591a-128">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="0591a-129">Только свойство Body является обязательным, другие свойства являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="0591a-129">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="0591a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0591a-130">Response</span></span>

<span data-ttu-id="0591a-131">В случае успешного выполнения этот метод `201 Created` возвращает код отклика с созданным [сообщением](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="0591a-131">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="0591a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0591a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0591a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0591a-133">Request</span></span>
<span data-ttu-id="0591a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0591a-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0591a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0591a-135">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0591a-136">C#</span><span class="sxs-lookup"><span data-stu-id="0591a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0591a-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="0591a-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0591a-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0591a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reply-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0591a-139">Java</span><span class="sxs-lookup"><span data-stu-id="0591a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0591a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0591a-140">Response</span></span>

<span data-ttu-id="0591a-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0591a-141">Here is an example of the response.</span></span>
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
