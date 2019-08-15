---
title: Создание цепочки
description: Создание цепочки в указанной беседе.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7a78352847ff8ff5aa64249bf688168d3c9df2a1
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417811"
---
# <a name="create-thread"></a><span data-ttu-id="edbad-103">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="edbad-103">Create thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edbad-104">Создание цепочки в указанной беседе.</span><span class="sxs-lookup"><span data-stu-id="edbad-104">Create a new thread in the specified conversation.</span></span>

<span data-ttu-id="edbad-p101">Создание указанных цепочки и записи. Используйте [цепочку ответов](conversationthread-reply.md), чтобы размещать дальнейшие записи в этой цепочке. Кроме того, если вы получаете идентификатор записи, вы можете [ответить](post-reply.md) на эту запись в цепочке.</span><span class="sxs-lookup"><span data-stu-id="edbad-p101">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="edbad-108">Примечание. Вы также можете [начать новую беседу, создав цепочку](group-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="edbad-108">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="edbad-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="edbad-109">Permissions</span></span>
<span data-ttu-id="edbad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edbad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edbad-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edbad-112">Permission type</span></span>      | <span data-ttu-id="edbad-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="edbad-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edbad-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edbad-114">Delegated (work or school account)</span></span> | <span data-ttu-id="edbad-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edbad-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="edbad-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edbad-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edbad-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edbad-117">Not supported.</span></span>    |
|<span data-ttu-id="edbad-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edbad-118">Application</span></span> | <span data-ttu-id="edbad-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edbad-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="edbad-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edbad-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="edbad-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edbad-121">Request headers</span></span>
| <span data-ttu-id="edbad-122">Имя</span><span class="sxs-lookup"><span data-stu-id="edbad-122">Name</span></span>       | <span data-ttu-id="edbad-123">Тип</span><span class="sxs-lookup"><span data-stu-id="edbad-123">Type</span></span> | <span data-ttu-id="edbad-124">Описание</span><span class="sxs-lookup"><span data-stu-id="edbad-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="edbad-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="edbad-125">Authorization</span></span>  | <span data-ttu-id="edbad-126">string</span><span class="sxs-lookup"><span data-stu-id="edbad-126">string</span></span>  | <span data-ttu-id="edbad-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edbad-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="edbad-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="edbad-129">Request body</span></span>
<span data-ttu-id="edbad-130">В теле запроса укажите описание объекта [ConversationThread](../resources/conversationthread.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edbad-130">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="edbad-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="edbad-131">Response</span></span>

<span data-ttu-id="edbad-132">В случае успеха этот метод возвратит код отклика `201 Created` и объект [ConversationThread](../resources/conversationthread.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="edbad-132">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edbad-133">Пример</span><span class="sxs-lookup"><span data-stu-id="edbad-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="edbad-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="edbad-134">Request</span></span>
<span data-ttu-id="edbad-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edbad-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="edbad-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="edbad-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="edbad-137">C#</span><span class="sxs-lookup"><span data-stu-id="edbad-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationthread-from-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="edbad-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edbad-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationthread-from-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="edbad-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="edbad-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationthread-from-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="edbad-140">В теле запроса укажите описание объекта [conversationThread](../resources/conversationthread.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edbad-140">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="edbad-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="edbad-141">Response</span></span>

<span data-ttu-id="edbad-p104">В случае успеха этот метод возвратит код отклика `201 Created` и `id` новой цепочки в теле отклика. Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="edbad-p104">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span>
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
