---
title: 'post: reply'
description: 'Ответ на публикацию и добавление новой публикации в указанную цепочку беседы группы. Можно указать '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ecc13135fee90d0fc8175669551578fe9e22d128
ms.sourcegitcommit: 7dc8ca82a8b2c25c5084e6b3121688766c9c14a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/02/2021
ms.locfileid: "50072382"
---
# <a name="post-reply"></a><span data-ttu-id="828cb-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="828cb-104">post: reply</span></span>

<span data-ttu-id="828cb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="828cb-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="828cb-106">Ответ на запись и добавление новой записи в указанную цепочку беседы группы.</span><span class="sxs-lookup"><span data-stu-id="828cb-106">Reply to a post and add a new post to the specified thread in a group conversation.</span></span> 

<span data-ttu-id="828cb-107">Вы можете указать в запросе родительскую беседу вместе с цепочкой или только родительскую цепочку.</span><span class="sxs-lookup"><span data-stu-id="828cb-107">You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="828cb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="828cb-108">Permissions</span></span>
<span data-ttu-id="828cb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="828cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="828cb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="828cb-111">Permission type</span></span>      | <span data-ttu-id="828cb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="828cb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="828cb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="828cb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="828cb-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="828cb-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="828cb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="828cb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="828cb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="828cb-116">Not supported.</span></span>    |
|<span data-ttu-id="828cb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="828cb-117">Application</span></span> | <span data-ttu-id="828cb-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="828cb-118">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="828cb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="828cb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="828cb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="828cb-120">Request headers</span></span>
| <span data-ttu-id="828cb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="828cb-121">Header</span></span>       | <span data-ttu-id="828cb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="828cb-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="828cb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="828cb-123">Authorization</span></span>  | <span data-ttu-id="828cb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="828cb-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="828cb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="828cb-126">Request body</span></span>
<span data-ttu-id="828cb-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="828cb-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="828cb-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="828cb-128">Parameter</span></span>    | <span data-ttu-id="828cb-129">Тип</span><span class="sxs-lookup"><span data-stu-id="828cb-129">Type</span></span>   |<span data-ttu-id="828cb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="828cb-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="828cb-131">post</span><span class="sxs-lookup"><span data-stu-id="828cb-131">post</span></span>|[<span data-ttu-id="828cb-132">post</span><span class="sxs-lookup"><span data-stu-id="828cb-132">post</span></span>](../resources/post.md)|<span data-ttu-id="828cb-133">Новая запись для ответа.</span><span class="sxs-lookup"><span data-stu-id="828cb-133">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="828cb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="828cb-134">Response</span></span>

<span data-ttu-id="828cb-p104">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="828cb-p104">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="828cb-137">Пример</span><span class="sxs-lookup"><span data-stu-id="828cb-137">Example</span></span>
<span data-ttu-id="828cb-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="828cb-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="828cb-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="828cb-139">Request</span></span>
<span data-ttu-id="828cb-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="828cb-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="828cb-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="828cb-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "datetime-value",
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
    "createdDateTime": "datetime-value",
    "lastModifiedDateTime": "datetime-value",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "@odata.type": "#microsoft.graph.fileAttachment",
        "lastModifiedDateTime": "datetime-value",
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
# <a name="c"></a>[<span data-ttu-id="828cb-142">C#</span><span class="sxs-lookup"><span data-stu-id="828cb-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="828cb-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="828cb-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="828cb-144">Java</span><span class="sxs-lookup"><span data-stu-id="828cb-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="828cb-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="828cb-145">Response</span></span>
<span data-ttu-id="828cb-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="828cb-146">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

