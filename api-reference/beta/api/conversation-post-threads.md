---
title: Создание цепочки
description: Создание цепочки в указанной беседе.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 31142bb2277f32aec1556d20e0915b97e621645a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956822"
---
# <a name="create-thread"></a><span data-ttu-id="4864f-103">Создание цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="4864f-103">Create thread</span></span>

<span data-ttu-id="4864f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4864f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4864f-105">Создание цепочки в указанной беседе.</span><span class="sxs-lookup"><span data-stu-id="4864f-105">Create a new thread in the specified conversation.</span></span>

<span data-ttu-id="4864f-p101">Создание указанных цепочки и записи. Используйте [цепочку ответов](conversationthread-reply.md), чтобы размещать дальнейшие записи в этой цепочке. Кроме того, если вы получаете идентификатор записи, вы можете [ответить](post-reply.md) на эту запись в цепочке.</span><span class="sxs-lookup"><span data-stu-id="4864f-p101">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="4864f-109">Примечание. Вы также можете [начать новую беседу, создав цепочку](group-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="4864f-109">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4864f-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4864f-110">Permissions</span></span>
<span data-ttu-id="4864f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4864f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4864f-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4864f-113">Permission type</span></span>      | <span data-ttu-id="4864f-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4864f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4864f-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4864f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4864f-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4864f-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4864f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4864f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4864f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4864f-118">Not supported.</span></span>    |
|<span data-ttu-id="4864f-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4864f-119">Application</span></span> | <span data-ttu-id="4864f-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4864f-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4864f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4864f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="4864f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4864f-122">Request headers</span></span>
| <span data-ttu-id="4864f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="4864f-123">Name</span></span>       | <span data-ttu-id="4864f-124">Тип</span><span class="sxs-lookup"><span data-stu-id="4864f-124">Type</span></span> | <span data-ttu-id="4864f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4864f-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4864f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4864f-126">Authorization</span></span>  | <span data-ttu-id="4864f-127">string</span><span class="sxs-lookup"><span data-stu-id="4864f-127">string</span></span>  | <span data-ttu-id="4864f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4864f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4864f-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4864f-130">Request body</span></span>
<span data-ttu-id="4864f-131">В теле запроса укажите описание объекта [ConversationThread](../resources/conversationthread.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4864f-131">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4864f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4864f-132">Response</span></span>

<span data-ttu-id="4864f-133">В случае успеха этот метод возвратит код отклика `201 Created` и объект [ConversationThread](../resources/conversationthread.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4864f-133">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4864f-134">Пример</span><span class="sxs-lookup"><span data-stu-id="4864f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4864f-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="4864f-135">Request</span></span>
<span data-ttu-id="4864f-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4864f-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4864f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4864f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
Content-type: application/json

{
  "topic": "topic-value",
  "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      }
  }]
}
```
# <a name="c"></a>[<span data-ttu-id="4864f-138">C#</span><span class="sxs-lookup"><span data-stu-id="4864f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationthread-from-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4864f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4864f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationthread-from-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4864f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4864f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationthread-from-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4864f-141">Java</span><span class="sxs-lookup"><span data-stu-id="4864f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversationthread-from-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4864f-142">В теле запроса укажите описание объекта [conversationThread](../resources/conversationthread.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4864f-142">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4864f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4864f-143">Response</span></span>

<span data-ttu-id="4864f-p104">В случае успеха этот метод возвратит код отклика `201 Created` и `id` новой цепочки в теле отклика. Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4864f-p104">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
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


