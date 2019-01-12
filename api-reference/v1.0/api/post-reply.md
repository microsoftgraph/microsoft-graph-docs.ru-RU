---
title: 'post: reply'
description: 'Ответ на публикацию и добавление новой публикации в указанную цепочку беседы группы. Можно указать '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4c53339170a133ef468112843fd378b5dbdc7c60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923931"
---
# <a name="post-reply"></a><span data-ttu-id="d2078-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="d2078-104">post: reply</span></span>

<span data-ttu-id="d2078-p102">Ответ на запись и добавление новой записи в указанную цепочку беседы группы. Вы можете указать в запросе родительскую беседу вместе с цепочкой или только родительскую цепочку.</span><span class="sxs-lookup"><span data-stu-id="d2078-p102">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2078-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2078-107">Permissions</span></span>
<span data-ttu-id="d2078-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2078-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2078-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2078-110">Permission type</span></span>      | <span data-ttu-id="d2078-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2078-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2078-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2078-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d2078-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2078-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d2078-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2078-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2078-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2078-115">Not supported.</span></span>    |
|<span data-ttu-id="d2078-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2078-116">Application</span></span> | <span data-ttu-id="d2078-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2078-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2078-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2078-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="d2078-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2078-119">Request headers</span></span>
| <span data-ttu-id="d2078-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2078-120">Header</span></span>       | <span data-ttu-id="d2078-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d2078-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d2078-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2078-122">Authorization</span></span>  | <span data-ttu-id="d2078-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2078-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2078-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2078-125">Request body</span></span>
<span data-ttu-id="d2078-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d2078-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d2078-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="d2078-127">Parameter</span></span>    | <span data-ttu-id="d2078-128">Тип</span><span class="sxs-lookup"><span data-stu-id="d2078-128">Type</span></span>   |<span data-ttu-id="d2078-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d2078-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2078-130">post</span><span class="sxs-lookup"><span data-stu-id="d2078-130">post</span></span>|[<span data-ttu-id="d2078-131">post</span><span class="sxs-lookup"><span data-stu-id="d2078-131">post</span></span>](../resources/post.md)|<span data-ttu-id="d2078-132">Новая запись для ответа.</span><span class="sxs-lookup"><span data-stu-id="d2078-132">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="d2078-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2078-133">Response</span></span>

<span data-ttu-id="d2078-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d2078-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2078-136">Пример</span><span class="sxs-lookup"><span data-stu-id="d2078-136">Example</span></span>
<span data-ttu-id="d2078-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d2078-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d2078-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2078-138">Request</span></span>
<span data-ttu-id="d2078-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2078-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d2078-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2078-140">Response</span></span>
<span data-ttu-id="d2078-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2078-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
