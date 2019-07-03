---
title: Создание цепочки беседы
description: 'Начните групповой чат, создав цепочку. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7e3de7d165b4bf7ce7bf6ad70deeb7de7d272527
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442820"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="730e2-103">Создание цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="730e2-103">Create conversation thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="730e2-104">Начните групповой чат, создав цепочку.</span><span class="sxs-lookup"><span data-stu-id="730e2-104">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="730e2-p101">В группе создаются беседа, цепочка беседы и запись. Размещать в цепочке дальнейшие записи можно с помощью ответов на [цепочки](conversationthread-reply.md) и [записи](post-reply.md).</span><span class="sxs-lookup"><span data-stu-id="730e2-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="730e2-107">Примечание. Вы также можете [создать цепочку и существующей беседе](conversation-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="730e2-107">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="730e2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="730e2-108">Permissions</span></span>
<span data-ttu-id="730e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="730e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="730e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="730e2-111">Permission type</span></span>      | <span data-ttu-id="730e2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="730e2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="730e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="730e2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="730e2-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="730e2-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="730e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="730e2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="730e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="730e2-116">Not supported.</span></span>    |
|<span data-ttu-id="730e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="730e2-117">Application</span></span> | <span data-ttu-id="730e2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="730e2-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="730e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="730e2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="730e2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="730e2-120">Request headers</span></span>
| <span data-ttu-id="730e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="730e2-121">Header</span></span>       | <span data-ttu-id="730e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="730e2-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="730e2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="730e2-123">Authorization</span></span>  | <span data-ttu-id="730e2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="730e2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="730e2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="730e2-126">Content-Type</span></span>  | <span data-ttu-id="730e2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="730e2-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="730e2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="730e2-128">Request body</span></span>
<span data-ttu-id="730e2-129">Предоставьте в тексте запроса описание объекта [conversationThread](../resources/conversationthread.md), содержащего объект [post](../resources/post.md), в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="730e2-129">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="730e2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="730e2-130">Response</span></span>
<span data-ttu-id="730e2-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="730e2-131">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="730e2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="730e2-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="730e2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="730e2-133">Request</span></span>
<span data-ttu-id="730e2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="730e2-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="730e2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="730e2-135">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="730e2-136">C#</span><span class="sxs-lookup"><span data-stu-id="730e2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationthread-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="730e2-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="730e2-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationthread-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="730e2-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="730e2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationthread-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="730e2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="730e2-139">Response</span></span>
<span data-ttu-id="730e2-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="730e2-140">The following is an example of the response.</span></span>
><span data-ttu-id="730e2-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="730e2-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="730e2-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="730e2-142">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
