---
title: Ответ на сообщение в канале
description: Ответ на существующее сообщение в канале.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9353751562308c7c487fff8965024d90556ceb14
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635563"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="c4c36-103">Ответ на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="c4c36-103">Reply to a message in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4c36-104">Создание нового ответа на [сообщение](../resources/chatmessage.md) в указанном канале [](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="c4c36-104">Create a new reply to a [message](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4c36-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4c36-105">Permissions</span></span>
<span data-ttu-id="c4c36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4c36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4c36-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4c36-108">Permission type</span></span>      | <span data-ttu-id="c4c36-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4c36-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4c36-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4c36-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c4c36-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4c36-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c4c36-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4c36-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4c36-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4c36-113">Not supported.</span></span>    |
|<span data-ttu-id="c4c36-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4c36-114">Application</span></span> | <span data-ttu-id="c4c36-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4c36-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4c36-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4c36-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```
## <a name="request-headers"></a><span data-ttu-id="c4c36-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4c36-117">Request headers</span></span>
| <span data-ttu-id="c4c36-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c4c36-118">Name</span></span>       | <span data-ttu-id="c4c36-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c4c36-119">Type</span></span> | <span data-ttu-id="c4c36-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c4c36-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c4c36-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4c36-121">Authorization</span></span>  | <span data-ttu-id="c4c36-122">string</span><span class="sxs-lookup"><span data-stu-id="c4c36-122">string</span></span>  | <span data-ttu-id="c4c36-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4c36-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4c36-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4c36-125">Request body</span></span>
<span data-ttu-id="c4c36-126">В тексте запроса добавьте представление объекта [Message](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4c36-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="c4c36-127">Только свойство Body является обязательным, другие свойства являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="c4c36-127">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="c4c36-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4c36-128">Response</span></span>

<span data-ttu-id="c4c36-129">В случае успешного выполнения этот метод `201 Created` возвращает код отклика с созданным [сообщением](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="c4c36-129">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="c4c36-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c4c36-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4c36-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4c36-131">Request</span></span>
<span data-ttu-id="c4c36-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4c36-132">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c4c36-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4c36-133">Response</span></span>

<span data-ttu-id="c4c36-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4c36-134">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c4c36-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="c4c36-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c4c36-136">Языках</span><span class="sxs-lookup"><span data-stu-id="c4c36-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_reply_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4c36-137">Язык</span><span class="sxs-lookup"><span data-stu-id="c4c36-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_reply_message-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/channel-post-messagereply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-post-messagereply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
