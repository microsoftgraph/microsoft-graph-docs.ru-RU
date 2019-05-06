---
title: 'post: reply'
description: 'Ответ на публикацию и добавление новой публикации в указанную цепочку беседы группы. Вы можете указать '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a5e1ec5d3ed2bca3b03c2298239f3168ff5b3699
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33595246"
---
# <a name="post-reply"></a><span data-ttu-id="3c25f-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="3c25f-104">post: reply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c25f-p102">Ответ на запись и добавление новой записи в указанную цепочку беседы группы. Вы можете указать в запросе родительскую беседу вместе с цепочкой или только родительскую цепочку.</span><span class="sxs-lookup"><span data-stu-id="3c25f-p102">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c25f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c25f-107">Permissions</span></span>
<span data-ttu-id="3c25f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c25f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c25f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c25f-110">Permission type</span></span>      | <span data-ttu-id="3c25f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c25f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c25f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c25f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3c25f-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c25f-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c25f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c25f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c25f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c25f-115">Not supported.</span></span>    |
|<span data-ttu-id="3c25f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c25f-116">Application</span></span> | <span data-ttu-id="3c25f-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c25f-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c25f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c25f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="3c25f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c25f-119">Request headers</span></span>
| <span data-ttu-id="3c25f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c25f-120">Header</span></span>       | <span data-ttu-id="3c25f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3c25f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3c25f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c25f-122">Authorization</span></span>  | <span data-ttu-id="3c25f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c25f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c25f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c25f-125">Request body</span></span>
<span data-ttu-id="3c25f-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3c25f-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3c25f-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="3c25f-127">Parameter</span></span>    | <span data-ttu-id="3c25f-128">Тип</span><span class="sxs-lookup"><span data-stu-id="3c25f-128">Type</span></span>   |<span data-ttu-id="3c25f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="3c25f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c25f-130">post</span><span class="sxs-lookup"><span data-stu-id="3c25f-130">post</span></span>|[<span data-ttu-id="3c25f-131">post</span><span class="sxs-lookup"><span data-stu-id="3c25f-131">post</span></span>](../resources/post.md)|<span data-ttu-id="3c25f-132">Новая запись для ответа.</span><span class="sxs-lookup"><span data-stu-id="3c25f-132">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="3c25f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c25f-133">Response</span></span>

<span data-ttu-id="3c25f-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3c25f-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c25f-136">Пример</span><span class="sxs-lookup"><span data-stu-id="3c25f-136">Example</span></span>
<span data-ttu-id="3c25f-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3c25f-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3c25f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c25f-138">Request</span></span>
<span data-ttu-id="3c25f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c25f-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "2016-10-19T10:37:00Z",
    "hasAttachments": true,
    "from": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "sender": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "conversationThreadId": "conversationThreadId-value",
    "newParticipants": [
      {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      }
    ],
    "conversationId": "conversationId-value",
    "createdDateTime": "2016-10-19T10:37:00Z",
    "lastModifiedDateTime": "2016-10-19T10:37:00Z",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "2016-10-19T10:37:00Z",
        "name": "name-value",
        "contentType": "contentType-value",
        "size": 99,
        "isInline": true,
        "id": "id-value"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="3c25f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c25f-140">Response</span></span>
##### <a name="response"></a><span data-ttu-id="3c25f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c25f-141">Response</span></span>
<span data-ttu-id="3c25f-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3c25f-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3c25f-143">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="3c25f-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3c25f-144">Языках</span><span class="sxs-lookup"><span data-stu-id="3c25f-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_reply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c25f-145">Язык</span><span class="sxs-lookup"><span data-stu-id="3c25f-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_reply-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/post-reply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/post-reply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
