---
title: 'post: reply'
description: 'Ответ на публикацию и добавление новой публикации в указанную цепочку беседы группы. Можно указать '
author: dkershaw10
ms.openlocfilehash: 33cd99fd24dc5acfca4b96f232f748a0377d1564
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324229"
---
# <a name="post-reply"></a><span data-ttu-id="bb00c-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="bb00c-104">post: reply</span></span>

> <span data-ttu-id="bb00c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bb00c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb00c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb00c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb00c-p103">Ответ на запись и добавление новой записи в указанную цепочку беседы группы. Вы можете указать в запросе родительскую беседу вместе с цепочкой или только родительскую цепочку.</span><span class="sxs-lookup"><span data-stu-id="bb00c-p103">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb00c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb00c-109">Permissions</span></span>
<span data-ttu-id="bb00c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb00c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb00c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb00c-112">Permission type</span></span>      | <span data-ttu-id="bb00c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb00c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb00c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb00c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bb00c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb00c-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bb00c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb00c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb00c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb00c-117">Not supported.</span></span>    |
|<span data-ttu-id="bb00c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb00c-118">Application</span></span> | <span data-ttu-id="bb00c-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb00c-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb00c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb00c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="bb00c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb00c-121">Request headers</span></span>
| <span data-ttu-id="bb00c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb00c-122">Header</span></span>       | <span data-ttu-id="bb00c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="bb00c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bb00c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb00c-124">Authorization</span></span>  | <span data-ttu-id="bb00c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb00c-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bb00c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb00c-127">Request body</span></span>
<span data-ttu-id="bb00c-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="bb00c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bb00c-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="bb00c-129">Parameter</span></span>    | <span data-ttu-id="bb00c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bb00c-130">Type</span></span>   |<span data-ttu-id="bb00c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bb00c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb00c-132">post</span><span class="sxs-lookup"><span data-stu-id="bb00c-132">post</span></span>|[<span data-ttu-id="bb00c-133">post</span><span class="sxs-lookup"><span data-stu-id="bb00c-133">post</span></span>](../resources/post.md)|<span data-ttu-id="bb00c-134">Новая запись для ответа.</span><span class="sxs-lookup"><span data-stu-id="bb00c-134">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="bb00c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb00c-135">Response</span></span>

<span data-ttu-id="bb00c-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bb00c-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb00c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="bb00c-138">Example</span></span>
<span data-ttu-id="bb00c-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bb00c-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bb00c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb00c-140">Request</span></span>
<span data-ttu-id="bb00c-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb00c-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="bb00c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb00c-142">Response</span></span>
##### <a name="response"></a><span data-ttu-id="bb00c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb00c-143">Response</span></span>
<span data-ttu-id="bb00c-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb00c-144">Here is an example of the response.</span></span>
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
