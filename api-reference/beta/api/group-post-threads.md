---
title: Создание цепочки беседы
description: 'Начните групповой чат, создав цепочку. '
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 9c6c63c6a8cb193f085e288c7b89c93a83525fa1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829067"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="180f8-103">Создание цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="180f8-103">Create conversation thread</span></span>

> <span data-ttu-id="180f8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="180f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="180f8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="180f8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="180f8-106">Начните групповой чат, создав цепочку.</span><span class="sxs-lookup"><span data-stu-id="180f8-106">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="180f8-p102">В группе создаются беседа, цепочка беседы и запись. Размещать в цепочке дальнейшие записи можно с помощью ответов на [цепочки](conversationthread-reply.md) и [записи](post-reply.md).</span><span class="sxs-lookup"><span data-stu-id="180f8-p102">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="180f8-109">Примечание. Вы также можете [создать цепочку и существующей беседе](conversation-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="180f8-109">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="180f8-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="180f8-110">Permissions</span></span>
<span data-ttu-id="180f8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="180f8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="180f8-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="180f8-113">Permission type</span></span>      | <span data-ttu-id="180f8-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="180f8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="180f8-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="180f8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="180f8-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="180f8-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="180f8-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="180f8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="180f8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="180f8-118">Not supported.</span></span>    |
|<span data-ttu-id="180f8-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="180f8-119">Application</span></span> | <span data-ttu-id="180f8-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="180f8-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="180f8-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="180f8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="180f8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="180f8-122">Request headers</span></span>
| <span data-ttu-id="180f8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="180f8-123">Header</span></span>       | <span data-ttu-id="180f8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="180f8-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="180f8-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="180f8-125">Authorization</span></span>  | <span data-ttu-id="180f8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="180f8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="180f8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="180f8-128">Content-Type</span></span>  | <span data-ttu-id="180f8-129">application/json</span><span class="sxs-lookup"><span data-stu-id="180f8-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="180f8-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="180f8-130">Request body</span></span>
<span data-ttu-id="180f8-131">Предоставьте в тексте запроса описание объекта [conversationThread](../resources/conversationthread.md), содержащего объект [post](../resources/post.md), в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="180f8-131">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="180f8-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="180f8-132">Response</span></span>
<span data-ttu-id="180f8-133">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="180f8-133">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="180f8-134">Пример</span><span class="sxs-lookup"><span data-stu-id="180f8-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="180f8-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="180f8-135">Request</span></span>
<span data-ttu-id="180f8-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="180f8-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads
Content-type: application/json

{
  "topic": "New Conversation Thread Topic",
  "posts": [{
    "body": {
      "contentType": "html",
      "content": "this is body content"
    },
    "newParticipants": [{
      "emailAddress": {
        "name": "Alex Darrow",
        "address": "alexd@contoso.com"
      }
    }]
  }]
}
```

#### <a name="response"></a><span data-ttu-id="180f8-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="180f8-137">Response</span></span>
<span data-ttu-id="180f8-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="180f8-138">The following is an example of the response.</span></span>
><span data-ttu-id="180f8-139">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="180f8-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="180f8-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="180f8-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
