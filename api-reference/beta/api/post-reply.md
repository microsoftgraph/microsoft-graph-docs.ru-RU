---
title: 'post: reply'
description: 'Ответ на публикацию и добавление новой публикации в указанную цепочку беседы группы. Можно указать '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 681fa62198d2d1e8832b90432e0a76e84722e010
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944189"
---
# <a name="post-reply"></a><span data-ttu-id="1b552-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="1b552-104">post: reply</span></span>

> <span data-ttu-id="1b552-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1b552-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b552-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b552-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1b552-p103">Ответ на запись и добавление новой записи в указанную цепочку беседы группы. Вы можете указать в запросе родительскую беседу вместе с цепочкой или только родительскую цепочку.</span><span class="sxs-lookup"><span data-stu-id="1b552-p103">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b552-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b552-109">Permissions</span></span>
<span data-ttu-id="1b552-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b552-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b552-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b552-112">Permission type</span></span>      | <span data-ttu-id="1b552-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b552-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b552-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b552-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1b552-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b552-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1b552-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b552-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b552-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b552-117">Not supported.</span></span>    |
|<span data-ttu-id="1b552-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b552-118">Application</span></span> | <span data-ttu-id="1b552-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b552-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b552-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b552-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="1b552-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b552-121">Request headers</span></span>
| <span data-ttu-id="1b552-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b552-122">Header</span></span>       | <span data-ttu-id="1b552-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1b552-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1b552-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b552-124">Authorization</span></span>  | <span data-ttu-id="1b552-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b552-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1b552-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1b552-127">Request body</span></span>
<span data-ttu-id="1b552-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1b552-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1b552-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="1b552-129">Parameter</span></span>    | <span data-ttu-id="1b552-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1b552-130">Type</span></span>   |<span data-ttu-id="1b552-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1b552-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b552-132">post</span><span class="sxs-lookup"><span data-stu-id="1b552-132">post</span></span>|[<span data-ttu-id="1b552-133">post</span><span class="sxs-lookup"><span data-stu-id="1b552-133">post</span></span>](../resources/post.md)|<span data-ttu-id="1b552-134">Новая запись для ответа.</span><span class="sxs-lookup"><span data-stu-id="1b552-134">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="1b552-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b552-135">Response</span></span>

<span data-ttu-id="1b552-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1b552-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b552-138">Пример</span><span class="sxs-lookup"><span data-stu-id="1b552-138">Example</span></span>
<span data-ttu-id="1b552-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1b552-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1b552-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b552-140">Request</span></span>
<span data-ttu-id="1b552-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b552-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1b552-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b552-142">Response</span></span>
##### <a name="response"></a><span data-ttu-id="1b552-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b552-143">Response</span></span>
<span data-ttu-id="1b552-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1b552-144">Here is an example of the response.</span></span>
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
