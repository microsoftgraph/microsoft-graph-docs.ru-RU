---
title: Создание цепочки беседы
description: 'Начните групповой чат, создав цепочку. '
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c118958262c3290c77b5046a76af799527fec292
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042039"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="c9482-103">Создание цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="c9482-103">Create conversation thread</span></span>

<span data-ttu-id="c9482-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9482-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c9482-105">Начните групповой чат, создав цепочку.</span><span class="sxs-lookup"><span data-stu-id="c9482-105">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="c9482-p101">В группе создаются беседа, цепочка беседы и запись. Размещать в цепочке дальнейшие записи можно с помощью ответов на [цепочки](conversationthread-reply.md) и [записи](post-reply.md).</span><span class="sxs-lookup"><span data-stu-id="c9482-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="c9482-108">Примечание. Вы также можете [создать цепочку и существующей беседе](conversation-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="c9482-108">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="c9482-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9482-109">Permissions</span></span>
<span data-ttu-id="c9482-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9482-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9482-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9482-112">Permission type</span></span>      | <span data-ttu-id="c9482-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9482-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9482-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9482-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c9482-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9482-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c9482-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9482-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9482-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9482-117">Not supported.</span></span>    |
|<span data-ttu-id="c9482-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9482-118">Application</span></span> | <span data-ttu-id="c9482-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9482-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9482-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9482-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="c9482-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9482-121">Request headers</span></span>
| <span data-ttu-id="c9482-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9482-122">Header</span></span>       | <span data-ttu-id="c9482-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c9482-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c9482-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9482-124">Authorization</span></span>  | <span data-ttu-id="c9482-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9482-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c9482-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c9482-127">Content-Type</span></span>  | <span data-ttu-id="c9482-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c9482-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c9482-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9482-129">Request body</span></span>
<span data-ttu-id="c9482-130">Предоставьте в тексте запроса описание объекта [conversationThread](../resources/conversationthread.md), содержащего объект [post](../resources/post.md), в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9482-130">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="c9482-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9482-131">Response</span></span>
<span data-ttu-id="c9482-132">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9482-132">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9482-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c9482-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c9482-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9482-134">Request</span></span>
<span data-ttu-id="c9482-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9482-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c9482-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9482-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads
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
# <a name="c"></a>[<span data-ttu-id="c9482-137">C#</span><span class="sxs-lookup"><span data-stu-id="c9482-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationthread-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9482-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9482-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationthread-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9482-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9482-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationthread-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9482-140">Java</span><span class="sxs-lookup"><span data-stu-id="c9482-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversationthread-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c9482-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9482-141">Response</span></span>
<span data-ttu-id="c9482-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c9482-142">The following is an example of the response.</span></span>
><span data-ttu-id="c9482-143">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c9482-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c9482-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9482-144">All the properties will be returned from an actual call.</span></span>
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
  "lastDeliveredDateTime": "datetime-value",
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

